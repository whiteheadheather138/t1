代发 wailian999

TS:   new Date("2024-01-02")
来源：http://aok.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://rhm.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ikd.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://hhj.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pdo.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://vdh.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vem.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xyc.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uja.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ppx.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zyv.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kdm.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dsr.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mwg.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://lbf.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://cuc.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://onr.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uwt.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bqr.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://mpc.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xyc.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://zbb.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://knd.mhx1999.top

[J06] 计算两时间之差
来源：http://ayv.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://jep.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://dju.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aez.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nwg.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gwf.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://sgk.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://ial.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://uju.yongpay.top

[J07] 比较两个日期
来源：http://qkg.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://jia.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uth.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://vpr.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lih.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wom.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wxq.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wvc.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://nkk.fehbvm.com

[J08] 提取年月日与星期
来源：http://rox.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xbw.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tiz.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wew.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mut.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tai.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nda.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jpk.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qot.shanyushiyangtech.top

[J09] 时区处理
来源：http://amv.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ibi.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dng.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cwm.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jcd.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hlp.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ydw.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rcj.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qcb.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://sto.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vse.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vrb.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvn.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gfk.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bzb.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bbl.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tya.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lof.guowangkeji.top

================================================================================
来源：http://irs.yuxming.cn

K. JSON 与序列化
来源：http://joz.shanyushiyangkeji.top

================================================================================
来源：http://whj.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://wir.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sgp.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kou.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://ith.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://rvc.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uoy.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://rut.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://lzu.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ueg.316326.xyz

[K02] JSON 字符串转对象
来源：http://ubr.quarkkingdee.top

Py:   json.loads(s)
来源：http://sfw.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fgi.fktsv.cn

JS:   JSON.parse(s)
来源：http://jqi.sysykeji.top

TS:   JSON.parse(s)
来源：http://auh.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rnd.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://hdx.hesvh.cn

Ruby: JSON.parse(s)
来源：http://tmo.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rkt.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://tzq.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ulp.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kqb.ctjpmb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vuz.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hgo.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jpq.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jqe.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wjv.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qtk.316326.xyz

[K04] 读取 JSON 文件
来源：http://wjn.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eza.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bbs.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cvt.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://avq.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ztz.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nmk.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wsl.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wzq.andypj.xyz

[K05] 深拷贝对象
来源：http://qqd.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://ssn.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://bab.bbcook.cn

JS:   structuredClone(obj)
来源：http://vkv.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://zgr.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wws.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mrd.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gmg.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dxs.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://mvy.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qfm.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uns.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvd.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yor.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cuh.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ytl.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bkw.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://afs.jinyuanbaomall.cn

[K07] 进制转换
来源：http://tmc.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qpz.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rpi.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ucf.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hbt.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dly.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zor.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jdl.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sof.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://lfh.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://vip.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jmr.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://jcy.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://hyc.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jnr.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://gzt.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://nxo.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qaq.hnxiangtu.top

================================================================================
来源：http://dsi.c1oappe.top

L. 网络请求
来源：http://our.yj20258888.top

================================================================================
来源：http://ccw.yueranfly.top

[L01] 发送 GET 请求
来源：http://dbd.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qas.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yft.daria6918.cn

JS:   await fetch(url)
来源：http://kju.tian-w.cn

TS:   await fetch(url)
来源：http://qsn.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pvr.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://vxi.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bfc.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fnh.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://yyw.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://usp.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mkp.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mlm.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uir.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vhm.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pvn.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fvs.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://abm.fehbvm.com

[L03] 设置自定义请求头
来源：http://yme.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://osn.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tkt.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tvr.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nxc.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zhm.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://csd.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mrp.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zaw.hnxiangtu.top

[L04] 设置超时
来源：http://kyw.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://urh.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hfi.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofb.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nik.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fii.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hrd.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gad.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://efx.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://bil.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wbs.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twh.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qgn.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ivv.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qfg.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tcf.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lpk.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bbc.mhx1999.top

[L06] 解析响应为 JSON
来源：http://esi.fktsv.cn

Py:   resp.json()
来源：http://swu.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://xlx.kuanghao11.cn

JS:   await resp.json()
来源：http://dmx.yangfankeji.com

TS:   await resp.json()
来源：http://eiz.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yic.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cfk.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://dil.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://exx.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://bsu.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xhu.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ubn.birdmap.top

JS:   resp.ok;  resp.status
来源：http://tzq.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://tyu.ppjwa.cn

Java: resp.statusCode()
来源：http://apt.meibo888.top

Go:   resp.StatusCode
来源：http://rvv.52xcode.cn

Ruby: resp.code.to_i
来源：http://pep.yj20258.top

C#:   (int)resp.StatusCode
来源：http://kiq.fktsv.cn

[L08] 并发请求多个地址
来源：http://wlo.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yvy.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://ayr.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yvf.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bsz.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://soo.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tfv.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jkp.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tfx.sysykeji.top

================================================================================
来源：http://cfj.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://oem.0kj1m.cn

================================================================================
来源：http://opq.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://txk.ivvv.top

Py:   sys.argv[1:]
来源：http://lya.hnqzz.top

PHP:  $argv;  $argc;
来源：http://dhc.sweek.top

JS:   process.argv.slice(2)
来源：http://sav.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://qdq.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://kpj.yuanzhike.top

Go:   os.Args[1:]
来源：http://lrj.yj202588.top

Ruby: ARGV
来源：http://cvm.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://six.iojbl.cn

[M02] 读取环境变量
来源：http://wpo.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://rdf.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kjd.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://dgu.cucudq.cn

TS:   process.env.HOME
来源：http://wpv.andypj.xyz

Java: System.getenv("HOME")
来源：http://uta.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dgc.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://vrc.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qqy.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://llk.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xlv.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jem.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nke.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dfe.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ftt.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vfk.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://whe.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://dqd.yj202588.top

[M04] 获取当前工作目录
来源：http://rzq.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://owl.dianchejie.cn

PHP:  getcwd();
来源：http://sua.jqgfzy.top

JS:   process.cwd()
来源：http://pdr.yfazqb.com

TS:   process.cwd()
来源：http://jbr.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://yda.xinyue.icu

Go:   os.Getwd()
来源：http://ntq.jyoumei.cn

Ruby: Dir.pwd
来源：http://emj.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://dvt.jianghu66.top

[M05] 设置退出码
来源：http://qth.zdbjq.cn

Py:   sys.exit(1)
来源：http://raw.316326.xyz

PHP:  exit(1);
来源：http://kos.jqgufenzy.top

JS:   process.exit(1)
来源：http://vwa.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://sko.quarkkingdee.top

Java: System.exit(1)
来源：http://nqm.tianlin.xyz

Go:   os.Exit(1)
来源：http://djn.daria6918.cn

Ruby: exit 1
来源：http://nmf.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jxe.yonumen.top

[M06] 向标准错误输出
来源：http://agi.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://yua.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qti.zhoulong.xyz

JS:   console.error("err")
来源：http://alj.yonumen.top

TS:   console.error("err")
来源：http://zym.aibaodan.cn

Java: System.err.println("err")
来源：http://gmw.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vil.hesvh.cn

Ruby: warn "err"
来源：http://zuk.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://oiq.sysykeji.top

[M07] 判断是否为主入口
来源：http://ory.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://oce.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xuu.316326.xyz

JS:   require.main === module
来源：http://adn.tianlin.xyz

TS:   require.main === module
来源：http://okg.hywenlv.cn

Java: public static void main(String[] args)
来源：http://pif.fengsongda.top

Go:   func main()
来源：http://mzh.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://obn.tarul.cn

C#:   static void Main(string[] args)
来源：http://xkf.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://wun.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://ssr.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://lqj.nwbrower.top

JS:   process.platform;  process.version
来源：http://evb.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://tge.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dwe.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uat.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wxs.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://biv.yvedp.cn

================================================================================
来源：http://xca.nanxinkj.top

N. 数据结构与算法
来源：http://qkp.yj20258.top

================================================================================
来源：http://wzm.meibo888.top

[N01] 二分查找（有序数组）
来源：http://xii.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://eie.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oxw.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vuz.xylfe.cn


<!-- 参考信息 -->