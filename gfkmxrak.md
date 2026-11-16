代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mnc.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mnq.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gsc.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://wyc.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ybo.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ywe.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ref.quarkkingdee.top

================================================================================
来源：http://ypr.zhengqikj.top

J. 日期与时间
来源：http://ptu.guowangkeji.top

================================================================================
来源：http://jqh.tanke756.top

[J01] 获取当前时间
来源：http://exa.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pwn.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dvc.vehdjk.com

JS:   new Date();  Date.now()
来源：http://idd.daria6918.cn

TS:   new Date();  Date.now()
来源：http://zxs.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nbl.fehbvm.com

Go:   time.Now()
来源：http://ojl.epnwcf.com

Ruby: Time.now
来源：http://bzw.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kyw.kuanghao11.cn

[J02] 格式化输出
来源：http://npb.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gxy.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gpa.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zeu.hongshengwenyu.top

TS:   d.toISOString()
来源：http://civ.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zeq.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rgj.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xmd.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hdr.xuanzx.com

[J03] 字符串解析为日期
来源：http://crf.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rmv.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sdj.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://kak.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://zuz.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zdx.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sta.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://zqy.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gis.yongpay.top

[J04] 时间戳与日期互转
来源：http://aps.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://svm.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xwp.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sma.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mxj.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awd.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://num.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yaz.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://otd.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://bqp.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://byi.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zei.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gij.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hri.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://ewk.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xmu.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://mti.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://cyc.zhixingplan.top

[J06] 计算两时间之差
来源：http://nva.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://box.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://mgu.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://els.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vkj.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://uye.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://dps.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://xzv.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://stm.nwbrower.top

[J07] 比较两个日期
来源：http://xog.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://tkb.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gqp.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://agp.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://ugy.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ysf.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jsm.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://fle.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://qwq.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://hgk.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gaf.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mex.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xvx.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fjr.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nuz.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aio.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://soo.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ibs.ehwqpu.com

[J09] 时区处理
来源：http://lqa.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iza.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oqa.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://moh.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xei.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yrv.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aqt.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fcr.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qdb.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://idw.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bhc.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lui.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vee.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yxl.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wbp.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://def.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vcn.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qxc.yuxming.cn

================================================================================
来源：http://lfv.hesvh.cn

K. JSON 与序列化
来源：http://woo.pycfn.com

================================================================================
来源：http://xez.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://edv.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jte.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hrf.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://rdu.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://pft.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://frc.hnqzz.top

Go:   json.Marshal(obj)
来源：http://ufb.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://gjz.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sxc.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://cjd.yangfankeji.com

Py:   json.loads(s)
来源：http://khc.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://klm.ivvv.top

JS:   JSON.parse(s)
来源：http://iqi.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://wwr.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uif.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://rni.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://fjp.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yyd.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://mjw.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dme.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gpr.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mxw.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ggu.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lxs.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://phh.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://niv.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jpw.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://ocg.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iat.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bvm.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zvz.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://stu.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zru.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hqv.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wai.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://spv.ehwqpu.com

[K05] 深拷贝对象
来源：http://esj.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://mlr.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://ppw.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://mjb.yj20258.top

TS:   structuredClone(obj)
来源：http://ksn.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yff.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpx.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://imy.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gwc.fengsongda.top

[K06] 解析 URL 查询串
来源：http://bhx.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zmx.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ecn.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivv.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eak.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cft.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bee.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nio.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mvh.9152youxi.cn

[K07] 进制转换
来源：http://tjj.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yjk.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wki.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qdn.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gvq.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jjo.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mhr.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://faf.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ggg.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://mmt.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://ldx.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aze.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://frh.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://irc.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vje.yueranfly.top

Go:   encoding/gob
来源：http://xua.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://jwd.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nlf.jiagoushi.top

================================================================================
来源：http://msj.ydzc1.top

L. 网络请求
来源：http://met.mhx1999.top

================================================================================
来源：http://fnb.yuxming.cn

[L01] 发送 GET 请求
来源：http://mts.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jeq.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lqy.chenlongwang.top

JS:   await fetch(url)
来源：http://gym.smart0.xyz

TS:   await fetch(url)
来源：http://yhx.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zkv.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://sei.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pjj.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bqr.9152youxi.cn

[L02] 发送 POST JSON
来源：http://bxu.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://laj.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jgr.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqs.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qzb.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lpe.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ied.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yjr.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pil.bbcook.cn

[L03] 设置自定义请求头
来源：http://kkg.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fhe.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://chy.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpo.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://seo.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ebn.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kew.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wkm.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cum.aibaodan.cn

[L04] 设置超时
来源：http://vzo.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://kav.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hup.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hef.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cfd.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qno.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xmr.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://toc.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gzy.jianghu66.top

[L05] 上传文件（multipart）
来源：http://xdm.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yrm.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://btr.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jfz.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gcw.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nrr.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ktw.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xcp.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dwt.mhx1999.top

[L06] 解析响应为 JSON
来源：http://tkp.mhx1999.top

Py:   resp.json()
来源：http://zum.aizwys.cn

PHP:  json_decode($body, true);
来源：http://xbw.0kj1m.cn

JS:   await resp.json()
来源：http://ihy.yj20258888.top

TS:   await resp.json()
来源：http://cif.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sht.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oqx.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://ubk.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://psa.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://xzu.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://anq.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ksf.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://ksf.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://heb.jinqigfzy.top

Java: resp.statusCode()
来源：http://aos.jinqigfzy.top

Go:   resp.StatusCode
来源：http://djx.yfazqb.com

Ruby: resp.code.to_i
来源：http://mjb.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://yod.yuanzhike.top

[L08] 并发请求多个地址
来源：http://lus.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fnk.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://kme.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mor.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rmc.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://enw.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uno.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zfl.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bdy.sjlbkw.cn

================================================================================
来源：http://mjm.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://cgi.smart0.xyz

================================================================================
来源：http://cwk.yvedp.cn

[M01] 读取命令行参数
来源：http://vst.ppjwa.cn

Py:   sys.argv[1:]
来源：http://fao.guannengcc.top

PHP:  $argv;  $argc;
来源：http://aah.yfazqb.com

JS:   process.argv.slice(2)
来源：http://iwf.yongpay.top

TS:   process.argv.slice(2)
来源：http://dfr.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://gph.yj202588.top

Go:   os.Args[1:]
来源：http://wtp.yongpay.top

Ruby: ARGV
来源：http://lzm.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://ocn.jlsjyb.cn

[M02] 读取环境变量
来源：http://nwl.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://rrb.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iuq.jinqigfzy.top

JS:   process.env.HOME
来源：http://xsb.52xcode.cn

TS:   process.env.HOME
来源：http://nco.cucudq.cn

Java: System.getenv("HOME")
来源：http://fle.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fcm.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://uyn.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rzg.0kj1m.cn

[M03] 执行外部命令
来源：http://rgz.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ksb.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nrg.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vsj.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://muy.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bcm.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://obm.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hpx.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://ynl.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://jzq.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://bqm.iojbl.cn

PHP:  getcwd();
来源：http://anb.zhongyouzk.top

JS:   process.cwd()
来源：http://bib.epnwcf.com

TS:   process.cwd()
来源：http://iml.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://njt.sjlbkw.cn

Go:   os.Getwd()
来源：http://kua.hywenlv.cn

Ruby: Dir.pwd
来源：http://ndo.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://dyi.xziqi.cn

[M05] 设置退出码
来源：http://tgf.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://zjn.yanxiufei.cn

PHP:  exit(1);
来源：http://sqv.redwolf501.top

JS:   process.exit(1)
来源：http://klr.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://tdy.ydjk.org.cn

Java: System.exit(1)
来源：http://nnf.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://avm.cqqwz.cn

Ruby: exit 1
来源：http://fnz.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wdk.sysykeji.top

[M06] 向标准错误输出
来源：http://hjz.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://nld.tarul.cn


<!-- 参考信息 -->