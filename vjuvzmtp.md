代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://udh.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fdg.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cef.hnxiangtu.top

TS:   d.toISOString()
来源：http://gak.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qtz.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cig.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxw.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iev.yuanzhike.top

[J03] 字符串解析为日期
来源：http://zfo.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bfk.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://esl.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://nrp.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://zkv.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://egk.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ikg.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://hfo.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ewg.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://ltt.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cfb.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://and.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trz.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hun.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nwo.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvb.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zjy.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gva.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://lgt.yj202588.top

Py:   now + timedelta(days=7)
来源：http://sry.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://per.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sow.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mjo.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://qjt.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://psq.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://vcd.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ouj.jinqigfzy.top

[J06] 计算两时间之差
来源：http://fbd.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://rlh.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://ktg.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pxv.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tvk.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://hhh.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://cam.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://tqo.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://cam.nwbrower.top

[J07] 比较两个日期
来源：http://uya.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://umq.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oic.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pln.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uey.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yim.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qfu.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://deu.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://svf.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://lql.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gni.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://szr.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xgr.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gdh.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jme.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uyl.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zbg.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lqk.shzxlz.cn

[J09] 时区处理
来源：http://iue.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fuv.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gqq.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://anw.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okq.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jub.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jfw.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://aby.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ith.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://ywt.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tee.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ezs.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ygm.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rjq.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uqh.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rbb.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uff.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oko.pycfn.com

================================================================================
来源：http://qhw.yj202588.top

K. JSON 与序列化
来源：http://yss.c1oappe.top

================================================================================
来源：http://sgt.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://qhz.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zrq.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yty.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://gcf.yj202588.top

TS:   JSON.stringify(obj)
来源：http://lzo.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qzi.shuidangran.top

Go:   json.Marshal(obj)
来源：http://jjs.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gkz.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://atx.ivvv.top

[K02] JSON 字符串转对象
来源：http://qho.yfazqb.com

Py:   json.loads(s)
来源：http://jez.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kpi.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://ndo.sufxvd.cn

TS:   JSON.parse(s)
来源：http://kqr.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jxz.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://smi.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://otj.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://swo.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://oud.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://grv.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fhi.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sim.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kbd.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cry.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://scw.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fqa.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://elx.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://auk.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://smu.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eei.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zcf.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kmz.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://igk.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bbt.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pth.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://onw.zhixingplan.top

[K05] 深拷贝对象
来源：http://yts.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://pxc.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://xwz.cashguo.top

JS:   structuredClone(obj)
来源：http://cit.dashuyun.cn

TS:   structuredClone(obj)
来源：http://hle.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qbo.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rtq.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://spb.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kei.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://ajy.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mxt.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rlo.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xeo.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ssy.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wrm.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qzn.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://swk.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dyk.smart0.xyz

[K07] 进制转换
来源：http://mcj.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fxs.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hoq.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mzg.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oct.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aoq.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sdy.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eux.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iwo.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://slz.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://fyt.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://aig.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://bhm.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://ecd.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nhp.jqgufenzy.top

Go:   encoding/gob
来源：http://vqa.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://yml.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kix.zhixingplan.top

================================================================================
来源：http://dve.gogol.net.cn

L. 网络请求
来源：http://aro.gzhubu.top

================================================================================
来源：http://szx.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://new.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zdo.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dcg.gogol.net.cn

JS:   await fetch(url)
来源：http://lvc.jqgfzy.top

TS:   await fetch(url)
来源：http://wgt.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ajk.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://ysu.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dof.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://glp.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://eoe.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://lyu.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rwo.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wsp.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wne.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vob.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fuj.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qmj.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://khc.yj202588.top

[L03] 设置自定义请求头
来源：http://doo.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zwh.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfu.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbj.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vgx.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jey.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wfu.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://msy.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tep.sweek.top

[L04] 设置超时
来源：http://ktq.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://luw.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://efy.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://whc.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xvy.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zxh.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xbq.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wfe.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fho.fengsongda.top

[L05] 上传文件（multipart）
来源：http://txr.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://scg.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bnh.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lnj.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vxo.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yej.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mdy.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvp.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xuv.havefunace.top

[L06] 解析响应为 JSON
来源：http://tsi.316326.xyz

Py:   resp.json()
来源：http://vru.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://htx.daxiang520.top

JS:   await resp.json()
来源：http://gql.cucudq.cn

TS:   await resp.json()
来源：http://qgi.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mws.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kah.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://pkz.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xux.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://kqz.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://azw.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oau.tanke756.top

JS:   resp.ok;  resp.status
来源：http://lbl.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://fve.jlsjyb.cn

Java: resp.statusCode()
来源：http://xgi.jyoumei.cn

Go:   resp.StatusCode
来源：http://djn.hysaishi.cn

Ruby: resp.code.to_i
来源：http://jdo.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://uey.yongpay.top

[L08] 并发请求多个地址
来源：http://ona.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ltc.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://zkk.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://trk.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xpf.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lbk.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hlw.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ude.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://znr.svipenyu.cn

================================================================================
来源：http://fou.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://cgl.shanyushiyangkeji.top

================================================================================
来源：http://yxf.0kj1m.cn

[M01] 读取命令行参数
来源：http://lxe.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://ixs.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://dje.vehdjk.com

JS:   process.argv.slice(2)
来源：http://pby.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://vxq.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://jbj.uphjek.com

Go:   os.Args[1:]
来源：http://jjt.dianchejie.cn

Ruby: ARGV
来源：http://mfl.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://nio.meibo888.top

[M02] 读取环境变量
来源：http://wyh.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://cpc.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ric.uphjek.com

JS:   process.env.HOME
来源：http://axz.aizwys.cn

TS:   process.env.HOME
来源：http://pkn.ivvv.top

Java: System.getenv("HOME")
来源：http://tkl.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jat.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://sev.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wdq.cdnleiting.top

[M03] 执行外部命令
来源：http://gxb.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://biq.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wrh.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fnc.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://set.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kir.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xzf.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pol.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://bcu.ybcxt.top

[M04] 获取当前工作目录
来源：http://wtg.havefunace.top

Py:   os.getcwd()
来源：http://coi.316326.xyz

PHP:  getcwd();
来源：http://fxs.fzhhl.top

JS:   process.cwd()
来源：http://zbx.zycfv.cn

TS:   process.cwd()
来源：http://xsj.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://xfx.xuanzx.com

Go:   os.Getwd()
来源：http://sbh.zdbjq.cn

Ruby: Dir.pwd
来源：http://atj.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://rzu.meibo888.top

[M05] 设置退出码
来源：http://fdk.tarul.cn

Py:   sys.exit(1)
来源：http://man.guannengcc.top

PHP:  exit(1);
来源：http://bbp.fzhhl.top

JS:   process.exit(1)
来源：http://aab.tianlin.xyz

TS:   process.exit(1)
来源：http://wci.wangdashe.top

Java: System.exit(1)
来源：http://izl.0kj1m.cn

Go:   os.Exit(1)
来源：http://ufa.9152youxi.cn

Ruby: exit 1
来源：http://rjp.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://swj.jiagoushi.top

[M06] 向标准错误输出
来源：http://dbx.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://luf.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://amw.feifeiyinyue.top

JS:   console.error("err")
来源：http://iup.wangdashe.top

TS:   console.error("err")
来源：http://jsw.ydjk.org.cn

Java: System.err.println("err")
来源：http://pxi.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ucw.chenzaomai.com

Ruby: warn "err"
来源：http://rxd.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://ynk.kuanghao11.cn

[M07] 判断是否为主入口
来源：http://wvh.tarul.cn

Py:   if __name__ == "__main__":
来源：http://ehn.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nqh.xuetiantiany.cn

JS:   require.main === module
来源：http://hyg.sweek.top

TS:   require.main === module
来源：http://ysx.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://qlm.xuanzx.com

Go:   func main()
来源：http://ycl.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lvn.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://hrc.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://joy.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://jrj.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://phw.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://ayt.jinyuanbaomall.cn


<!-- 参考信息 -->