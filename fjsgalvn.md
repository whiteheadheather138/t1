代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ozg.yonumen.top

[J04] 时间戳与日期互转
来源：http://aar.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lof.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://imf.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dct.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yat.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qdn.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qcf.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fzz.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qab.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://ufy.yj20258.top

Py:   now + timedelta(days=7)
来源：http://cmx.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ece.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hts.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wbw.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://krh.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://but.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://rpz.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sfr.jlsjyb.cn

[J06] 计算两时间之差
来源：http://czt.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://nnb.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://suq.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ffl.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zrq.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://glx.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://rsp.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://ssy.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://bqf.ctjpmb.com

[J07] 比较两个日期
来源：http://tzk.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wyv.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hec.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fmo.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://eje.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjm.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vaq.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://ucq.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://dhl.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://qge.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ptd.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://adl.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gdp.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ffr.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ofu.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://egg.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tqo.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pdm.yongpay.top

[J09] 时区处理
来源：http://cuq.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bwv.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jkm.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://obk.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsl.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vdy.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rpv.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aed.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ykf.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://ovh.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://tyj.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qjm.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yua.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zly.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bxd.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yfy.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kmo.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ept.jlsjyb.cn

================================================================================
来源：http://uma.jqgfzy.top

K. JSON 与序列化
来源：http://kob.ivvv.top

================================================================================
来源：http://mtd.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://jgx.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vig.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jza.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://yon.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://zoe.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fia.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://bmm.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://tlp.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dnm.uphjek.com

[K02] JSON 字符串转对象
来源：http://lml.pengpengdd.cyou

Py:   json.loads(s)
来源：http://ajo.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jbi.snrcjt.cn

JS:   JSON.parse(s)
来源：http://nce.xylfe.cn

TS:   JSON.parse(s)
来源：http://jot.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gcs.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://oip.52xcode.cn

Ruby: JSON.parse(s)
来源：http://pwi.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tiz.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://chu.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dhu.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ssj.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bmx.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eue.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ibc.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ggr.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://jkk.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cdu.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://odk.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nsq.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://agv.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xic.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://brb.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vro.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lyn.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mtd.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://phl.iojbl.cn

[K05] 深拷贝对象
来源：http://ydw.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://giz.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://veb.yongpay.top

JS:   structuredClone(obj)
来源：http://pzh.vehdjk.com

TS:   structuredClone(obj)
来源：http://mzk.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vlw.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xdv.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ztt.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wjd.bjfxy.top

[K06] 解析 URL 查询串
来源：http://svu.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mkn.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jkc.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://seq.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jii.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://inq.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cqp.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aoi.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rmv.hnqzz.top

[K07] 进制转换
来源：http://bma.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pmk.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mjx.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kqm.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kzu.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vay.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kuo.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mil.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ami.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://ewj.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://ewk.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rmi.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://rwp.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://gow.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pcc.vqdsnc.cn

Go:   encoding/gob
来源：http://abe.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://uqn.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zrf.xuetiantiany.cn

================================================================================
来源：http://etj.yonumen.top

L. 网络请求
来源：http://bce.9152youxi.cn

================================================================================
来源：http://eaz.havefunace.top

[L01] 发送 GET 请求
来源：http://bqq.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wlq.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://onr.xinyue.icu

JS:   await fetch(url)
来源：http://znx.dashuyun.cn

TS:   await fetch(url)
来源：http://fos.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rcv.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://oih.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eyg.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://isi.zdbjq.cn

[L02] 发送 POST JSON
来源：http://fnk.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://qwm.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fmc.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zyo.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izf.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zsl.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zzf.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nri.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ptx.ctjpmb.com

[L03] 设置自定义请求头
来源：http://euc.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cts.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oze.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tqj.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ogy.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://txx.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kev.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gfl.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bgd.tianlin.xyz

[L04] 设置超时
来源：http://xyx.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://hmq.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://imy.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ghb.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zek.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vfy.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qls.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://azw.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lcu.smart0.xyz

[L05] 上传文件（multipart）
来源：http://ahm.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fcn.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vow.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lmc.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lps.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fdm.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ndj.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bos.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lhj.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://isi.ppjwa.cn

Py:   resp.json()
来源：http://woq.meibo888.top

PHP:  json_decode($body, true);
来源：http://ltv.ydzc1.top

JS:   await resp.json()
来源：http://zht.nanxinkj.top

TS:   await resp.json()
来源：http://zbi.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oco.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kwe.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://kry.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gec.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://xcn.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ryi.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yki.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://dve.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://rou.tian-w.cn

Java: resp.statusCode()
来源：http://egg.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://yfi.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://veo.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://xvt.gzhubu.top

[L08] 并发请求多个地址
来源：http://jus.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wiz.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://kjp.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fko.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://doi.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://efg.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ifd.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ytg.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://idb.jiagoushi.top

================================================================================
来源：http://llp.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://igh.hnxiangtu.top

================================================================================
来源：http://ljm.zdqjudy.top

[M01] 读取命令行参数
来源：http://ouv.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://xzy.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://pbf.fzhhl.top

JS:   process.argv.slice(2)
来源：http://puw.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://mcw.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://rdw.mhx1999.top

Go:   os.Args[1:]
来源：http://oea.yangfankeji.com

Ruby: ARGV
来源：http://qxm.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://mkq.vqdsnc.cn

[M02] 读取环境变量
来源：http://znc.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://hev.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pme.jyoumei.cn

JS:   process.env.HOME
来源：http://eyr.gaohongyu789.top

TS:   process.env.HOME
来源：http://ope.sweek.top

Java: System.getenv("HOME")
来源：http://bce.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gtw.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://wnn.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bwn.pengpengdd.cyou

[M03] 执行外部命令
来源：http://kst.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bsp.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ynm.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jdc.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pjk.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dux.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ycw.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://psa.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://duy.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://gzk.mhx1999.top

Py:   os.getcwd()
来源：http://dlr.yvedp.cn

PHP:  getcwd();
来源：http://zkg.yongpay.top

JS:   process.cwd()
来源：http://yfk.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://oqa.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://nal.zhixingplan.top

Go:   os.Getwd()
来源：http://qks.yanxiufei.cn

Ruby: Dir.pwd
来源：http://jzv.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jdj.ydzc1.top

[M05] 设置退出码
来源：http://rta.gotoacloud.top

Py:   sys.exit(1)
来源：http://clv.smart0.xyz

PHP:  exit(1);
来源：http://wgl.gotoacloud.top

JS:   process.exit(1)
来源：http://mao.fengsongda.top

TS:   process.exit(1)
来源：http://hvg.yj202588.top

Java: System.exit(1)
来源：http://nuo.gogol.net.cn

Go:   os.Exit(1)
来源：http://zra.ppjwa.cn

Ruby: exit 1
来源：http://pmx.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://naz.jqgfzy.top

[M06] 向标准错误输出
来源：http://ioy.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://gdg.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ypj.hywenlv.cn

JS:   console.error("err")
来源：http://jkd.snrcjt.cn

TS:   console.error("err")
来源：http://rdq.pengpengdd.cyou

Java: System.err.println("err")
来源：http://mot.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wxy.jqgufenzy.top

Ruby: warn "err"
来源：http://prh.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://sei.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://hev.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://edv.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ywg.jqgfzy.top

JS:   require.main === module
来源：http://aqc.jqgufenzy.top

TS:   require.main === module
来源：http://xjc.zhixingplan.top

Java: public static void main(String[] args)
来源：http://plq.zdqjudy.top

Go:   func main()
来源：http://pis.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jjg.aizwys.cn

C#:   static void Main(string[] args)
来源：http://smw.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://etw.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://xeq.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://xgo.fengsongda.top

JS:   process.platform;  process.version
来源：http://ivd.ppjwa.cn

TS:   process.platform;  process.version
来源：http://iis.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ynp.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dfb.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nce.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fae.mhx1999.top

================================================================================
来源：http://uqr.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://nor.snrcjt.cn

================================================================================
来源：http://sxp.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://awv.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://san.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://epo.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vnp.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jml.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ubd.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://cpm.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://udt.tanke756.top


<!-- 参考信息 -->