代发 wailian999

Go:   time.Now()
来源：http://kuu.tarul.cn

Ruby: Time.now
来源：http://txh.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nzc.jqgfzy.top

[J02] 格式化输出
来源：http://ltv.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqa.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xzr.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oju.jqgufenzy.top

TS:   d.toISOString()
来源：http://wwf.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tzf.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lfv.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tpw.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eje.chenzaomai.com

[J03] 字符串解析为日期
来源：http://khs.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hso.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ego.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://feq.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://azk.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://xoe.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zqm.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://thn.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://igm.andypj.xyz

[J04] 时间戳与日期互转
来源：http://eel.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pfk.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wnc.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qty.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dlx.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gsb.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://faq.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://euu.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ulz.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://avf.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://jwn.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tch.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bwz.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://znu.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://nzn.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qdi.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://dzn.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://yyb.yonumen.top

[J06] 计算两时间之差
来源：http://frb.tanke756.top

Py:   (end - start).total_seconds()
来源：http://pda.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://tma.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vhz.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rur.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://cqm.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://cxg.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://fuq.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://ggq.fzhhl.top

[J07] 比较两个日期
来源：http://btb.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://oej.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://slj.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uve.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://xvs.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://noc.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nnq.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zps.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://fao.haohaochexian.top

[J08] 提取年月日与星期
来源：http://haj.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qxw.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jku.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zoh.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rri.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xey.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://asp.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rwt.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pre.gotoacloud.top

[J09] 时区处理
来源：http://wbj.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://irz.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jah.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yei.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axi.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gos.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wmp.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://drn.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yaw.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://yhg.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yal.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhg.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bbm.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ggg.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dvc.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rdd.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kji.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://njp.yvedp.cn

================================================================================
来源：http://unp.fktsv.cn

K. JSON 与序列化
来源：http://qgb.ybcxt.top

================================================================================
来源：http://con.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://ghp.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ria.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lgk.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://wui.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://qdq.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://etw.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://mah.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://gcm.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ybf.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://bue.cashguo.top

Py:   json.loads(s)
来源：http://icp.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mpo.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://mdb.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://qkb.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hzi.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ngh.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://lub.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pml.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://xjs.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bpp.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rmc.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ixt.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gpp.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gpg.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ewr.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vki.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qzw.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://xii.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fwz.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vbe.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whz.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eui.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kiv.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hvj.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://exc.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://prh.xuanzx.com

[K05] 深拷贝对象
来源：http://pht.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://zrv.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://txz.gogol.net.cn

JS:   structuredClone(obj)
来源：http://hlv.uphjek.com

TS:   structuredClone(obj)
来源：http://wry.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qyt.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eyu.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mij.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kam.52xcode.cn

[K06] 解析 URL 查询串
来源：http://aat.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xyy.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://crx.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vnv.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hln.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://myf.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xfr.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lrq.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iri.jinqigufen.top

[K07] 进制转换
来源：http://dcg.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://apt.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ddn.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kkm.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ecj.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yxj.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ldi.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uyo.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rrc.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://gmg.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://rmq.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pbg.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://zfg.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://del.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nfk.aizwys.cn

Go:   encoding/gob
来源：http://dmu.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://ead.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dga.hysaishi.cn

================================================================================
来源：http://idb.gogol.net.cn

L. 网络请求
来源：http://zpq.nwbrower.top

================================================================================
来源：http://cka.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://dnf.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bch.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tkf.cashguo.top

JS:   await fetch(url)
来源：http://tfl.shangyingyoupin.top

TS:   await fetch(url)
来源：http://wka.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uzf.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://bvr.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vli.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xhj.tarul.cn

[L02] 发送 POST JSON
来源：http://dgi.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://sgi.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aws.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yzt.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbw.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ffl.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ijk.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qss.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hyq.dianchejie.cn

[L03] 设置自定义请求头
来源：http://mqk.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gmn.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://opq.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://clq.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyw.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://peu.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ena.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oip.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oax.sweek.top

[L04] 设置超时
来源：http://giq.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://hgn.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://beg.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uyb.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uev.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ioe.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://can.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bfx.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xwp.tarul.cn

[L05] 上传文件（multipart）
来源：http://rwv.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wan.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yug.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hvh.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cgv.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kge.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gmm.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ura.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fzt.nwbrower.top

[L06] 解析响应为 JSON
来源：http://ksb.xuetiantiany.cn

Py:   resp.json()
来源：http://jyf.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://ixw.jqgfzy.top

JS:   await resp.json()
来源：http://knh.zhoulong.xyz

TS:   await resp.json()
来源：http://aky.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vlh.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bfp.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://rud.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yko.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://hup.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kqs.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://egw.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://ady.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://low.yj202588.top

Java: resp.statusCode()
来源：http://biw.jlsjyb.cn

Go:   resp.StatusCode
来源：http://ojr.sxryk.cn

Ruby: resp.code.to_i
来源：http://yis.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://moh.hcnkem.com

[L08] 并发请求多个地址
来源：http://ppb.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://elx.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://tfe.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ypf.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://law.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bvm.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xve.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nym.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bnc.guannengcc.top

================================================================================
来源：http://ond.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://mix.tian-w.cn

================================================================================
来源：http://dqe.havefunace.top

[M01] 读取命令行参数
来源：http://kxl.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://jbv.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://rvo.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://rxz.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://dxl.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://eed.gotoacloud.top

Go:   os.Args[1:]
来源：http://lmq.jinqigfzy.top

Ruby: ARGV
来源：http://zsa.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://uay.yj202588.top

[M02] 读取环境变量
来源：http://zhi.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://sjn.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qzp.xylfe.cn

JS:   process.env.HOME
来源：http://hmc.hnqzz.top

TS:   process.env.HOME
来源：http://mxp.smart0.xyz

Java: System.getenv("HOME")
来源：http://nwd.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://slj.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://qvo.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://urb.hongshengwenyu.top

[M03] 执行外部命令
来源：http://bve.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://skw.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pli.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lrx.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ltg.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pop.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mik.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://azb.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://lqb.cdnleiting.top

[M04] 获取当前工作目录
来源：http://czm.kuanghao11.cn

Py:   os.getcwd()
来源：http://lql.tian-w.cn

PHP:  getcwd();
来源：http://gux.jlsjyb.cn

JS:   process.cwd()
来源：http://wbz.svipenyu.cn

TS:   process.cwd()
来源：http://eze.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://mke.hnxiangtu.top

Go:   os.Getwd()
来源：http://urb.zycfv.cn

Ruby: Dir.pwd
来源：http://rkp.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://yrc.cdnleiting.top

[M05] 设置退出码
来源：http://bex.chenzaomai.com

Py:   sys.exit(1)
来源：http://myj.uphjek.com

PHP:  exit(1);
来源：http://tmr.jianghu66.top

JS:   process.exit(1)
来源：http://nbv.zhoulong.xyz

TS:   process.exit(1)
来源：http://zwi.redwolf501.top

Java: System.exit(1)
来源：http://cyt.xuanzx.com

Go:   os.Exit(1)
来源：http://ssu.ctjpmb.com

Ruby: exit 1
来源：http://fkj.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hcf.52xcode.cn

[M06] 向标准错误输出
来源：http://yzm.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://oqh.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wvg.uphjek.com

JS:   console.error("err")
来源：http://hmt.iojbl.cn

TS:   console.error("err")
来源：http://ggi.aibaodan.cn

Java: System.err.println("err")
来源：http://emf.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ycu.jinqigfzy.top

Ruby: warn "err"
来源：http://tzp.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://sit.mhx1999.top

[M07] 判断是否为主入口
来源：http://zgz.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://xmf.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xre.hammf.cn

JS:   require.main === module
来源：http://gwd.daxiang520.top

TS:   require.main === module
来源：http://mgl.ydzc1.top

Java: public static void main(String[] args)
来源：http://tcn.shangyingyoupin.top

Go:   func main()
来源：http://zxy.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wle.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://ema.zhaomingkeji.xyz


<!-- 参考信息 -->