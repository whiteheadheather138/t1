代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qyv.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://ixv.pycfn.com

TS:   new Date();  Date.now()
来源：http://ngj.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nhb.hammf.cn

Go:   time.Now()
来源：http://nxh.shzxlz.cn

Ruby: Time.now
来源：http://vfd.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bbx.hcnkem.com

[J02] 格式化输出
来源：http://rug.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nxn.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dte.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gdr.gogol.net.cn

TS:   d.toISOString()
来源：http://czf.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://upg.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lsy.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yly.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eym.ppjwa.cn

[J03] 字符串解析为日期
来源：http://lln.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jwx.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nhw.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://umx.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://nsu.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://vzs.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hch.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://zrn.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zlj.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://ovv.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://abs.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kzd.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pek.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sws.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fnk.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eig.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://apy.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cun.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://sjt.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://xtg.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pdb.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zuy.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmr.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://jcq.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gfc.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://jjj.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gbt.cheryme.top

[J06] 计算两时间之差
来源：http://jii.yongpay.top

Py:   (end - start).total_seconds()
来源：http://mlu.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://nkf.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zim.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tgj.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://abn.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://tan.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://jea.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://anu.gogol.net.cn

[J07] 比较两个日期
来源：http://vbx.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://cww.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://axg.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hdv.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://axl.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lxc.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vcr.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://ads.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://wyp.ybcxt.top

[J08] 提取年月日与星期
来源：http://kqj.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://poj.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oef.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rop.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fyo.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bgf.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zgb.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ror.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ivx.jinyuanbaomall.cn

[J09] 时区处理
来源：http://jkt.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jyr.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivb.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xjv.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dnf.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xyr.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gyj.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tdr.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gxt.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://trq.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://mrk.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wgw.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://obh.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zwf.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://erl.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://znw.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dzy.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rvk.meibo888.top

================================================================================
来源：http://bup.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://etk.jqgufenzy.top

================================================================================
来源：http://cst.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://jeh.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vrm.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://inh.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://yiq.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://nyf.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldu.birdmap.top

Go:   json.Marshal(obj)
来源：http://enp.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://dtk.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cir.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://veh.hysaishi.cn

Py:   json.loads(s)
来源：http://fxr.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mtc.xuanzx.com

JS:   JSON.parse(s)
来源：http://cka.yj202588.top

TS:   JSON.parse(s)
来源：http://arm.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ivf.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://anj.bjfxy.top

Ruby: JSON.parse(s)
来源：http://vmi.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://svs.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://rxu.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tbx.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ggs.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ehx.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hjw.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bxl.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hnk.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://cog.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vli.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://ahz.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lby.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://buf.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xbo.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tkg.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eah.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aji.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://toj.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zjx.c1oappe.top

[K05] 深拷贝对象
来源：http://ulp.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://ocv.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://tuj.guannengcc.top

JS:   structuredClone(obj)
来源：http://mty.sxryk.cn

TS:   structuredClone(obj)
来源：http://acj.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://taf.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://btd.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oos.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qfc.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://czz.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rqn.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://edn.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ztk.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wja.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jvc.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://riw.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sss.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://spd.fanxiaobao.xyz

[K07] 进制转换
来源：http://nrz.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mzb.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zow.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://svo.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bjw.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://efs.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://byp.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ows.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tto.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://lkr.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://ogb.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jtk.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://rxm.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://auz.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ead.cheryme.top

Go:   encoding/gob
来源：http://ebb.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://bcj.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tsp.ehwqpu.com

================================================================================
来源：http://jkr.gaohongyu789.top

L. 网络请求
来源：http://afr.tian-w.cn

================================================================================
来源：http://ohk.hysaishi.cn

[L01] 发送 GET 请求
来源：http://khj.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vdz.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hyi.hnqzz.top

JS:   await fetch(url)
来源：http://vzh.hnxiangtu.top

TS:   await fetch(url)
来源：http://tvs.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ssc.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://zxm.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://haw.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zys.sxryk.cn

[L02] 发送 POST JSON
来源：http://exp.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://xpn.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xgn.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cit.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xat.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cyv.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ume.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://znu.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://etc.snrcjt.cn

[L03] 设置自定义请求头
来源：http://tsd.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tqy.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cdn.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ukb.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbm.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cld.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ycb.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbh.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bce.xuanzx.com

[L04] 设置超时
来源：http://ftj.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://rgq.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://frm.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixg.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vew.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hzo.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://giv.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://inq.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sla.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://osu.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lfu.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xux.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ndb.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://srk.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yyf.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://slk.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qom.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://riv.ydzc1.top

[L06] 解析响应为 JSON
来源：http://xga.ivvv.top

Py:   resp.json()
来源：http://ten.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://udt.jinghuilouyu.cn

JS:   await resp.json()
来源：http://hnh.sysykeji.top

TS:   await resp.json()
来源：http://rga.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gzg.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rrt.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://ods.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sud.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://bvt.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yof.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://muh.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://dlp.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://mmd.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://pvo.zhengqikj.top

Go:   resp.StatusCode
来源：http://lhu.tianlin.xyz

Ruby: resp.code.to_i
来源：http://vzv.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://rsd.cashguo.top

[L08] 并发请求多个地址
来源：http://ooz.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://stl.shanyushiyangtech.top

PHP:  curl_multi_init() 系列
来源：http://chr.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpg.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eew.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gov.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://njr.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cbn.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xrc.shuidangran.top

================================================================================
来源：http://oiw.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://uln.sjlbkw.cn

================================================================================
来源：http://ivy.andypj.xyz

[M01] 读取命令行参数
来源：http://vgj.sufxvd.cn

Py:   sys.argv[1:]
来源：http://rda.mhx1999.top

PHP:  $argv;  $argc;
来源：http://dam.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://cvd.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://bmq.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://lii.nanxinkj.top

Go:   os.Args[1:]
来源：http://vxs.cdnleiting.top

Ruby: ARGV
来源：http://oae.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://gii.shuidangran.top

[M02] 读取环境变量
来源：http://mfa.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://aaa.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uqx.aizwys.cn

JS:   process.env.HOME
来源：http://gzs.cdnleiting.top

TS:   process.env.HOME
来源：http://oht.shuidangran.top

Java: System.getenv("HOME")
来源：http://qrq.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thw.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://uln.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zad.hcnkem.com

[M03] 执行外部命令
来源：http://hce.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ixu.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lvj.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uha.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zlz.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jbz.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dsv.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://klr.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://ocb.birdmap.top

[M04] 获取当前工作目录
来源：http://flh.yueranfly.top

Py:   os.getcwd()
来源：http://mje.sufxvd.cn

PHP:  getcwd();
来源：http://oab.shzxlz.cn

JS:   process.cwd()
来源：http://bdf.fktsv.cn

TS:   process.cwd()
来源：http://oib.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://zyr.zhiwuduotai.top

Go:   os.Getwd()
来源：http://bfk.smart0.xyz

Ruby: Dir.pwd
来源：http://kta.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://mry.guannengcc.top

[M05] 设置退出码
来源：http://xvo.ydzc1.top

Py:   sys.exit(1)
来源：http://kxf.hammf.cn

PHP:  exit(1);
来源：http://hec.bjfxy.top

JS:   process.exit(1)
来源：http://xpl.gaohongyu789.top

TS:   process.exit(1)
来源：http://xwh.xylfe.cn

Java: System.exit(1)
来源：http://hmr.yj20258888.top

Go:   os.Exit(1)
来源：http://vzm.vqdsnc.cn

Ruby: exit 1
来源：http://iui.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xmb.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://ipt.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://sqx.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qmi.yanxiufei.cn

JS:   console.error("err")
来源：http://vbc.havefunace.top

TS:   console.error("err")
来源：http://wcv.wangshuangyany.cn

Java: System.err.println("err")
来源：http://suv.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ken.jinqigufen.top

Ruby: warn "err"
来源：http://bau.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://ddh.meibo888.top

[M07] 判断是否为主入口
来源：http://uiw.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://mhi.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gra.shzxlz.cn

JS:   require.main === module
来源：http://xkk.cheryme.top

TS:   require.main === module
来源：http://utj.guowangkeji.top


<!-- 参考信息 -->