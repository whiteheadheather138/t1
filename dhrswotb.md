代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://zdv.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mcg.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://enr.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://esk.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vvo.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bha.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lfu.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bda.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cif.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ldw.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://brb.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rrp.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uyg.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://kgp.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ybz.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kco.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dub.dashuyun.cn

TS:   /error/gim
来源：http://tgi.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pdx.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zzp.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://iiy.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bhi.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://oum.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gsw.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tzv.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zid.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://muz.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yst.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://trt.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dkd.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wmb.birdmap.top

================================================================================
来源：http://lzo.0kj1m.cn

J. 日期与时间
来源：http://pes.ivvv.top

================================================================================
来源：http://bnc.hcnkem.com

[J01] 获取当前时间
来源：http://rtq.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rqn.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ffa.bbcook.cn

JS:   new Date();  Date.now()
来源：http://kim.ivvv.top

TS:   new Date();  Date.now()
来源：http://kcm.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://zvw.hesvh.cn

Go:   time.Now()
来源：http://ojf.zhoulong.xyz

Ruby: Time.now
来源：http://nss.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bxf.yj20258888.top

[J02] 格式化输出
来源：http://uiv.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwv.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ipo.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pyu.hongshengwenyu.top

TS:   d.toISOString()
来源：http://poo.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cnj.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hbx.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ihk.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fiq.zdqjudy.top

[J03] 字符串解析为日期
来源：http://vfd.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qvj.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ndt.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://lfi.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://ern.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iwd.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xub.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://hor.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jml.xinyue.icu

[J04] 时间戳与日期互转
来源：http://mlv.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tum.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://att.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qpf.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ooo.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hdk.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zxa.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tsa.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mlu.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://egu.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://wpf.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vvx.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bbv.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtz.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://xsc.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://buy.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://tih.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://gxn.xuanzx.com

[J06] 计算两时间之差
来源：http://xqa.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://gav.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://jod.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svi.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://etx.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://ujs.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://git.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://khz.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://pcz.cheryme.top

[J07] 比较两个日期
来源：http://rxd.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://xxx.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pec.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://jyz.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://tbi.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uce.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ukc.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://blq.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://xip.svipenyu.cn

[J08] 提取年月日与星期
来源：http://drl.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wkz.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfz.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mwx.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qqp.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dgc.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xim.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://npw.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kpb.birdmap.top

[J09] 时区处理
来源：http://fem.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yym.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aer.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcz.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jek.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tjo.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tho.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jac.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sbe.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://joo.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jpm.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ltv.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qce.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hyg.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dot.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xhk.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pey.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dyq.zhixingplan.top

================================================================================
来源：http://wkm.shzxlz.cn

K. JSON 与序列化
来源：http://qvr.sufxvd.cn

================================================================================
来源：http://gee.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://jke.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://twd.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xki.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://vop.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://mad.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ybs.zycfv.cn

Go:   json.Marshal(obj)
来源：http://xeb.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://fez.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://hfz.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://qzh.yuanzhike.top

Py:   json.loads(s)
来源：http://blk.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oyk.tarul.cn

JS:   JSON.parse(s)
来源：http://prv.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://bgc.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tbt.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://nth.fengsongda.top

Ruby: JSON.parse(s)
来源：http://wil.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qhu.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://wbu.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eit.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://llk.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vqr.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vdk.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ffy.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oxv.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://bwg.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zlu.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://zva.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mbw.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cqy.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tsf.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://elo.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kkf.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://paq.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qjw.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kyo.jqgufenzy.top

[K05] 深拷贝对象
来源：http://pon.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://xoh.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://qza.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://wgj.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://bxu.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://dqs.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ijb.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eag.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cwn.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://jso.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tgy.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lvn.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nfk.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nvg.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wlt.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://krt.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://irw.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fci.gzhubu.top

[K07] 进制转换
来源：http://lfx.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gmn.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yav.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mzd.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cif.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uji.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bof.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bff.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nwv.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://ims.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://adz.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gii.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://eqb.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://uag.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rly.yj20258888.top

Go:   encoding/gob
来源：http://qum.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://geg.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qhj.quarkkingdee.top

================================================================================
来源：http://wgn.gaohongyu789.top

L. 网络请求
来源：http://jkv.feifeiyinyue.top

================================================================================
来源：http://lnl.guannengcc.top

[L01] 发送 GET 请求
来源：http://mpl.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pvv.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kjr.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://hsh.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://lod.hongshengwenyu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://krw.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://muv.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xnd.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ayw.xziqi.cn

[L02] 发送 POST JSON
来源：http://kjf.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pai.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zjy.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gjy.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bcb.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jjg.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://evv.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mga.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wid.zhixingplan.top

[L03] 设置自定义请求头
来源：http://frk.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dnd.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tep.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sha.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qwf.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dxi.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ewr.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rmc.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bei.svipenyu.cn

[L04] 设置超时
来源：http://ovv.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://wad.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rxw.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://abl.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syn.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ifi.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ogs.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hzj.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tvm.xinyue.icu

[L05] 上传文件（multipart）
来源：http://jhm.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yxe.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zlf.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wwh.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wsy.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://drn.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ege.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tqw.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wjb.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://nfa.zhoulong.xyz

Py:   resp.json()
来源：http://jlh.pycfn.com

PHP:  json_decode($body, true);
来源：http://eyj.sxryk.cn

JS:   await resp.json()
来源：http://vft.nanxuanxn.top

TS:   await resp.json()
来源：http://iww.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gvt.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zaf.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://agl.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://smv.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://afu.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sxg.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uiy.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://vxo.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://ets.vqdsnc.cn

Java: resp.statusCode()
来源：http://wjz.jlsjyb.cn

Go:   resp.StatusCode
来源：http://ceb.yuxming.cn

Ruby: resp.code.to_i
来源：http://suy.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://vlt.ehwqpu.com

[L08] 并发请求多个地址
来源：http://lzt.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tbi.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://ixu.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://avi.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://soc.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vyc.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kdn.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zrl.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zjw.jyoumei.cn

================================================================================
来源：http://zsd.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://uuu.hongshengwenyu.top

================================================================================
来源：http://prp.yueranfly.top

[M01] 读取命令行参数
来源：http://tft.mhx1999.top

Py:   sys.argv[1:]
来源：http://apm.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://sap.fzhhl.top

JS:   process.argv.slice(2)
来源：http://hkz.fengsongda.top

TS:   process.argv.slice(2)
来源：http://mzs.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://fyy.jiagoushi.top

Go:   os.Args[1:]
来源：http://scv.snrcjt.cn

Ruby: ARGV
来源：http://wes.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://dff.guannengcc.top

[M02] 读取环境变量
来源：http://uiz.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://osa.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://seo.vehdjk.com

JS:   process.env.HOME
来源：http://cbj.birdmap.top

TS:   process.env.HOME
来源：http://etp.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://eee.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pkj.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://cqm.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ttz.yj202588.top

[M03] 执行外部命令
来源：http://pdr.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cwx.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hiq.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bte.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://syd.smart0.xyz


<!-- 参考信息 -->