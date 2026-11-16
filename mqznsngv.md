代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://shs.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dse.ivvv.top

[I04] 正则替换
来源：http://yes.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ysf.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kvf.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yqr.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://aji.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://eiq.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ctw.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rre.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jsd.hysaishi.cn

[I05] 按正则拆分
来源：http://bub.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rep.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vnr.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://gkb.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://lpb.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://vrc.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ubk.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://flu.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://igg.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hkq.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ilg.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://usi.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aja.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://njb.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wcl.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tyj.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qkx.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tuf.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://ykk.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vkq.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kjf.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rhd.tian-w.cn

TS:   /error/gim
来源：http://aum.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ddk.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hrb.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://pmy.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://anp.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://jrr.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ftu.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zpm.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wft.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxy.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vqz.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tiz.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pgf.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ykd.jyoumei.cn

================================================================================
来源：http://gra.gzhubu.top

J. 日期与时间
来源：http://hma.gogol.net.cn

================================================================================
来源：http://jpd.yuanzhike.top

[J01] 获取当前时间
来源：http://aam.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bxn.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xfl.vehdjk.com

JS:   new Date();  Date.now()
来源：http://yle.wangdashe.top

TS:   new Date();  Date.now()
来源：http://hlx.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://skm.xinyue.icu

Go:   time.Now()
来源：http://mkk.tian-w.cn

Ruby: Time.now
来源：http://fxs.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uko.shangyingyoupin.top

[J02] 格式化输出
来源：http://tjo.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqn.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kgq.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lpg.yj20258.top

TS:   d.toISOString()
来源：http://zqx.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qqc.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ppf.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://giy.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://opq.havefunace.top

[J03] 字符串解析为日期
来源：http://pjx.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fmb.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rvc.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://dud.yj202588.top

TS:   new Date("2024-01-02")
来源：http://yll.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vos.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ilb.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://geo.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://icd.yvedp.cn

[J04] 时间戳与日期互转
来源：http://kij.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vfn.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://inj.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ygo.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jtl.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hpu.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uve.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fpc.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wms.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://myx.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://xxm.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mfu.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tad.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ygl.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://mgo.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iln.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://tpc.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://iga.yj20258.top

[J06] 计算两时间之差
来源：http://oxz.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://xjs.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://hyg.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxl.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pat.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://uxn.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://cpy.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://yyo.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://dnb.hysaishi.cn

[J07] 比较两个日期
来源：http://gii.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://eml.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rql.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lgv.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://brz.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pib.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tbh.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://abv.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://are.aizwys.cn

[J08] 提取年月日与星期
来源：http://kjq.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://upc.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nta.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wai.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://erp.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nbq.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iqw.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://srn.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fdx.yangfankeji.com

[J09] 时区处理
来源：http://vqb.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vht.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ncb.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rmx.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vsd.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mis.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hlx.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sqy.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uoe.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://ddk.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ezo.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zba.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zyj.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://csw.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pkw.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://djf.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wou.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dui.daxiang520.top

================================================================================
来源：http://vey.jqgfzy.top

K. JSON 与序列化
来源：http://cfz.pengpengdd.cyou

================================================================================
来源：http://ygt.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://aqs.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qwv.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ysb.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://pzr.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://mor.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hao.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://sjt.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ahn.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://evt.tarul.cn

[K02] JSON 字符串转对象
来源：http://yra.hesvh.cn

Py:   json.loads(s)
来源：http://akx.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fav.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://qao.hammf.cn

TS:   JSON.parse(s)
来源：http://koj.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dju.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://hck.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://jsn.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rqr.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://fpe.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fvd.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cnm.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wqk.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://xer.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rkd.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xsj.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hth.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tko.guannengcc.top

[K04] 读取 JSON 文件
来源：http://yhr.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ipm.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hvz.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zuf.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://edt.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wpy.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qzo.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lfm.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lml.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://hem.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://mhl.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://epg.zhixingplan.top

JS:   structuredClone(obj)
来源：http://xlx.sysykeji.top

TS:   structuredClone(obj)
来源：http://npn.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://koq.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zjo.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rov.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://axo.xinyue.icu

[K06] 解析 URL 查询串
来源：http://ndv.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bdy.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rmd.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qgu.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujn.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://urg.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nwl.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://smv.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://msl.tian-w.cn

[K07] 进制转换
来源：http://him.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vmo.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mun.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gox.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dqs.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pfu.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mim.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://asr.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wdz.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://snp.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://wge.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pok.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://xwa.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://tup.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fcy.zhoulong.xyz

Go:   encoding/gob
来源：http://cst.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://htc.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cec.quarkkingdee.top

================================================================================
来源：http://ieq.yonumen.top

L. 网络请求
来源：http://jpm.svipenyu.cn

================================================================================
来源：http://myt.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://nof.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jzb.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tks.cheryme.top

JS:   await fetch(url)
来源：http://uly.yj202588.top

TS:   await fetch(url)
来源：http://qpr.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://duo.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://kdq.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iiq.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jbc.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://cdp.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gex.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gyq.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oyt.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nvq.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sjx.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yca.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pec.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wot.guowangkeji.top

[L03] 设置自定义请求头
来源：http://ahf.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ztf.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txg.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zsb.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ehq.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fsn.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://diu.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dcq.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yjl.ybcxt.top

[L04] 设置超时
来源：http://kyw.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://pll.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sft.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbf.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://awv.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zxd.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wcx.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jgj.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rhx.yueranfly.top

[L05] 上传文件（multipart）
来源：http://woo.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yqk.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://szb.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gfc.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ffb.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uyn.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ylh.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ibw.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oqe.52xcode.cn

[L06] 解析响应为 JSON
来源：http://umm.ctjpmb.com

Py:   resp.json()
来源：http://vcy.nwbrower.top

PHP:  json_decode($body, true);
来源：http://aqu.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://asj.xylfe.cn

TS:   await resp.json()
来源：http://ngf.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ysl.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rss.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://ari.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sne.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://gnt.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hdy.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyf.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://nwq.sweek.top

TS:   resp.ok;  resp.status
来源：http://tof.cheryme.top

Java: resp.statusCode()
来源：http://bhd.tanke756.top

Go:   resp.StatusCode
来源：http://cax.aizwys.cn

Ruby: resp.code.to_i
来源：http://voa.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://fgu.yuanzhike.top

[L08] 并发请求多个地址
来源：http://lyf.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fgo.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://zpl.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://loc.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lgt.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://car.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dmc.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fgq.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bqv.jqgufenzy.top

================================================================================
来源：http://xwd.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://rix.316326.xyz

================================================================================
来源：http://tuz.sysykeji.top

[M01] 读取命令行参数
来源：http://dhm.yfazqb.com

Py:   sys.argv[1:]
来源：http://vvv.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://jfk.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://coa.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://uvc.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://nlf.yvedp.cn

Go:   os.Args[1:]
来源：http://awx.kuanghao11.cn


<!-- 参考信息 -->