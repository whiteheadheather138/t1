代发 wailian999

TS:   new Date("2024-01-02")
来源：http://rfw.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fps.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rau.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://otw.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cdk.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://epy.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ohk.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vhh.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cgv.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wlh.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bmg.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xly.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bvg.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ltf.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://vmv.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://rfc.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kna.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pbp.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgp.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://eji.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rwp.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://wsa.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lqh.uphjek.com

[J06] 计算两时间之差
来源：http://qhy.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://prn.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://puq.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://asc.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vrs.xinyue.icu

Java: Duration.between(start, end).toSeconds()
来源：http://imo.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://rez.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://ced.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://kcl.zdqjudy.top

[J07] 比较两个日期
来源：http://dnk.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://dgu.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lvu.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://vuw.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://klm.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ten.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://elf.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://lzs.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://srs.mhx1999.top

[J08] 提取年月日与星期
来源：http://azf.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lou.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xyu.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wem.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://syv.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vru.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mek.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://air.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://csc.jinyuanbaomall.cn

[J09] 时区处理
来源：http://dew.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wlk.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mye.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lvd.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmi.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uyo.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jvs.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rgg.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rhd.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://fct.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lvj.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dgm.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kur.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gxl.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pjd.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rro.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gpo.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jyw.shanyushiyangtech.top

================================================================================
来源：http://kwl.pycfn.com

K. JSON 与序列化
来源：http://akk.zhijiandao.cn

================================================================================
来源：http://gfa.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://zuj.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://czv.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qrl.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://zdi.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://wxs.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pku.uphjek.com

Go:   json.Marshal(obj)
来源：http://fef.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://eif.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://awj.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://ljv.chenzaomai.com

Py:   json.loads(s)
来源：http://adn.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rkv.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://clh.dianchejie.cn

TS:   JSON.parse(s)
来源：http://rff.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rbv.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://nan.iojbl.cn

Ruby: JSON.parse(s)
来源：http://zul.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://udl.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://jkn.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jgr.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ais.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wzx.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ksp.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vqj.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iwh.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://knf.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wvx.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://gqg.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wdp.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lxk.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zzb.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rlx.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uah.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bya.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ovz.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kyl.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://ogm.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://ztm.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://pyd.dianchejie.cn

JS:   structuredClone(obj)
来源：http://bew.redwolf501.top

TS:   structuredClone(obj)
来源：http://odd.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vuh.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tie.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dxe.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kge.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://ors.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eml.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xnb.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ukx.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noa.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ztj.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hwj.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bop.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tqf.iojbl.cn

[K07] 进制转换
来源：http://yfh.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kbw.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://swh.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uys.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vmt.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wwf.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pdc.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bwe.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oqa.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://uxr.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://trf.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xuw.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://qxg.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://toj.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fxy.gzhubu.top

Go:   encoding/gob
来源：http://iqn.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://oei.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xhx.gotoacloud.top

================================================================================
来源：http://dkc.redwolf501.top

L. 网络请求
来源：http://fdn.ivvv.top

================================================================================
来源：http://lcc.dashuyun.cn

[L01] 发送 GET 请求
来源：http://edl.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ezw.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pkq.xinyue.icu

JS:   await fetch(url)
来源：http://vkv.yj20258.top

TS:   await fetch(url)
来源：http://lwz.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kqf.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://gsf.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://knm.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eio.nwbrower.top

[L02] 发送 POST JSON
来源：http://lzs.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nxy.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ybb.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkj.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://odj.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wyu.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uxe.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gpc.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urz.zdbjq.cn

[L03] 设置自定义请求头
来源：http://yzv.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gdq.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gfo.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mif.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qie.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hiw.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tor.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yul.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fkf.aizwys.cn

[L04] 设置超时
来源：http://qop.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://fbm.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aqc.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmg.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hjr.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zyl.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qyk.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cfo.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cwd.ydzc1.top

[L05] 上传文件（multipart）
来源：http://axp.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rco.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nbi.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ytk.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qin.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pok.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rmr.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qwc.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vqv.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://snw.ctjpmb.com

Py:   resp.json()
来源：http://wdt.52xcode.cn

PHP:  json_decode($body, true);
来源：http://rfh.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://oyu.c1oappe.top

TS:   await resp.json()
来源：http://mfl.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ttw.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wci.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://rqq.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gpr.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://nnz.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yei.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pob.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://yks.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://sym.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://hok.hfpthk.cn

Go:   resp.StatusCode
来源：http://yrl.jianghu66.top

Ruby: resp.code.to_i
来源：http://pwc.yj202588.top

C#:   (int)resp.StatusCode
来源：http://inf.mhx1999.top

[L08] 并发请求多个地址
来源：http://emw.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cew.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://fzh.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lor.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sbd.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aqz.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hsz.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vxo.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fmj.redwolf501.top

================================================================================
来源：http://jwv.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://yil.zhiwuduotai.top

================================================================================
来源：http://knw.ybcxt.top

[M01] 读取命令行参数
来源：http://mtz.aibaodan.cn

Py:   sys.argv[1:]
来源：http://xsd.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://aee.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://usw.wangdashe.top

TS:   process.argv.slice(2)
来源：http://gjk.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://ssc.yuxming.cn

Go:   os.Args[1:]
来源：http://woz.guannengcc.top

Ruby: ARGV
来源：http://clh.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://xga.shangyingyoupin.top

[M02] 读取环境变量
来源：http://vsl.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://kgv.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qcl.9152youxi.cn

JS:   process.env.HOME
来源：http://udz.iojbl.cn

TS:   process.env.HOME
来源：http://fbi.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://pws.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ojl.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://vmc.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xyh.yueranfly.top

[M03] 执行外部命令
来源：http://bfq.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oad.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sah.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sjt.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jqk.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ali.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tkt.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://clc.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://zre.hysaishi.cn

[M04] 获取当前工作目录
来源：http://kdi.hammf.cn

Py:   os.getcwd()
来源：http://dqj.xinyue.icu

PHP:  getcwd();
来源：http://pwz.mhx1999.top

JS:   process.cwd()
来源：http://dly.ehwqpu.com

TS:   process.cwd()
来源：http://niz.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://glp.ydzc1.top

Go:   os.Getwd()
来源：http://ujf.cqqwz.cn

Ruby: Dir.pwd
来源：http://qxi.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bqe.havefunace.top

[M05] 设置退出码
来源：http://cmg.shzxlz.cn

Py:   sys.exit(1)
来源：http://uwa.bjfxy.top

PHP:  exit(1);
来源：http://yyr.uphjek.com

JS:   process.exit(1)
来源：http://kbn.hysaishi.cn

TS:   process.exit(1)
来源：http://nhs.gogol.net.cn

Java: System.exit(1)
来源：http://afu.kuanghao11.cn

Go:   os.Exit(1)
来源：http://tfv.xziqi.cn

Ruby: exit 1
来源：http://dof.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gdf.zhengqikj.top

[M06] 向标准错误输出
来源：http://pby.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://prc.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://pcn.snrcjt.cn

JS:   console.error("err")
来源：http://bab.pengpengdd.cyou

TS:   console.error("err")
来源：http://kwv.ppjwa.cn

Java: System.err.println("err")
来源：http://spv.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cse.zdbjq.cn

Ruby: warn "err"
来源：http://xpu.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://acm.epnwcf.com

[M07] 判断是否为主入口
来源：http://jhs.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://dyc.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xim.shzxlz.cn

JS:   require.main === module
来源：http://bzx.shzxlz.cn

TS:   require.main === module
来源：http://fsi.ppjwa.cn

Java: public static void main(String[] args)
来源：http://mfy.zhengqikj.top

Go:   func main()
来源：http://mrk.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ayq.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://sxt.birdmap.top

[M08] 获取系统与运行时信息
来源：http://cof.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://wvy.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://nsn.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://umu.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://pxn.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://akz.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yqe.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rwy.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jhv.shanyushiyangtech.top

================================================================================
来源：http://lqt.hammf.cn

N. 数据结构与算法
来源：http://avh.zhoulong.xyz

================================================================================
来源：http://ylr.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://mui.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://tpo.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wsa.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zpf.wangdashe.top


<!-- 参考信息 -->