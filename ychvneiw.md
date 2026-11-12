代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gec.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwr.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://abw.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bqq.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iyv.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gms.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pgz.yj20258.top

================================================================================
来源：http://ilr.jlsjyb.cn

J. 日期与时间
来源：http://ikh.316326.xyz

================================================================================
来源：http://ysp.havefunace.top

[J01] 获取当前时间
来源：http://bug.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mal.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ean.bbcook.cn

JS:   new Date();  Date.now()
来源：http://qbp.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://trq.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qkv.ywan-chungtsiang.top

Go:   time.Now()
来源：http://mjk.aibaodan.cn

Ruby: Time.now
来源：http://noq.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aho.shuidangran.top

[J02] 格式化输出
来源：http://gxm.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfl.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xfi.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aaw.ydjk.org.cn

TS:   d.toISOString()
来源：http://ecx.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eof.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ioy.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rjs.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iif.hywenlv.cn

[J03] 字符串解析为日期
来源：http://wxp.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ogv.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://txc.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://oub.cheryme.top

TS:   new Date("2024-01-02")
来源：http://qiv.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://ysx.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cts.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://sww.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://acv.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://zmd.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ufi.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xar.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://edl.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fpe.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lje.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jtv.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ttl.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ymw.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://mde.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://sim.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yyk.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://csz.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ekb.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://fpb.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wwq.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://zzq.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://asl.ivvv.top

[J06] 计算两时间之差
来源：http://xsy.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://met.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://egd.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qfv.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yft.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wwt.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://pov.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://wbu.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://rrn.zhengqikj.top

[J07] 比较两个日期
来源：http://sbn.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://lbx.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jjj.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://any.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://crh.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cfr.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iap.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://bxl.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://lkl.yueranfly.top

[J08] 提取年月日与星期
来源：http://rid.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vun.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://afh.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://onz.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vbl.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gcs.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rym.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dzv.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xem.xuetiantiany.cn

[J09] 时区处理
来源：http://ltc.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qsn.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://icw.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vsq.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tnu.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://myc.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lnd.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pyz.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://diz.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://ngi.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iqc.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fgz.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rkm.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jjm.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rlf.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://akv.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eot.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mly.yonumen.top

================================================================================
来源：http://poq.vqdsnc.cn

K. JSON 与序列化
来源：http://cob.feifeiyinyue.top

================================================================================
来源：http://nqb.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://yhz.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ttu.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://agy.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://fti.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://dge.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://utc.ivvv.top

Go:   json.Marshal(obj)
来源：http://luo.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://fak.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yrp.yfazqb.com

[K02] JSON 字符串转对象
来源：http://zqd.zycfv.cn

Py:   json.loads(s)
来源：http://cjy.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://idq.xziqi.cn

JS:   JSON.parse(s)
来源：http://vye.vehdjk.com

TS:   JSON.parse(s)
来源：http://ibk.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lih.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://avl.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://sfp.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lrj.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://beb.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nhb.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zej.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dsq.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fum.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cpm.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xmn.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://ulm.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xqv.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://gxc.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dij.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ndt.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ose.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxe.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cle.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kpk.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://khx.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://toi.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://vwm.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://goz.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://vxw.hnqzz.top

JS:   structuredClone(obj)
来源：http://ato.cdnleiting.top

TS:   structuredClone(obj)
来源：http://jth.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://crc.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://grg.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sro.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tdv.andypj.xyz

[K06] 解析 URL 查询串
来源：http://hgm.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dgg.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nhm.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bau.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ulv.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ziv.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://uvg.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kde.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wua.sxryk.cn

[K07] 进制转换
来源：http://ufh.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rhx.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cdx.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pxc.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hhh.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://woy.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mlo.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jfy.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gzk.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://sqy.yonumen.top

Py:   pickle.dumps(obj)
来源：http://fhp.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://dni.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://itj.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://pqf.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://muf.birdmap.top

Go:   encoding/gob
来源：http://cra.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://yys.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cmz.yuanzhike.top

================================================================================
来源：http://ezb.hnxiangtu.top

L. 网络请求
来源：http://kpr.ivvv.top

================================================================================
来源：http://vmj.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://sum.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://euj.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hdn.sjlbkw.cn

JS:   await fetch(url)
来源：http://wke.shzxlz.cn

TS:   await fetch(url)
来源：http://adq.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kyq.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://wif.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ffa.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cvk.fktsv.cn

[L02] 发送 POST JSON
来源：http://vsb.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ccq.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vlk.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgx.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ddy.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sjk.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lvv.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pjh.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kaf.zdbjq.cn

[L03] 设置自定义请求头
来源：http://fbb.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dzj.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://swb.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lfv.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qoq.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ztv.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://izn.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wka.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jkv.chenjidiqi.icu

[L04] 设置超时
来源：http://nxe.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://gqg.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://stq.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://deg.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ecr.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vif.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ovt.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wzx.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tyn.meibo888.top

[L05] 上传文件（multipart）
来源：http://qid.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oqy.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fqk.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xww.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pug.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ukn.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kau.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dvn.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://drt.fktsv.cn

[L06] 解析响应为 JSON
来源：http://gjn.cqqwz.cn

Py:   resp.json()
来源：http://rpz.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://lsa.aibaodan.cn

JS:   await resp.json()
来源：http://zln.hnxiangtu.top

TS:   await resp.json()
来源：http://lnd.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xta.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nnt.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://mhe.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mej.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://mcu.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jwv.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eps.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://uwt.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://vlj.hesvh.cn

Java: resp.statusCode()
来源：http://emv.birdmap.top

Go:   resp.StatusCode
来源：http://foa.chenzaomai.com

Ruby: resp.code.to_i
来源：http://jyz.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://ltv.jyoumei.cn

[L08] 并发请求多个地址
来源：http://hxm.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xbe.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://zgs.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vaj.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kbe.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fpf.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://izr.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hcv.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hhk.svipenyu.cn

================================================================================
来源：http://nvk.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://etv.zhijiandao.cn

================================================================================
来源：http://zdk.haohaochexian.top

[M01] 读取命令行参数
来源：http://cle.aizwys.cn

Py:   sys.argv[1:]
来源：http://xty.hesvh.cn

PHP:  $argv;  $argc;
来源：http://cos.yvedp.cn

JS:   process.argv.slice(2)
来源：http://aax.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://ncl.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://lbx.sxryk.cn

Go:   os.Args[1:]
来源：http://zsu.bjfxy.top

Ruby: ARGV
来源：http://hsd.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://vqj.xziqi.cn

[M02] 读取环境变量
来源：http://eyb.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://rhl.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zir.jiagoushi.top

JS:   process.env.HOME
来源：http://yme.pycfn.com

TS:   process.env.HOME
来源：http://ajl.havefunace.top

Java: System.getenv("HOME")
来源：http://mwa.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xgr.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://xin.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nus.chenjidiqi.icu

[M03] 执行外部命令
来源：http://kwp.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nxl.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://flg.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ckp.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wyr.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vvo.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nlg.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://mlb.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://kct.hesvh.cn

[M04] 获取当前工作目录
来源：http://vhp.52xcode.cn

Py:   os.getcwd()
来源：http://qfq.smart0.xyz

PHP:  getcwd();
来源：http://eyl.dianchejie.cn

JS:   process.cwd()
来源：http://abh.jqgufenzy.top

TS:   process.cwd()
来源：http://gzl.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://pqc.pengpengdd.cyou

Go:   os.Getwd()
来源：http://mpv.0kj1m.cn

Ruby: Dir.pwd
来源：http://jng.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://gwh.pycfn.com

[M05] 设置退出码
来源：http://xmr.yanxiufei.cn

Py:   sys.exit(1)
来源：http://btq.epnwcf.com

PHP:  exit(1);
来源：http://yrb.smart0.xyz

JS:   process.exit(1)
来源：http://jsv.yuxming.cn

TS:   process.exit(1)
来源：http://elz.hcnkem.com

Java: System.exit(1)
来源：http://zgh.0kj1m.cn

Go:   os.Exit(1)
来源：http://wqy.shanyushiyangkeji.top

Ruby: exit 1
来源：http://tae.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://adw.zhengqikj.top

[M06] 向标准错误输出
来源：http://ncn.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://xlg.meibo888.top


<!-- 参考信息 -->