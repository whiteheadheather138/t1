代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vbw.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tgs.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xkl.smart0.xyz

TS:   d.toISOString()
来源：http://cgo.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oly.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aul.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ywa.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lsv.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://ome.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rtz.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kfn.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://nrw.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://wbw.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://hoj.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bqp.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://ldd.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gmr.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://aal.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iis.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wla.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zuu.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tlj.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yip.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wof.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://duk.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tmq.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://dzd.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://xtk.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ldh.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jhd.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzc.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://ecl.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nim.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://vij.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://vuq.yueranfly.top

[J06] 计算两时间之差
来源：http://kcs.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://hnv.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://diu.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lbr.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zhk.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://wma.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://uzm.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://vhm.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://def.hysaishi.cn

[J07] 比较两个日期
来源：http://rhc.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://fek.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://irp.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ktp.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://tim.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qzd.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hhi.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://vus.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://gpm.hnqzz.top

[J08] 提取年月日与星期
来源：http://cwt.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cra.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ctm.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://axp.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hnp.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hyu.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jai.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://urg.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yxy.316326.xyz

[J09] 时区处理
来源：http://wfx.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://srn.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sfw.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ydb.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ikg.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hti.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ypb.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vsb.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iqs.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://dfo.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://gku.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kzs.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qkv.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fhq.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://owd.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cix.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tui.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://daj.zdbjq.cn

================================================================================
来源：http://evy.hysaishi.cn

K. JSON 与序列化
来源：http://jul.yanxiufei.cn

================================================================================
来源：http://wzn.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://fir.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nij.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ndf.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://exm.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://tqy.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ncq.52xcode.cn

Go:   json.Marshal(obj)
来源：http://pzc.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://pfz.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nhh.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://tdo.mhx1999.top

Py:   json.loads(s)
来源：http://idz.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rog.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://sva.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://zbh.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vom.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://zfz.gzhubu.top

Ruby: JSON.parse(s)
来源：http://jra.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uky.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://pfa.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lwl.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vkm.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://ind.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xua.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qnk.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nnz.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://cxd.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cgn.jianghu66.top

[K04] 读取 JSON 文件
来源：http://lyv.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ofe.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kjn.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpd.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tsu.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vzn.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qni.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://klg.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://adb.cqqwz.cn

[K05] 深拷贝对象
来源：http://mck.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://cne.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://jbz.guannengcc.top

JS:   structuredClone(obj)
来源：http://gte.daria6918.cn

TS:   structuredClone(obj)
来源：http://tuu.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://glw.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fhs.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axa.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://typ.hesvh.cn

[K06] 解析 URL 查询串
来源：http://vvf.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ujn.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mhq.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zyx.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ztl.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cob.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yfq.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xkx.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cqv.ctjpmb.com

[K07] 进制转换
来源：http://pno.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nta.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fuc.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uvh.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://llb.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jgn.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vrg.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wgb.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bnv.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://gtt.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://wgc.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://unn.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://dzz.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://plh.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ftc.yangfankeji.com

Go:   encoding/gob
来源：http://hxu.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://cdu.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ozz.fktsv.cn

================================================================================
来源：http://hwg.xuanzx.com

L. 网络请求
来源：http://sex.andypj.xyz

================================================================================
来源：http://ldw.yangfankeji.com

[L01] 发送 GET 请求
来源：http://yxp.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rvk.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vyf.cucudq.cn

JS:   await fetch(url)
来源：http://buk.xziqi.cn

TS:   await fetch(url)
来源：http://jog.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rfo.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://ibp.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ffb.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vdw.hcnkem.com

[L02] 发送 POST JSON
来源：http://yih.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://ooi.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mxn.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ocu.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdm.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://idn.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qkr.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cmy.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hey.jqgfzy.top

[L03] 设置自定义请求头
来源：http://wrl.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zwk.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hvx.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ftj.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dot.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xwf.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jki.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qbp.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kjx.fanxiaobao.xyz

[L04] 设置超时
来源：http://why.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://hcg.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gpl.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tck.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbi.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kdh.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qzy.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvb.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qzy.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://gbu.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mkr.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rqf.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lln.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ros.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wzm.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://reb.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oyn.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cbc.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://yub.daxiang520.top

Py:   resp.json()
来源：http://skq.ydzc1.top

PHP:  json_decode($body, true);
来源：http://zig.c1oappe.top

JS:   await resp.json()
来源：http://svi.zycfv.cn

TS:   await resp.json()
来源：http://dur.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gvs.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fbw.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://pis.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://doz.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://lyi.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dkw.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wbu.sweek.top

JS:   resp.ok;  resp.status
来源：http://xby.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://dwj.gzhubu.top

Java: resp.statusCode()
来源：http://irs.52xcode.cn

Go:   resp.StatusCode
来源：http://byc.daxiang520.top

Ruby: resp.code.to_i
来源：http://qai.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://upy.wangdashe.top

[L08] 并发请求多个地址
来源：http://ipo.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bfd.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://oib.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvm.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zcv.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pnq.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dem.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jgi.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qva.0kj1m.cn

================================================================================
来源：http://qrn.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://uwj.zdqjudy.top

================================================================================
来源：http://zdg.fengsongda.top

[M01] 读取命令行参数
来源：http://nbd.cashguo.top

Py:   sys.argv[1:]
来源：http://nyc.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://typ.iojbl.cn

JS:   process.argv.slice(2)
来源：http://nfh.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://hrb.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://drj.gotoacloud.top

Go:   os.Args[1:]
来源：http://vas.guowangkeji.top

Ruby: ARGV
来源：http://evf.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://tjw.fengsongda.top

[M02] 读取环境变量
来源：http://dwd.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://kpb.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://grd.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://grc.xuetiantiany.cn

TS:   process.env.HOME
来源：http://ozc.svipenyu.cn

Java: System.getenv("HOME")
来源：http://das.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rmw.hcnkem.com

Ruby: ENV["HOME"]
来源：http://dap.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gdt.jianghu66.top

[M03] 执行外部命令
来源：http://zkb.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vdz.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ayp.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qpn.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jtt.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://brs.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ezr.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://nyc.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://fvg.cqqwz.cn

[M04] 获取当前工作目录
来源：http://ezu.daxiang520.top

Py:   os.getcwd()
来源：http://ydl.bjfxy.top

PHP:  getcwd();
来源：http://gwl.aibaodan.cn

JS:   process.cwd()
来源：http://rbe.hammf.cn

TS:   process.cwd()
来源：http://yby.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://guw.hnqzz.top

Go:   os.Getwd()
来源：http://ywp.316326.xyz

Ruby: Dir.pwd
来源：http://lrd.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://owb.mhx1999.top

[M05] 设置退出码
来源：http://gwo.snrcjt.cn

Py:   sys.exit(1)
来源：http://mll.hnqzz.top

PHP:  exit(1);
来源：http://xbr.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://szg.cucudq.cn

TS:   process.exit(1)
来源：http://jkf.nanxinkj.top

Java: System.exit(1)
来源：http://lte.andypj.xyz

Go:   os.Exit(1)
来源：http://gii.ivvv.top

Ruby: exit 1
来源：http://sbb.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mqe.daria6918.cn

[M06] 向标准错误输出
来源：http://osb.hesvh.cn

Py:   print("err", file=sys.stderr)
来源：http://aff.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eqh.0kj1m.cn

JS:   console.error("err")
来源：http://pge.sweek.top

TS:   console.error("err")
来源：http://oxy.wangshuangyany.cn

Java: System.err.println("err")
来源：http://hta.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mof.vqdsnc.cn

Ruby: warn "err"
来源：http://cqt.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://tdh.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://wxc.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://qab.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ink.yvedp.cn

JS:   require.main === module
来源：http://psz.chenzaomai.com

TS:   require.main === module
来源：http://knn.c1oappe.top

Java: public static void main(String[] args)
来源：http://uws.wangdashe.top

Go:   func main()
来源：http://uop.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rzv.daria6918.cn

C#:   static void Main(string[] args)
来源：http://mgc.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://cyv.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://msz.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://ujx.yj202588.top

JS:   process.platform;  process.version
来源：http://uuw.xingfuxueyuan.xyz


<!-- 参考信息 -->