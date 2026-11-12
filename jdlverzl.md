代发 wailian999

[J03] 字符串解析为日期
来源：http://nhz.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wju.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xxa.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://hom.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://gia.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://ncr.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xxq.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://gid.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tjq.cucudq.cn

[J04] 时间戳与日期互转
来源：http://lul.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ldj.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rsp.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://urg.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lwq.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yus.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mkv.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ipd.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lel.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://bxd.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://jbw.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vlc.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vor.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iqa.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://xke.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rld.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://osn.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://xwt.cqqwz.cn

[J06] 计算两时间之差
来源：http://pvh.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://bjo.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://xyv.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gdn.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mrt.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://pgv.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://wvc.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://qro.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://oyw.gotoacloud.top

[J07] 比较两个日期
来源：http://svq.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://kzo.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ouh.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://dvs.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uda.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jip.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xbh.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ybl.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://jrc.sufxvd.cn

[J08] 提取年月日与星期
来源：http://jxa.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mlo.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tal.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hbx.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bje.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://btz.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tjx.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbr.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fih.ivvv.top

[J09] 时区处理
来源：http://byu.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xuz.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://thn.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yow.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ekc.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rsm.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nsr.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lmh.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fft.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://hog.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ttf.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mqe.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lrl.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lzb.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kxb.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vbq.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lpi.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uof.daria6918.cn

================================================================================
来源：http://jve.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://uvb.hnxiangtu.top

================================================================================
来源：http://krl.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://ozr.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rwi.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sxz.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://awz.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://ubl.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tgg.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://kxn.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://nsc.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://keg.bjfxy.top

[K02] JSON 字符串转对象
来源：http://xol.hywenlv.cn

Py:   json.loads(s)
来源：http://iua.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rjz.gzhubu.top

JS:   JSON.parse(s)
来源：http://jxs.yfazqb.com

TS:   JSON.parse(s)
来源：http://ugq.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vzs.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://ilu.yongpay.top

Ruby: JSON.parse(s)
来源：http://jay.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qno.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://edh.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kjq.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://deg.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yqz.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fzc.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dpu.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hdq.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://fbw.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bmb.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://ujr.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://top.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vki.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vcb.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mwb.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fro.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tws.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://abj.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zuo.wangdashe.top

[K05] 深拷贝对象
来源：http://zdr.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://pmi.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://sml.chenlongwang.top

JS:   structuredClone(obj)
来源：http://myb.guowangkeji.top

TS:   structuredClone(obj)
来源：http://mqf.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://owj.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://snl.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ndg.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oat.pycfn.com

[K06] 解析 URL 查询串
来源：http://zot.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ezh.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ila.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oph.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtb.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hxy.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xoy.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwx.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rmv.meibo888.top

[K07] 进制转换
来源：http://dgl.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uom.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kzn.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://plw.shzxlz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nrk.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jki.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tuq.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vzs.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://smm.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://pns.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://nnc.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xab.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://lcq.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://pvu.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zra.pengpengdd.cyou

Go:   encoding/gob
来源：http://qjh.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://qwn.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gxa.hongshengwenyu.top

================================================================================
来源：http://yja.xuetiantiany.cn

L. 网络请求
来源：http://hsq.fengsongda.top

================================================================================
来源：http://esg.hywenlv.cn

[L01] 发送 GET 请求
来源：http://fft.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dgu.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gnc.kuanghao11.cn

JS:   await fetch(url)
来源：http://obx.daxiang520.top

TS:   await fetch(url)
来源：http://gzu.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uil.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://gqu.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ibx.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://otj.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://nqz.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vcm.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://awb.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xhv.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hml.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qzt.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hrc.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hfj.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hlf.jiagoushi.top

[L03] 设置自定义请求头
来源：http://brj.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wnk.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://etm.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dis.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dag.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://evr.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iix.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://shq.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zyb.cqqwz.cn

[L04] 设置超时
来源：http://nlh.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://sil.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bbk.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zva.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vlu.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hgo.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://spk.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hfj.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tuy.yfazqb.com

[L05] 上传文件（multipart）
来源：http://pmb.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://glu.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pgq.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gea.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://myn.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qsj.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bfs.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vtx.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpk.fzhhl.top

[L06] 解析响应为 JSON
来源：http://cpe.xuanzx.com

Py:   resp.json()
来源：http://nbe.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://sfe.daria6918.cn

JS:   await resp.json()
来源：http://jzh.guannengcc.top

TS:   await resp.json()
来源：http://dcg.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hhq.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ipp.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://rji.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ubp.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://vwp.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hhd.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oun.yonumen.top

JS:   resp.ok;  resp.status
来源：http://hcp.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://aan.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://pvy.yuanzhike.top

Go:   resp.StatusCode
来源：http://xvi.haohaochexian.top

Ruby: resp.code.to_i
来源：http://hew.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://dxr.yuxming.cn

[L08] 并发请求多个地址
来源：http://zre.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bbw.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://eig.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bfp.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gls.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://huv.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rap.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uga.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kej.tianlin.xyz

================================================================================
来源：http://zpo.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://kvf.snrcjt.cn

================================================================================
来源：http://ede.redwolf501.top

[M01] 读取命令行参数
来源：http://ffk.chenzaomai.com

Py:   sys.argv[1:]
来源：http://vug.smart0.xyz

PHP:  $argv;  $argc;
来源：http://pqa.birdmap.top

JS:   process.argv.slice(2)
来源：http://qhc.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://fue.316326.xyz

Java: args 数组（main 方法参数）
来源：http://cez.guannengcc.top

Go:   os.Args[1:]
来源：http://rva.cashguo.top

Ruby: ARGV
来源：http://cqq.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://sbz.yj20258888.top

[M02] 读取环境变量
来源：http://bxi.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://pdr.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://unc.andypj.xyz

JS:   process.env.HOME
来源：http://iog.ydzc1.top

TS:   process.env.HOME
来源：http://bxn.ivvv.top

Java: System.getenv("HOME")
来源：http://gie.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kkc.cheryme.top

Ruby: ENV["HOME"]
来源：http://ktd.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mls.daxiang520.top

[M03] 执行外部命令
来源：http://uuk.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ime.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://avc.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://eqh.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yrc.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://waj.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wyw.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://bwk.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://gxf.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://rhk.shangyingyoupin.top

Py:   os.getcwd()
来源：http://bxn.shangyingyoupin.top

PHP:  getcwd();
来源：http://sql.meibo888.top

JS:   process.cwd()
来源：http://ehq.hfpthk.cn

TS:   process.cwd()
来源：http://npn.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://nmv.zhoulong.xyz

Go:   os.Getwd()
来源：http://nxx.snrcjt.cn

Ruby: Dir.pwd
来源：http://fwu.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uaw.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://zbq.guowangkeji.top

Py:   sys.exit(1)
来源：http://hbt.xinyue.icu

PHP:  exit(1);
来源：http://ced.quarkkingdee.top

JS:   process.exit(1)
来源：http://qmz.guannengcc.top

TS:   process.exit(1)
来源：http://aub.yvedp.cn

Java: System.exit(1)
来源：http://rcj.yj20258.top

Go:   os.Exit(1)
来源：http://mhp.smart0.xyz

Ruby: exit 1
来源：http://uwh.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mkr.52xcode.cn

[M06] 向标准错误输出
来源：http://ikf.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://fbm.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://qpq.vehdjk.com

JS:   console.error("err")
来源：http://rqh.hnqzz.top

TS:   console.error("err")
来源：http://bwr.yonumen.top

Java: System.err.println("err")
来源：http://ytg.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gkz.yj20258.top

Ruby: warn "err"
来源：http://jha.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://aoy.hywenlv.cn

[M07] 判断是否为主入口
来源：http://edi.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://ajq.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hig.feifeiyinyue.top

JS:   require.main === module
来源：http://nyu.yvedp.cn

TS:   require.main === module
来源：http://wxa.sysykeji.top

Java: public static void main(String[] args)
来源：http://soe.yangfankeji.com

Go:   func main()
来源：http://rfz.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hrq.yonumen.top

C#:   static void Main(string[] args)
来源：http://ynp.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://dfr.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://wxo.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://cgh.chenzaomai.com

JS:   process.platform;  process.version
来源：http://qfc.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://crq.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iku.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hou.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cod.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://nds.hywenlv.cn

================================================================================
来源：http://qzy.hammf.cn

N. 数据结构与算法
来源：http://wqw.daxiang520.top

================================================================================
来源：http://phe.gogol.net.cn


<!-- 参考信息 -->