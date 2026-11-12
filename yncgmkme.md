代发 wailian999

Go:   time.Now()
来源：http://ebf.redwolf501.top

Ruby: Time.now
来源：http://kht.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://udl.ctjpmb.com

[J02] 格式化输出
来源：http://spy.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wbj.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sgm.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ghu.yanxiufei.cn

TS:   d.toISOString()
来源：http://lqg.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ohc.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hok.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bdu.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iuq.hysaishi.cn

[J03] 字符串解析为日期
来源：http://ycs.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://det.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fqq.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://xsu.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://fuf.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bco.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hbj.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://xrb.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ayy.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://igq.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dxl.gzhubu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://izk.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hut.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wxm.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hzv.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dtt.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hxt.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ruf.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://jyw.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://iis.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://scy.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltx.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kha.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://mbq.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kvd.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://lsy.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dye.kuanghao11.cn

[J06] 计算两时间之差
来源：http://lkb.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://nkk.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://vue.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mtt.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xwm.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://ghi.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://boz.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://rll.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://kwg.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://iam.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://gqz.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pmn.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://nxt.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://frx.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fwd.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vyj.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://sfo.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://nsk.jianghu66.top

[J08] 提取年月日与星期
来源：http://flq.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://klw.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://haz.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ynr.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ptj.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wya.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dvr.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kgj.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://niy.jinqigufen.top

[J09] 时区处理
来源：http://gbr.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qkc.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qki.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xnb.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlo.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fyl.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pvo.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iuz.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zus.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://chp.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://nyk.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nav.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfn.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lbo.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yfh.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hnk.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ysk.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qez.yanxiufei.cn

================================================================================
来源：http://wwo.jqgufenzy.top

K. JSON 与序列化
来源：http://jmh.ybcxt.top

================================================================================
来源：http://ovm.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://wst.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ybg.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hmi.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://nzf.hammf.cn

TS:   JSON.stringify(obj)
来源：http://wjv.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gku.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://qil.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://uef.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sfx.hesvh.cn

[K02] JSON 字符串转对象
来源：http://fas.sysykeji.top

Py:   json.loads(s)
来源：http://gxx.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://egj.snrcjt.cn

JS:   JSON.parse(s)
来源：http://udg.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://rqw.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lws.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://ten.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://bpe.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hfl.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://spu.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://whh.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wug.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dpw.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mnh.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fyd.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lxd.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://csr.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gtf.daria6918.cn

[K04] 读取 JSON 文件
来源：http://jvf.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xwq.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://utu.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://olf.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wij.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qeo.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hyc.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://sqs.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kuu.andypj.xyz

[K05] 深拷贝对象
来源：http://mjc.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://ykp.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://jps.gotoacloud.top

JS:   structuredClone(obj)
来源：http://thy.smart0.xyz

TS:   structuredClone(obj)
来源：http://ghl.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xud.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yzk.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tls.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zmo.yuxming.cn

[K06] 解析 URL 查询串
来源：http://mhi.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qvh.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jte.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyr.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujd.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://clk.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://doh.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wde.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wvc.jinqigufen.top

[K07] 进制转换
来源：http://bzq.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eij.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://clb.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rgs.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ati.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ovo.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gmq.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vuu.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mrk.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://ley.havefunace.top

Py:   pickle.dumps(obj)
来源：http://taj.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cwh.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://ssf.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://cvq.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hqz.shuidangran.top

Go:   encoding/gob
来源：http://xbb.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://cag.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tvr.guannengcc.top

================================================================================
来源：http://xxg.dianchejie.cn

L. 网络请求
来源：http://ieu.quarkkingdee.top

================================================================================
来源：http://wtb.gzhubu.top

[L01] 发送 GET 请求
来源：http://gsd.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nvp.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wbh.quarkkingdee.top

JS:   await fetch(url)
来源：http://vul.zhiwuduotai.top

TS:   await fetch(url)
来源：http://jwk.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://new.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://iuh.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tiv.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://frj.zhengqikj.top

[L02] 发送 POST JSON
来源：http://xyb.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://kkt.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lhe.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qdk.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cen.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tls.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sce.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://clm.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vsw.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://lgl.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://irm.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yhj.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uci.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nte.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://weh.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://few.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dra.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://juc.zhoulong.xyz

[L04] 设置超时
来源：http://nle.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://fgt.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dsy.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://shd.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://apx.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ylo.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lak.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cip.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zsq.bjfxy.top

[L05] 上传文件（multipart）
来源：http://hfn.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tqh.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vpa.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gtm.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fnb.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://une.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jel.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uhj.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bck.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://npa.xuanzx.com

Py:   resp.json()
来源：http://kjh.tarul.cn

PHP:  json_decode($body, true);
来源：http://uob.gotoacloud.top

JS:   await resp.json()
来源：http://koq.chenlongwang.top

TS:   await resp.json()
来源：http://jfa.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ygj.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yws.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://prt.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pap.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://iul.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qwz.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://agh.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://aeq.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://pjm.ehwqpu.com

Java: resp.statusCode()
来源：http://lrk.vqdsnc.cn

Go:   resp.StatusCode
来源：http://msq.xuanzx.com

Ruby: resp.code.to_i
来源：http://hgc.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://czi.316326.xyz

[L08] 并发请求多个地址
来源：http://xms.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zyt.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://cnq.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xlr.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tlw.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pqf.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nqw.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wmd.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ihj.yuxming.cn

================================================================================
来源：http://sba.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://dlt.pycfn.com

================================================================================
来源：http://cwg.daxiang520.top

[M01] 读取命令行参数
来源：http://ocq.daria6918.cn

Py:   sys.argv[1:]
来源：http://kec.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://mle.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://oqi.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://ecy.meibo888.top

Java: args 数组（main 方法参数）
来源：http://uvi.havefunace.top

Go:   os.Args[1:]
来源：http://bce.yongpay.top

Ruby: ARGV
来源：http://ubp.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://exv.zhixingplan.top

[M02] 读取环境变量
来源：http://qbs.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://qoo.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ayw.bjfxy.top

JS:   process.env.HOME
来源：http://pqt.shangyingyoupin.top

TS:   process.env.HOME
来源：http://mnl.ivvv.top

Java: System.getenv("HOME")
来源：http://kdp.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nmd.zhaomingkeji.xyz

Ruby: ENV["HOME"]
来源：http://yji.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ppe.xuanzx.com

[M03] 执行外部命令
来源：http://ttv.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tvt.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mzu.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gtj.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hpb.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bca.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ajt.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yju.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://pod.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://ffc.sysykeji.top

Py:   os.getcwd()
来源：http://wng.shuidangran.top

PHP:  getcwd();
来源：http://ctv.yfazqb.com

JS:   process.cwd()
来源：http://jro.nanxinkj.top

TS:   process.cwd()
来源：http://eky.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://zcr.dianchejie.cn

Go:   os.Getwd()
来源：http://kuz.9152youxi.cn

Ruby: Dir.pwd
来源：http://tez.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iia.yongpay.top

[M05] 设置退出码
来源：http://gmx.tanke756.top

Py:   sys.exit(1)
来源：http://vze.yj20258.top

PHP:  exit(1);
来源：http://pps.ybcxt.top

JS:   process.exit(1)
来源：http://qwx.vehdjk.com

TS:   process.exit(1)
来源：http://zzo.guannengcc.top

Java: System.exit(1)
来源：http://oly.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://yoq.hfpthk.cn

Ruby: exit 1
来源：http://lpd.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nxp.fzhhl.top

[M06] 向标准错误输出
来源：http://lug.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://wgp.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qcb.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://xhw.316326.xyz

TS:   console.error("err")
来源：http://gfs.hywenlv.cn

Java: System.err.println("err")
来源：http://jju.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://whl.hnxiangtu.top

Ruby: warn "err"
来源：http://mpf.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://xtz.ppjwa.cn

[M07] 判断是否为主入口
来源：http://cwf.yonumen.top

Py:   if __name__ == "__main__":
来源：http://xqa.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://omw.guowangkeji.top

JS:   require.main === module
来源：http://oal.hesvh.cn

TS:   require.main === module
来源：http://tgr.yvedp.cn

Java: public static void main(String[] args)
来源：http://ews.svipenyu.cn

Go:   func main()
来源：http://lnd.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gid.yuxming.cn

C#:   static void Main(string[] args)
来源：http://avu.xylfe.cn


<!-- 参考信息 -->