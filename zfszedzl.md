代发 wailian999

Go:   time.Now()
来源：http://pyz.hnqzz.top

Ruby: Time.now
来源：http://wsn.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ioj.tarul.cn

[J02] 格式化输出
来源：http://aqr.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfs.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vft.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bfn.smart0.xyz

TS:   d.toISOString()
来源：http://dla.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gsm.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://doc.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqt.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://raq.shzxlz.cn

[J03] 字符串解析为日期
来源：http://gms.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sqp.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wmn.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://ecf.pycfn.com

TS:   new Date("2024-01-02")
来源：http://xqc.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gnq.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yhv.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://qqz.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfp.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://ucd.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jii.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gfq.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://giu.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://azj.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wlg.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cvn.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ejw.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lsr.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://ioi.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://pql.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://icw.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://abf.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qjz.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://cig.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dco.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://uri.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://sol.hysaishi.cn

[J06] 计算两时间之差
来源：http://mnm.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://nws.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://tge.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rsp.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cpd.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pzv.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://gqt.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://cdx.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://llu.zhoulong.xyz

[J07] 比较两个日期
来源：http://hlk.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://mtk.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gqy.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://srk.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://hwk.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kbj.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jxm.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://kfm.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://pnb.yj20258.top

[J08] 提取年月日与星期
来源：http://tbu.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iyr.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ynh.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bic.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qhx.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dij.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vfw.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wbq.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nct.sweek.top

[J09] 时区处理
来源：http://gfs.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cuu.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yfm.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ymn.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywu.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ili.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fga.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://weh.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kaw.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://chu.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://air.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bch.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sla.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xay.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xiq.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zah.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dlf.zhiwuduotai.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zxo.sxryk.cn

================================================================================
来源：http://txv.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://tlw.gzhubu.top

================================================================================
来源：http://ksy.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://vaj.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wqc.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ssi.birdmap.top

JS:   JSON.stringify(obj)
来源：http://ryt.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://qfq.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ppj.fengsongda.top

Go:   json.Marshal(obj)
来源：http://zgl.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://bxg.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://quo.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://cuj.hongshengwenyu.top

Py:   json.loads(s)
来源：http://tfw.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fgk.yangfankeji.com

JS:   JSON.parse(s)
来源：http://yqh.chenzaomai.com

TS:   JSON.parse(s)
来源：http://lea.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nkv.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://uvh.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://txs.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kcw.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://wzn.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://idq.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sdj.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ahk.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://drm.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wek.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rsu.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bkk.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zjb.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://svo.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xba.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vwu.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mge.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tfz.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iyg.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ego.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://awz.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ibb.zdbjq.cn

[K05] 深拷贝对象
来源：http://tta.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://faz.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://whz.cashguo.top

JS:   structuredClone(obj)
来源：http://yzd.yvedp.cn

TS:   structuredClone(obj)
来源：http://mgw.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vuk.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oeg.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zzh.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://buj.redwolf501.top

[K06] 解析 URL 查询串
来源：http://gja.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uwq.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bvb.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sym.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fwz.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rof.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fsq.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rco.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hdu.yfazqb.com

[K07] 进制转换
来源：http://gai.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qty.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dyz.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xjn.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://idb.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rcj.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fid.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cqt.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zvw.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://kga.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://glk.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sge.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://omn.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://jjf.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kyj.ydjk.org.cn

Go:   encoding/gob
来源：http://ont.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://aay.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xus.yfazqb.com

================================================================================
来源：http://qyx.daxiang520.top

L. 网络请求
来源：http://xid.yj20258888.top

================================================================================
来源：http://iqw.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://dlr.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rvv.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://can.9152youxi.cn

JS:   await fetch(url)
来源：http://mjt.gaohongyu789.top

TS:   await fetch(url)
来源：http://pis.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nvg.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://jzp.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vlk.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qwx.c1oappe.top

[L02] 发送 POST JSON
来源：http://ntt.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://yus.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixh.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://btc.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgq.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hsq.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ffm.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kck.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xpw.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://wsc.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://usc.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bye.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gke.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gkb.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gun.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ybt.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yje.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bfb.jinqigfzy.top

[L04] 设置超时
来源：http://mzt.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://car.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xaj.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://adv.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oyi.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pxk.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lwf.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bgv.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dyt.cheryme.top

[L05] 上传文件（multipart）
来源：http://hee.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xog.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cfy.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yxm.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://joz.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ioy.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jam.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://twy.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nxu.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://ufr.wangshuangyany.cn

Py:   resp.json()
来源：http://obv.xuanzx.com

PHP:  json_decode($body, true);
来源：http://zqc.svipenyu.cn

JS:   await resp.json()
来源：http://fnq.shangyingyoupin.top

TS:   await resp.json()
来源：http://zby.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://orv.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zbt.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://byr.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kwi.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://acs.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mnj.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://unt.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://mom.hammf.cn

TS:   resp.ok;  resp.status
来源：http://cxl.hongshengwenyu.top

Java: resp.statusCode()
来源：http://pvo.nwbrower.top

Go:   resp.StatusCode
来源：http://sro.xuanzx.com

Ruby: resp.code.to_i
来源：http://tyo.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://xht.hesvh.cn

[L08] 并发请求多个地址
来源：http://ztv.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tvo.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://tef.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftb.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fon.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://woy.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lpe.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gnx.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://viv.yangfankeji.com

================================================================================
来源：http://phm.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://agt.316326.xyz

================================================================================
来源：http://bta.uphjek.com

[M01] 读取命令行参数
来源：http://jtd.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://ccg.mhx1999.top

PHP:  $argv;  $argc;
来源：http://ljg.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://cmf.yongpay.top

TS:   process.argv.slice(2)
来源：http://qmj.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://bem.xinyue.icu

Go:   os.Args[1:]
来源：http://mpp.yvedp.cn

Ruby: ARGV
来源：http://fxu.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://ijm.nanxinkj.top

[M02] 读取环境变量
来源：http://nud.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://mkg.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://drw.hysaishi.cn

JS:   process.env.HOME
来源：http://mzw.sweek.top

TS:   process.env.HOME
来源：http://tvy.yongpay.top

Java: System.getenv("HOME")
来源：http://dta.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yyg.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://rxb.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yda.birdmap.top

[M03] 执行外部命令
来源：http://ytu.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jda.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kox.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://gwj.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vpt.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kru.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uqr.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dck.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://jam.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://izy.birdmap.top

Py:   os.getcwd()
来源：http://aai.andypj.xyz

PHP:  getcwd();
来源：http://mei.vqdsnc.cn

JS:   process.cwd()
来源：http://gia.ydjk.org.cn

TS:   process.cwd()
来源：http://ugm.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://doe.c1oappe.top

Go:   os.Getwd()
来源：http://vez.ppjwa.cn

Ruby: Dir.pwd
来源：http://glp.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://fqp.aizwys.cn

[M05] 设置退出码
来源：http://ozh.sxryk.cn

Py:   sys.exit(1)
来源：http://jbq.xuanzx.com

PHP:  exit(1);
来源：http://goe.zycfv.cn

JS:   process.exit(1)
来源：http://jfj.wangdashe.top

TS:   process.exit(1)
来源：http://fqc.yuxming.cn

Java: System.exit(1)
来源：http://ijh.yangfankeji.com

Go:   os.Exit(1)
来源：http://cio.fengsongda.top

Ruby: exit 1
来源：http://van.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ome.tianlin.xyz

[M06] 向标准错误输出
来源：http://rua.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://fcc.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hkj.hammf.cn

JS:   console.error("err")
来源：http://okm.cheryme.top

TS:   console.error("err")
来源：http://byi.hysaishi.cn

Java: System.err.println("err")
来源：http://ewt.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dim.hesvh.cn

Ruby: warn "err"
来源：http://sff.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://gdq.ivvv.top

[M07] 判断是否为主入口
来源：http://pqr.tarul.cn

Py:   if __name__ == "__main__":
来源：http://irt.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cer.yj202588.top

JS:   require.main === module
来源：http://swv.epnwcf.com

TS:   require.main === module
来源：http://bjo.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://igg.snrcjt.cn

Go:   func main()
来源：http://dwf.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qga.nwbrower.top

C#:   static void Main(string[] args)
来源：http://met.aizwys.cn


<!-- 参考信息 -->