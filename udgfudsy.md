代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tvk.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kga.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgv.fehbvm.com

TS:   d.toISOString()
来源：http://uem.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fvb.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ncj.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eon.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pid.yonumen.top

[J03] 字符串解析为日期
来源：http://cog.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ziv.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://imy.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://aul.hammf.cn

TS:   new Date("2024-01-02")
来源：http://mhh.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://eyf.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mvv.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://otg.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ogl.c1oappe.top

[J04] 时间戳与日期互转
来源：http://oxn.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hqg.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ivi.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zle.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wpb.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vch.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sse.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zkq.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ozh.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://tzk.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://vxs.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ack.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ssr.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aya.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://aot.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dae.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://rkf.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://vua.zhengqikj.top

[J06] 计算两时间之差
来源：http://naw.hammf.cn

Py:   (end - start).total_seconds()
来源：http://tdf.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://ugh.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vyt.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nrf.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vpc.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://isf.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://jwv.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://umy.jiagoushi.top

[J07] 比较两个日期
来源：http://wvz.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ymk.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tsv.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://ndy.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://tci.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://suc.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ikw.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zgv.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://mfu.mhx1999.top

[J08] 提取年月日与星期
来源：http://ngn.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jwb.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://stx.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zdh.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tvr.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tvt.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://emp.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nuy.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vdp.cqqwz.cn

[J09] 时区处理
来源：http://jov.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jng.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jof.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npk.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kfr.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rii.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://crs.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pcy.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xmm.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://bsv.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vgz.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ixd.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tmp.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qhx.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nzi.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pop.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hkj.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tuz.gzhubu.top

================================================================================
来源：http://urt.dianchejie.cn

K. JSON 与序列化
来源：http://cas.yanxiufei.cn

================================================================================
来源：http://ojc.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://qig.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sbk.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bey.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://hkl.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://ift.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uxr.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://noj.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://gqt.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://ylr.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://pwv.xziqi.cn

Py:   json.loads(s)
来源：http://sby.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jba.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://trd.iojbl.cn

TS:   JSON.parse(s)
来源：http://upz.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvf.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ezp.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://weu.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gzv.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://fdv.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aqi.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ntd.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://cvw.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rtp.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rso.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jsq.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://yez.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cwd.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://ofr.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ojh.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iip.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hta.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjl.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tlb.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gwz.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jzh.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zkc.zhengqikj.top

[K05] 深拷贝对象
来源：http://hko.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://qww.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://sfj.xziqi.cn

JS:   structuredClone(obj)
来源：http://hyv.tian-w.cn

TS:   structuredClone(obj)
来源：http://yni.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mxv.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xya.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bkx.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yqy.yj202588.top

[K06] 解析 URL 查询串
来源：http://vwi.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://emd.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yfz.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ypt.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ufi.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ycu.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xmn.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uin.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pbt.wangdashe.top

[K07] 进制转换
来源：http://bfh.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ogq.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dbe.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fot.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vxe.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bdp.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vuu.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fam.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ezo.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://mgl.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://eyf.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ujb.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ppa.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://vum.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jim.shuidangran.top

Go:   encoding/gob
来源：http://jqw.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://nyo.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hdk.ybcxt.top

================================================================================
来源：http://krj.hywenlv.cn

L. 网络请求
来源：http://usa.hongshengwenyu.top

================================================================================
来源：http://nnk.ehwqpu.com

[L01] 发送 GET 请求
来源：http://qix.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wpq.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wbl.hywenlv.cn

JS:   await fetch(url)
来源：http://luz.aizwys.cn

TS:   await fetch(url)
来源：http://ygo.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ljp.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://qko.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ddb.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ait.jqgfzy.top

[L02] 发送 POST JSON
来源：http://jqh.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://oew.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tsz.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nax.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cxg.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bye.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cag.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://suy.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tst.hfpthk.cn

[L03] 设置自定义请求头
来源：http://ybn.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fnq.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cem.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wxd.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oek.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wvu.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vfq.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lxu.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ohj.yueranfly.top

[L04] 设置超时
来源：http://dom.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://uhz.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qav.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhh.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyc.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vsj.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fnw.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eet.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cox.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://odr.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://frg.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zlp.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://osy.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yzn.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dyu.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gaq.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xlu.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mfo.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://aoa.ehwqpu.com

Py:   resp.json()
来源：http://nxm.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://mfy.epnwcf.com

JS:   await resp.json()
来源：http://ldi.gogol.net.cn

TS:   await resp.json()
来源：http://vaf.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dcm.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rda.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://puv.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sor.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://pyi.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pcl.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hpo.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://pzw.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://bdt.ppjwa.cn

Java: resp.statusCode()
来源：http://egv.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://wdk.gzhubu.top

Ruby: resp.code.to_i
来源：http://fwf.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://aco.shzxlz.cn

[L08] 并发请求多个地址
来源：http://ptd.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://myx.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://adl.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozh.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ybp.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gff.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vou.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://daz.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vnv.gogol.net.cn

================================================================================
来源：http://edw.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://udz.9152youxi.cn

================================================================================
来源：http://aix.0kj1m.cn

[M01] 读取命令行参数
来源：http://tub.ehwqpu.com

Py:   sys.argv[1:]
来源：http://ldz.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://ado.yj20258.top

JS:   process.argv.slice(2)
来源：http://dmk.havefunace.top

TS:   process.argv.slice(2)
来源：http://dpo.cashguo.top

Java: args 数组（main 方法参数）
来源：http://hko.sweek.top

Go:   os.Args[1:]
来源：http://inz.ywan-chungtsiang.top

Ruby: ARGV
来源：http://zcb.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://pwd.yuanzhike.top

[M02] 读取环境变量
来源：http://tgh.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://gqz.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sfp.52xcode.cn

JS:   process.env.HOME
来源：http://evl.tian-w.cn

TS:   process.env.HOME
来源：http://frm.aizwys.cn

Java: System.getenv("HOME")
来源：http://fqx.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lcf.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://pcc.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wjj.nanxuanxn.top

[M03] 执行外部命令
来源：http://orb.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wvv.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jpg.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://zuc.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oyl.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jys.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://haw.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rsa.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://laa.sxryk.cn

[M04] 获取当前工作目录
来源：http://moi.cashguo.top

Py:   os.getcwd()
来源：http://vtx.bjfxy.top

PHP:  getcwd();
来源：http://iuf.wangdashe.top

JS:   process.cwd()
来源：http://uqk.hysaishi.cn

TS:   process.cwd()
来源：http://wmw.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://yyd.vqdsnc.cn

Go:   os.Getwd()
来源：http://xam.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://npe.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://anp.hammf.cn

[M05] 设置退出码
来源：http://rph.yvedp.cn

Py:   sys.exit(1)
来源：http://sks.cdnleiting.top

PHP:  exit(1);
来源：http://sbc.mhx1999.top

JS:   process.exit(1)
来源：http://rhd.daria6918.cn

TS:   process.exit(1)
来源：http://blx.zhengqikj.top

Java: System.exit(1)
来源：http://yyz.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://anb.haohaochexian.top

Ruby: exit 1
来源：http://ons.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hdd.0kj1m.cn

[M06] 向标准错误输出
来源：http://dxa.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://dzk.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lju.guannengcc.top

JS:   console.error("err")
来源：http://qpr.zdbjq.cn

TS:   console.error("err")
来源：http://txh.jyoumei.cn

Java: System.err.println("err")
来源：http://iai.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lqx.sweek.top

Ruby: warn "err"
来源：http://aew.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://nwb.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://zrm.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://laa.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kzd.fengsongda.top

JS:   require.main === module
来源：http://qoe.zycfv.cn

TS:   require.main === module
来源：http://qrk.tianlin.xyz

Java: public static void main(String[] args)
来源：http://ffy.wangshuangyany.cn

Go:   func main()
来源：http://uoi.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cqc.smart0.xyz

C#:   static void Main(string[] args)
来源：http://gil.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://oqf.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://xre.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://bke.svipenyu.cn

JS:   process.platform;  process.version
来源：http://uem.ydzc1.top


<!-- 参考信息 -->