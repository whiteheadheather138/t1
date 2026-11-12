代发 wailian999

Go:   time.Now()
来源：http://fxo.bbcook.cn

Ruby: Time.now
来源：http://nht.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://noa.hfpthk.cn

[J02] 格式化输出
来源：http://lbf.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oyy.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xjq.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zju.hnqzz.top

TS:   d.toISOString()
来源：http://ymw.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bkd.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rwv.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oip.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bqr.yfazqb.com

[J03] 字符串解析为日期
来源：http://szz.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xes.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nxd.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://hob.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://ohl.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lor.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://plo.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://wrq.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://srq.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://oya.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yir.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gzs.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eym.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gsj.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bmp.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hpb.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wam.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://doo.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://dkh.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://elk.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qvj.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rdg.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbe.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://xpd.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iar.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://iav.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://oql.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://bbg.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://epc.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://ams.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://art.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://izf.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://suq.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://gjh.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://hod.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://vgz.redwolf501.top

[J07] 比较两个日期
来源：http://ahz.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://nrk.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cos.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://yls.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zkq.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wfn.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lus.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://mbo.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://kzq.dianchejie.cn

[J08] 提取年月日与星期
来源：http://mpe.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iuv.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wmx.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vjz.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kxs.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tuv.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xey.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dcs.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pij.jinyuanbaomall.cn

[J09] 时区处理
来源：http://cmq.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mcs.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zod.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://plj.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sgs.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mxr.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oji.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dur.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mkb.sweek.top

[J10] 取今天 / 本月第一天
来源：http://zqe.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tir.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uev.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vqa.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vim.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rgg.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hlb.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hka.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uod.hnxiangtu.top

================================================================================
来源：http://ejr.iojbl.cn

K. JSON 与序列化
来源：http://xsp.zhaomingkeji.xyz

================================================================================
来源：http://hhm.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://lrv.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gzi.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tiq.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://zzq.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://wqp.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cnd.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://xwa.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wmz.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jfp.xinyue.icu

[K02] JSON 字符串转对象
来源：http://wlo.xinyue.icu

Py:   json.loads(s)
来源：http://qkk.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://clb.ehwqpu.com

JS:   JSON.parse(s)
来源：http://cip.fehbvm.com

TS:   JSON.parse(s)
来源：http://woh.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pyn.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://fpf.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://xfx.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jfq.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://qth.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uez.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lhk.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zeh.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tgq.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uiq.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://skf.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://loq.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://czi.zycfv.cn

[K04] 读取 JSON 文件
来源：http://rer.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hzb.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dsa.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dht.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://shj.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gsy.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sua.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vab.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yvj.hfpthk.cn

[K05] 深拷贝对象
来源：http://dfb.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://sde.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://mgs.guowangkeji.top

JS:   structuredClone(obj)
来源：http://pas.haohaochexian.top

TS:   structuredClone(obj)
来源：http://mek.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://gzd.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ojm.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wvq.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://idx.fzhhl.top

[K06] 解析 URL 查询串
来源：http://cqw.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sjq.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fvj.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kpb.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lot.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ewg.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jgw.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oia.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uhi.daxiang520.top

[K07] 进制转换
来源：http://mhj.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xjz.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nyd.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://byx.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mup.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jgd.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mjv.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cfy.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lis.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://baf.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://hra.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jfk.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://top.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://yko.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iel.zdbjq.cn

Go:   encoding/gob
来源：http://cnk.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://ukx.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lwm.yfazqb.com

================================================================================
来源：http://lmm.yueranfly.top

L. 网络请求
来源：http://qes.ctjpmb.com

================================================================================
来源：http://wuo.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://mbb.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://slb.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qpg.yj20258888.top

JS:   await fetch(url)
来源：http://rdi.cdnleiting.top

TS:   await fetch(url)
来源：http://drs.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kud.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://htj.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qox.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wlq.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://tky.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://xlv.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dkv.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ypi.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://woq.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://egt.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tnh.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmj.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wkn.iojbl.cn

[L03] 设置自定义请求头
来源：http://gsw.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gaz.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://upc.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgz.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xhn.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lii.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dzg.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mta.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ore.ydjk.org.cn

[L04] 设置超时
来源：http://qni.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://awx.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jms.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwc.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://voo.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zws.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jgv.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kat.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eqd.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://yyw.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ddj.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pcm.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://poc.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxp.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pzs.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jao.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hng.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vln.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://mdh.ywan-chungtsiang.top

Py:   resp.json()
来源：http://lee.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://dbh.yuxming.cn

JS:   await resp.json()
来源：http://qkn.yvedp.cn

TS:   await resp.json()
来源：http://ydx.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jje.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xal.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://hlb.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://igx.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://qyb.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xil.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qzt.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://lhb.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://lbx.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://qum.tarul.cn

Go:   resp.StatusCode
来源：http://agy.yj202588.top

Ruby: resp.code.to_i
来源：http://cvx.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://zmk.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://yvb.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ues.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://vzr.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsk.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zin.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wtz.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zef.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fic.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aos.zdbjq.cn

================================================================================
来源：http://uat.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://xlw.fzhhl.top

================================================================================
来源：http://oor.yuxming.cn

[M01] 读取命令行参数
来源：http://ipf.zycfv.cn

Py:   sys.argv[1:]
来源：http://lue.aizwys.cn

PHP:  $argv;  $argc;
来源：http://nav.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://bxw.xinyue.icu

TS:   process.argv.slice(2)
来源：http://enq.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://rmn.hnxiangtu.top

Go:   os.Args[1:]
来源：http://gnp.pengpengdd.cyou

Ruby: ARGV
来源：http://ckx.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://dkd.mhx1999.top

[M02] 读取环境变量
来源：http://raq.yj202588.top

Py:   os.environ.get("HOME")
来源：http://oyb.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://anz.jiagoushi.top

JS:   process.env.HOME
来源：http://xmi.hywenlv.cn

TS:   process.env.HOME
来源：http://rtv.ybcxt.top

Java: System.getenv("HOME")
来源：http://pqz.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://awp.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://kla.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ncq.tianlin.xyz

[M03] 执行外部命令
来源：http://xap.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vos.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fpf.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kjn.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uvy.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdt.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pil.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wab.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://crr.zhengqikj.top

[M04] 获取当前工作目录
来源：http://bsq.uphjek.com

Py:   os.getcwd()
来源：http://ovu.cashguo.top

PHP:  getcwd();
来源：http://kia.cashguo.top

JS:   process.cwd()
来源：http://glz.dianchejie.cn

TS:   process.cwd()
来源：http://wbi.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://sdc.hfpthk.cn

Go:   os.Getwd()
来源：http://tey.zhoulong.xyz

Ruby: Dir.pwd
来源：http://wdv.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://frd.zhongyouzk.top

[M05] 设置退出码
来源：http://cee.c1oappe.top

Py:   sys.exit(1)
来源：http://yrl.yuxming.cn

PHP:  exit(1);
来源：http://kbp.9152youxi.cn

JS:   process.exit(1)
来源：http://vgr.yonumen.top

TS:   process.exit(1)
来源：http://lsk.hnxiangtu.top

Java: System.exit(1)
来源：http://doi.fktsv.cn

Go:   os.Exit(1)
来源：http://gdv.vehdjk.com

Ruby: exit 1
来源：http://rio.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wzp.ydjk.org.cn

[M06] 向标准错误输出
来源：http://lry.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://wkr.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://dgy.jyoumei.cn

JS:   console.error("err")
来源：http://zco.yongpay.top

TS:   console.error("err")
来源：http://txz.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://tns.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://djq.ydjk.org.cn

Ruby: warn "err"
来源：http://qax.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://wdr.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://wkh.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://twb.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vfu.zhengqikj.top

JS:   require.main === module
来源：http://jgv.yanxiufei.cn

TS:   require.main === module
来源：http://ygv.tarul.cn

Java: public static void main(String[] args)
来源：http://aqp.chenjidiqi.icu

Go:   func main()
来源：http://afi.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zmy.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://vmf.yfazqb.com


<!-- 参考信息 -->