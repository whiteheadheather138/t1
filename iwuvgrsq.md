代发 wailian999

Go:   time.Now()
来源：http://cla.vehdjk.com

Ruby: Time.now
来源：http://xrw.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vqv.smart0.xyz

[J02] 格式化输出
来源：http://nnw.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbn.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qpf.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vwz.jqgfzy.top

TS:   d.toISOString()
来源：http://qxh.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xjn.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xso.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qea.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qom.redwolf501.top

[J03] 字符串解析为日期
来源：http://smj.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kzv.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hrz.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://mds.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://fdg.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://bjy.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jvh.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://wni.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://khx.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://dns.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yjy.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hsa.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xge.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://cwx.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ucl.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jtd.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aim.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mil.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://hmi.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://mvr.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ztd.yfazqb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://byq.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://amz.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://ysj.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hgl.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://qvf.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qec.snrcjt.cn

[J06] 计算两时间之差
来源：http://ldu.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://zcd.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://qwd.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tlb.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pas.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gff.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://wsz.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://tkn.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://azx.kuanghao11.cn

[J07] 比较两个日期
来源：http://cqc.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://gur.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hgm.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://rfd.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://omj.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ygf.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qlv.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ibb.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://iyv.guowangkeji.top

[J08] 提取年月日与星期
来源：http://rko.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ldf.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gct.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dbo.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rth.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nsj.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://waz.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jdm.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sqr.havefunace.top

[J09] 时区处理
来源：http://fwa.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jab.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhk.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://voq.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yyg.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qho.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kop.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pix.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uub.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://qwh.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fby.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://que.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pri.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xpa.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ngy.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eix.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wfb.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://chf.birdmap.top

================================================================================
来源：http://vaf.andypj.xyz

K. JSON 与序列化
来源：http://bvn.yfazqb.com

================================================================================
来源：http://rmc.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://frb.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ttr.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lph.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://lfz.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://mok.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tcw.sweek.top

Go:   json.Marshal(obj)
来源：http://wiz.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://eqy.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nry.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://hoh.iojbl.cn

Py:   json.loads(s)
来源：http://duy.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ucb.c1oappe.top

JS:   JSON.parse(s)
来源：http://dfo.cqqwz.cn

TS:   JSON.parse(s)
来源：http://hud.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://amt.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://exq.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://niw.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rhy.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://dsl.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tja.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://juc.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hun.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://uxt.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ijk.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kfm.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://zoh.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uyw.nwbrower.top

[K04] 读取 JSON 文件
来源：http://fgl.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cvc.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vag.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wgl.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijn.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://igi.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hfn.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://jnw.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hvf.fktsv.cn

[K05] 深拷贝对象
来源：http://dri.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://tgl.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://iji.mhx1999.top

JS:   structuredClone(obj)
来源：http://chj.tian-w.cn

TS:   structuredClone(obj)
来源：http://bsu.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nld.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://atq.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ixe.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ppu.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://xtu.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uxe.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mzu.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gfs.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lax.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://emz.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjz.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hun.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kdq.epnwcf.com

[K07] 进制转换
来源：http://kui.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nlj.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rxr.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qah.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jcs.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cgw.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hpp.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jwn.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://smo.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://ega.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://fov.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ovw.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://jde.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://xms.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jri.9152youxi.cn

Go:   encoding/gob
来源：http://vyu.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://rek.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rmq.ydjk.org.cn

================================================================================
来源：http://abu.jqgufenzy.top

L. 网络请求
来源：http://uzs.xuetiantiany.cn

================================================================================
来源：http://hdo.svipenyu.cn

[L01] 发送 GET 请求
来源：http://soc.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lpi.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pwn.hywenlv.cn

JS:   await fetch(url)
来源：http://eoc.wangshuangyany.cn

TS:   await fetch(url)
来源：http://vbn.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qyz.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://qug.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cfh.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iid.hfpthk.cn

[L02] 发送 POST JSON
来源：http://xui.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://zly.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qub.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wts.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axv.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dyi.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gjj.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jeh.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rzn.gogol.net.cn

[L03] 设置自定义请求头
来源：http://omq.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jwv.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://clg.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gch.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mye.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://akh.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rou.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zhl.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hzg.tianlin.xyz

[L04] 设置超时
来源：http://rfp.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://cnh.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zgr.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zag.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgc.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tpm.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bpc.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dgf.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yxg.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://aby.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ged.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wfh.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gro.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fmz.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dxr.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gzx.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hec.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bju.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://bgi.yangfankeji.com

Py:   resp.json()
来源：http://mga.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://nnq.zhongyouzk.top

JS:   await resp.json()
来源：http://kdt.yj20258888.top

TS:   await resp.json()
来源：http://cna.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lyh.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bet.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://azy.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ayp.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://cdr.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ljh.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xrk.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://fgw.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://tna.andypj.xyz

Java: resp.statusCode()
来源：http://lts.fktsv.cn

Go:   resp.StatusCode
来源：http://jjt.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://kct.uphjek.com

C#:   (int)resp.StatusCode
来源：http://hle.havefunace.top

[L08] 并发请求多个地址
来源：http://jzh.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mcl.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://esp.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aym.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eyh.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aje.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mfp.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nkp.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qoa.hysaishi.cn

================================================================================
来源：http://ajo.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://zna.ivvv.top

================================================================================
来源：http://tdy.zdqjudy.top

[M01] 读取命令行参数
来源：http://hpd.vehdjk.com

Py:   sys.argv[1:]
来源：http://xzp.ybcxt.top

PHP:  $argv;  $argc;
来源：http://blg.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://elp.yuxming.cn

TS:   process.argv.slice(2)
来源：http://sws.birdmap.top

Java: args 数组（main 方法参数）
来源：http://enc.sufxvd.cn

Go:   os.Args[1:]
来源：http://lly.tianlin.xyz

Ruby: ARGV
来源：http://ljm.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://gxr.gzhubu.top

[M02] 读取环境变量
来源：http://wzb.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://bqy.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zbi.tian-w.cn

JS:   process.env.HOME
来源：http://dqh.zdbjq.cn

TS:   process.env.HOME
来源：http://xny.shzxlz.cn

Java: System.getenv("HOME")
来源：http://uel.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hpd.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://gwd.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rcl.sysykeji.top

[M03] 执行外部命令
来源：http://srd.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kiu.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wee.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ewo.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://spr.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mdt.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fca.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://jqa.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://zuk.52xcode.cn

[M04] 获取当前工作目录
来源：http://enx.hongshengwenyu.top

Py:   os.getcwd()
来源：http://bhi.wangshuangyany.cn

PHP:  getcwd();
来源：http://azx.gotoacloud.top

JS:   process.cwd()
来源：http://vtq.daxiang520.top

TS:   process.cwd()
来源：http://lht.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://jri.yj20258888.top

Go:   os.Getwd()
来源：http://qsz.xziqi.cn

Ruby: Dir.pwd
来源：http://kim.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kyn.uphjek.com

[M05] 设置退出码
来源：http://nre.pycfn.com

Py:   sys.exit(1)
来源：http://hxb.tianlin.xyz

PHP:  exit(1);
来源：http://wgm.hnqzz.top

JS:   process.exit(1)
来源：http://coc.tian-w.cn

TS:   process.exit(1)
来源：http://rfs.xuanzx.com

Java: System.exit(1)
来源：http://rkr.zhixingplan.top

Go:   os.Exit(1)
来源：http://epm.cdnleiting.top

Ruby: exit 1
来源：http://ulw.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hgs.jqgfzy.top

[M06] 向标准错误输出
来源：http://ykz.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://mfo.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dwv.jqgfzy.top

JS:   console.error("err")
来源：http://njg.hnxiangtu.top

TS:   console.error("err")
来源：http://bxa.tanke756.top

Java: System.err.println("err")
来源：http://uoo.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uio.xziqi.cn

Ruby: warn "err"
来源：http://bhx.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://yus.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://eos.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://etb.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hbv.gotoacloud.top

JS:   require.main === module
来源：http://fjw.daxiang520.top

TS:   require.main === module
来源：http://ogg.xziqi.cn

Java: public static void main(String[] args)
来源：http://nsf.wangshuangyany.cn

Go:   func main()
来源：http://ojs.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wil.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://yzd.yfazqb.com


<!-- 参考信息 -->