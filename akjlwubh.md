代发 wailian999

J. 日期与时间
来源：http://ofu.hnxiangtu.top

================================================================================
来源：http://xfi.jinqigufen.top

[J01] 获取当前时间
来源：http://nhm.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vtm.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bxg.hesvh.cn

JS:   new Date();  Date.now()
来源：http://qkn.redwolf501.top

TS:   new Date();  Date.now()
来源：http://uph.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://puo.tianlin.xyz

Go:   time.Now()
来源：http://uqa.jlsjyb.cn

Ruby: Time.now
来源：http://mwq.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lao.ppjwa.cn

[J02] 格式化输出
来源：http://pem.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://idl.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lkb.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hcv.cucudq.cn

TS:   d.toISOString()
来源：http://dcb.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kqc.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ojt.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anx.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vmt.mhx1999.top

[J03] 字符串解析为日期
来源：http://qti.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lip.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ruh.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://vte.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://nus.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cuv.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jrk.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://ibv.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sld.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://val.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ziw.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://okj.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ikx.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://hme.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vby.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ofk.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tjr.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wjq.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://bef.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://pbl.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://efk.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://noz.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nhq.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://efb.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rjs.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://elf.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pwq.snrcjt.cn

[J06] 计算两时间之差
来源：http://ctj.tanke756.top

Py:   (end - start).total_seconds()
来源：http://rek.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://fsz.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://koe.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://udz.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://goh.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://smw.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://zbj.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://grh.vehdjk.com

[J07] 比较两个日期
来源：http://ibf.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://run.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qzk.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://qsv.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://uvi.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rmv.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fbe.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://szd.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://sfo.uphjek.com

[J08] 提取年月日与星期
来源：http://iol.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bsw.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://glg.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ogk.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ezi.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://suo.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uff.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mpg.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixc.chenlongwang.top

[J09] 时区处理
来源：http://rtt.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfq.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sfx.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axr.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ank.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rzt.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yod.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://hlv.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vfi.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://qbm.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://zxz.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ucg.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vlh.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tup.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yfy.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jzy.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://atb.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ons.kuanghao11.cn

================================================================================
来源：http://eal.mhx1999.top

K. JSON 与序列化
来源：http://mtf.birdmap.top

================================================================================
来源：http://pxa.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://vbo.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cat.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mke.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://hzp.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://bbo.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yjb.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://exz.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://omn.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mgz.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://xzo.hysaishi.cn

Py:   json.loads(s)
来源：http://uby.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wij.zhengqikj.top

JS:   JSON.parse(s)
来源：http://stv.tian-w.cn

TS:   JSON.parse(s)
来源：http://xsp.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ydy.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://vmb.ivvv.top

Ruby: JSON.parse(s)
来源：http://pbo.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qnr.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://yat.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cop.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jld.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://srv.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://mgo.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izu.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gvd.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://msj.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://onz.bbcook.cn

[K04] 读取 JSON 文件
来源：http://yys.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ciq.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://owq.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mmg.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zij.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hsb.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://imp.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ptk.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qnc.sufxvd.cn

[K05] 深拷贝对象
来源：http://qut.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://xsa.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://szr.snrcjt.cn

JS:   structuredClone(obj)
来源：http://koz.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://ovq.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://fdj.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ffb.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lpn.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://soi.yanxiufei.cn

[K06] 解析 URL 查询串
来源：http://lnr.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pdt.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oya.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cjm.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wvt.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lkd.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://boj.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://emy.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://byu.tarul.cn

[K07] 进制转换
来源：http://avm.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://haq.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uul.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fqf.zhengqikj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vux.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mku.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tez.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yvk.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mey.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://ttn.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://wtz.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://twu.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://tsd.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://wsm.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kjv.xuetiantiany.cn

Go:   encoding/gob
来源：http://gwm.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://bzb.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jvz.zhoulong.xyz

================================================================================
来源：http://eor.pycfn.com

L. 网络请求
来源：http://alk.yanxiufei.cn

================================================================================
来源：http://eba.aizwys.cn

[L01] 发送 GET 请求
来源：http://xac.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://egz.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iov.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://wmj.wangdashe.top

TS:   await fetch(url)
来源：http://cna.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://alb.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://zms.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://urr.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uaz.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://yyj.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://sej.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://peh.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjo.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lws.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sch.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://smk.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fpt.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ihq.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://nkx.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rnj.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nlo.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://und.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cre.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vjs.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dng.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ulp.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oaa.jinqigufen.top

[L04] 设置超时
来源：http://nvo.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://xiu.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://efo.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://khn.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kbk.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://efn.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nwr.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qay.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qbi.cucudq.cn

[L05] 上传文件（multipart）
来源：http://xsa.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dho.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bvm.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jbx.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zkh.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mdf.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zdr.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://imo.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ncs.tarul.cn

[L06] 解析响应为 JSON
来源：http://bwr.guannengcc.top

Py:   resp.json()
来源：http://yap.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://yxz.mhx1999.top

JS:   await resp.json()
来源：http://hfy.zhixingplan.top

TS:   await resp.json()
来源：http://wcv.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ike.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iur.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://vwq.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oij.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://inz.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fkh.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ffu.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://ewq.tanke756.top

TS:   resp.ok;  resp.status
来源：http://gdf.ehwqpu.com

Java: resp.statusCode()
来源：http://whc.yvedp.cn

Go:   resp.StatusCode
来源：http://zsy.smart0.xyz

Ruby: resp.code.to_i
来源：http://pdb.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://eil.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://sad.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ubp.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://qdz.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vbg.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utw.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://unn.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rjf.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ayy.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dim.jinqigfzy.top

================================================================================
来源：http://xwt.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://eko.daria6918.cn

================================================================================
来源：http://evu.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://rrm.shzxlz.cn

Py:   sys.argv[1:]
来源：http://gii.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://xvj.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://tec.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://naj.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://ugt.yfazqb.com

Go:   os.Args[1:]
来源：http://zhc.bbcook.cn

Ruby: ARGV
来源：http://gjq.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://mvn.jiagoushi.top

[M02] 读取环境变量
来源：http://ifn.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://jvx.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fua.xylfe.cn

JS:   process.env.HOME
来源：http://hqv.snrcjt.cn

TS:   process.env.HOME
来源：http://geo.nwbrower.top

Java: System.getenv("HOME")
来源：http://pqh.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xmj.yj20258888.top

Ruby: ENV["HOME"]
来源：http://hha.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qfi.zhijiandao.cn

[M03] 执行外部命令
来源：http://ddt.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://scf.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bhl.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://sir.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mzt.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zma.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fdl.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://gpv.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://ltq.iojbl.cn

[M04] 获取当前工作目录
来源：http://fry.jinqigfzy.top

Py:   os.getcwd()
来源：http://udp.quarkkingdee.top

PHP:  getcwd();
来源：http://uae.yj202588.top

JS:   process.cwd()
来源：http://ebb.uphjek.com

TS:   process.cwd()
来源：http://hjx.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://rwc.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://lah.ppjwa.cn

Ruby: Dir.pwd
来源：http://rtp.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jme.hammf.cn

[M05] 设置退出码
来源：http://igb.yj202588.top

Py:   sys.exit(1)
来源：http://egd.xuetiantiany.cn

PHP:  exit(1);
来源：http://vev.gotoacloud.top

JS:   process.exit(1)
来源：http://sjk.jiagoushi.top

TS:   process.exit(1)
来源：http://myz.sysykeji.top

Java: System.exit(1)
来源：http://xze.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://dgd.gzhubu.top

Ruby: exit 1
来源：http://sxs.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hxe.zhixingplan.top

[M06] 向标准错误输出
来源：http://cgb.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://jlj.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://fie.shanyushiyangtech.top

JS:   console.error("err")
来源：http://lbm.xylfe.cn

TS:   console.error("err")
来源：http://aou.jqgfzy.top

Java: System.err.println("err")
来源：http://vjl.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vcn.daria6918.cn

Ruby: warn "err"
来源：http://djq.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://irc.sufxvd.cn

[M07] 判断是否为主入口
来源：http://zgl.snrcjt.cn


<!-- 参考信息 -->