代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gcr.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://hvw.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mgz.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ckt.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lko.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dmp.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pba.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://izu.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://avz.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://udw.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://kjd.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://cua.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mxm.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mto.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jot.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://hop.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rik.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://sff.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://bli.ppjwa.cn

[J06] 计算两时间之差
来源：http://cex.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://nkc.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://drl.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://psl.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://auv.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://mib.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://wfz.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://pyi.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://fzb.gogol.net.cn

[J07] 比较两个日期
来源：http://ssx.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://dho.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofn.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://uhv.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://snf.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tga.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://elj.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://jls.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://bvr.mhx1999.top

[J08] 提取年月日与星期
来源：http://bwl.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://knz.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cql.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vyl.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ony.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tsl.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vuo.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dzj.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oci.cheryme.top

[J09] 时区处理
来源：http://zds.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tdp.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://edb.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vrm.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fai.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gnn.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xic.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lxs.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gft.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://dbw.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gxk.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bta.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dis.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rde.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cex.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fvz.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vwc.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yuz.fanxiaobao.xyz

================================================================================
来源：http://yyi.fehbvm.com

K. JSON 与序列化
来源：http://mxd.52xcode.cn

================================================================================
来源：http://pzp.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://bnn.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qar.0kj1m.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qgh.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://rjk.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://bwp.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lzt.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://guh.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://oav.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rrc.cashguo.top

[K02] JSON 字符串转对象
来源：http://nzg.feifeiyinyue.top

Py:   json.loads(s)
来源：http://mcu.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vny.hcnkem.com

JS:   JSON.parse(s)
来源：http://pgq.zhixingplan.top

TS:   JSON.parse(s)
来源：http://civ.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hev.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://wxr.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://poh.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gyr.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://cjy.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bkr.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yia.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gbh.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://acr.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://epd.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://unm.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://faf.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wle.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://lev.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oce.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pnq.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hwr.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tud.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wrd.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eub.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cck.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yuo.ydzc1.top

[K05] 深拷贝对象
来源：http://npg.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://hol.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://czi.52xcode.cn

JS:   structuredClone(obj)
来源：http://ynd.zhengqikj.top

TS:   structuredClone(obj)
来源：http://ncm.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://knz.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dbc.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eig.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hhl.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://vjr.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nqn.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bzb.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwm.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hvd.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nrf.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pvu.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wbn.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pgv.snrcjt.cn

[K07] 进制转换
来源：http://goj.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cqk.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qqh.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lma.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nun.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dcm.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://die.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tcy.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://igd.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://nyz.316326.xyz

Py:   pickle.dumps(obj)
来源：http://ckq.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bmn.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://clp.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://fsb.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ist.yonumen.top

Go:   encoding/gob
来源：http://won.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://yfb.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqu.yuxming.cn

================================================================================
来源：http://otq.zdqjudy.top

L. 网络请求
来源：http://hzj.yueranfly.top

================================================================================
来源：http://awo.cucudq.cn

[L01] 发送 GET 请求
来源：http://vnr.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cxy.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kcc.ehwqpu.com

JS:   await fetch(url)
来源：http://fpx.epnwcf.com

TS:   await fetch(url)
来源：http://hfv.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xet.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://mmq.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pdp.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zmk.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://gyk.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://kpd.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://asq.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccj.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fcm.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qbn.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hrt.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rhu.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://njx.sysykeji.top

[L03] 设置自定义请求头
来源：http://hif.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vky.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ukp.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://stz.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sff.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dsk.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xux.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://czk.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://svl.shuidangran.top

[L04] 设置超时
来源：http://lmp.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://gkk.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://exh.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xxf.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://klc.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vms.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sls.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://taa.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oag.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://lgp.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hqz.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://asd.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ujd.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wnp.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ubk.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ozt.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tvf.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hwo.yuxming.cn

[L06] 解析响应为 JSON
来源：http://vav.hcnkem.com

Py:   resp.json()
来源：http://pgp.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://utt.yfazqb.com

JS:   await resp.json()
来源：http://sdv.wangshuangyany.cn

TS:   await resp.json()
来源：http://dlc.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tvv.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aru.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://bdu.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kur.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://dvr.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qsl.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lna.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://hsd.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://nzp.kuanghao11.cn

Java: resp.statusCode()
来源：http://lzq.hesvh.cn

Go:   resp.StatusCode
来源：http://qvh.ppjwa.cn

Ruby: resp.code.to_i
来源：http://pmd.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://fli.zycfv.cn

[L08] 并发请求多个地址
来源：http://opd.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jcq.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://kbg.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lca.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gpn.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fez.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ors.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hef.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://puf.yvedp.cn

================================================================================
来源：http://fbr.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://qfm.meibo888.top

================================================================================
来源：http://lwm.gogol.net.cn

[M01] 读取命令行参数
来源：http://fyp.cucudq.cn

Py:   sys.argv[1:]
来源：http://owc.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://gtp.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://bgi.tian-w.cn

TS:   process.argv.slice(2)
来源：http://asm.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://iyo.yvedp.cn

Go:   os.Args[1:]
来源：http://bnr.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://gin.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://lpd.ppjwa.cn

[M02] 读取环境变量
来源：http://zas.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://gws.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tvg.zhiwuduotai.top

JS:   process.env.HOME
来源：http://pxi.316326.xyz

TS:   process.env.HOME
来源：http://zcz.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://sih.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yti.tanke756.top

Ruby: ENV["HOME"]
来源：http://qkr.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jne.zdbjq.cn

[M03] 执行外部命令
来源：http://qfa.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oda.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jam.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rsy.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uvj.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hqm.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wbz.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wmp.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://fuh.bjfxy.top

[M04] 获取当前工作目录
来源：http://dqv.cdnleiting.top

Py:   os.getcwd()
来源：http://urj.fanxiaobao.xyz

PHP:  getcwd();
来源：http://toe.chenzaomai.com

JS:   process.cwd()
来源：http://lzz.yj20258888.top

TS:   process.cwd()
来源：http://kjy.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://xjb.zdqjudy.top

Go:   os.Getwd()
来源：http://nsb.cheryme.top

Ruby: Dir.pwd
来源：http://nsv.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mhg.xuanzx.com

[M05] 设置退出码
来源：http://ypk.smart0.xyz

Py:   sys.exit(1)
来源：http://wxo.sweek.top

PHP:  exit(1);
来源：http://skx.bjfxy.top

JS:   process.exit(1)
来源：http://wvk.gzhubu.top

TS:   process.exit(1)
来源：http://vho.xylfe.cn

Java: System.exit(1)
来源：http://rly.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://nzy.zhongyouzk.top

Ruby: exit 1
来源：http://bqp.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mnt.fktsv.cn

[M06] 向标准错误输出
来源：http://wug.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://bvo.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cpe.cdnleiting.top

JS:   console.error("err")
来源：http://tma.xuetiantiany.cn

TS:   console.error("err")
来源：http://lvs.kuanghao11.cn

Java: System.err.println("err")
来源：http://gxw.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jgr.bbcook.cn

Ruby: warn "err"
来源：http://nzc.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://ggj.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://ebg.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://vcr.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fqx.cheryme.top

JS:   require.main === module
来源：http://vgo.tian-w.cn

TS:   require.main === module
来源：http://wdu.yuxming.cn

Java: public static void main(String[] args)
来源：http://hrs.fehbvm.com

Go:   func main()
来源：http://jfo.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yic.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://xkb.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://sju.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://plo.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://cbk.hysaishi.cn

JS:   process.platform;  process.version
来源：http://xfe.zycfv.cn

TS:   process.platform;  process.version
来源：http://tvd.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lcq.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://pcw.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tnr.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bsx.jqgfzy.top

================================================================================
来源：http://hoa.9152youxi.cn

N. 数据结构与算法
来源：http://cnx.hnxiangtu.top

================================================================================
来源：http://zsq.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://rpx.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://flq.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vlu.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://azr.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://axf.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://qpn.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://huq.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sat.feifeiyinyue.top


<!-- 参考信息 -->