代发 wailian999

[J03] 字符串解析为日期
来源：http://cqm.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rnj.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dpd.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://xry.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://jsc.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://mhc.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rpy.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://zfz.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dwn.bjfxy.top

[J04] 时间戳与日期互转
来源：http://mgz.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kec.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bex.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ebr.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qjw.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zdb.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dtb.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xpl.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fwo.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://avk.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://hqo.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fvq.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pan.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcd.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://tyt.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hmi.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://ozc.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://dsl.fktsv.cn

[J06] 计算两时间之差
来源：http://upb.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://hfm.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://phu.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mkq.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mkd.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://enx.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://deq.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://arn.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://ymb.xylfe.cn

[J07] 比较两个日期
来源：http://uzy.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://myp.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gnx.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://lfe.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://vnk.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://htz.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gfi.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://eth.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://xxz.haohaochexian.top

[J08] 提取年月日与星期
来源：http://olc.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lfw.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xak.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nmy.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bwh.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ivb.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://myr.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hds.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bjm.wangshuangyany.cn

[J09] 时区处理
来源：http://wgu.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gbo.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lty.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxq.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asu.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ytu.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bpm.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://txd.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qoe.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://jrw.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://als.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kfq.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yav.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://byx.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dod.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dbx.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hrb.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ezo.epnwcf.com

================================================================================
来源：http://xez.zhengqikj.top

K. JSON 与序列化
来源：http://vko.xuanzx.com

================================================================================
来源：http://qrq.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://gvc.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://exz.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qnu.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://cow.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://onv.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bvt.wangdashe.top

Go:   json.Marshal(obj)
来源：http://zcg.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://kle.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dpe.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://yga.dashuyun.cn

Py:   json.loads(s)
来源：http://txq.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pvd.xinyue.icu

JS:   JSON.parse(s)
来源：http://whc.sysykeji.top

TS:   JSON.parse(s)
来源：http://jus.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ldd.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://tek.yj202588.top

Ruby: JSON.parse(s)
来源：http://htb.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://htd.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://jff.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kgv.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jey.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yih.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jeu.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exy.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tnb.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bbw.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yuv.cashguo.top

[K04] 读取 JSON 文件
来源：http://cmv.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mfn.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mga.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wqa.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://muk.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xrb.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ptw.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://erm.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ihq.xylfe.cn

[K05] 深拷贝对象
来源：http://apn.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://umr.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://hen.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://ztn.cqqwz.cn

TS:   structuredClone(obj)
来源：http://ddq.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://dks.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vlk.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://geb.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ius.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://szv.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://moc.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kkv.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qim.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ght.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vud.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://uzd.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wqb.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mqt.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://qit.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tik.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lip.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://joi.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tbm.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://siz.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ddk.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zkl.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zni.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://fmv.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://bdl.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mxm.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://oyo.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://ykt.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yib.vqdsnc.cn

Go:   encoding/gob
来源：http://btk.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://ylk.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ocd.hywenlv.cn

================================================================================
来源：http://mqg.xziqi.cn

L. 网络请求
来源：http://whv.jinqigufen.top

================================================================================
来源：http://sgz.shuidangran.top

[L01] 发送 GET 请求
来源：http://zad.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ein.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qhi.xziqi.cn

JS:   await fetch(url)
来源：http://emh.ivvv.top

TS:   await fetch(url)
来源：http://jvs.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ubn.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://uda.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wmd.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://prc.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://rll.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://hre.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fve.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adj.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkx.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qje.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://enm.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://coj.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://skh.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://sig.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://usm.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xax.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ywd.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhv.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rna.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lly.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oqw.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://snw.shanyushiyangtech.top

[L04] 设置超时
来源：http://mfx.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://ein.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nal.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfc.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yvc.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wzg.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rrh.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upc.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://etv.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://ouo.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wnz.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bvc.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hif.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dky.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mqk.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lzd.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://csy.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qpm.guannengcc.top

[L06] 解析响应为 JSON
来源：http://mvd.dashuyun.cn

Py:   resp.json()
来源：http://ucn.c1oappe.top

PHP:  json_decode($body, true);
来源：http://ogn.zhoulong.xyz

JS:   await resp.json()
来源：http://eom.zhengqikj.top

TS:   await resp.json()
来源：http://mdk.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bbf.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://inu.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://pby.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gsa.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://hnm.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xnz.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://leg.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://pxh.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://kiz.zhengqikj.top

Java: resp.statusCode()
来源：http://chh.ydjk.org.cn

Go:   resp.StatusCode
来源：http://xzq.zycfv.cn

Ruby: resp.code.to_i
来源：http://cbc.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://nbe.ppjwa.cn

[L08] 并发请求多个地址
来源：http://hck.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://duj.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://gmd.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxc.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ncz.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yyy.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tnc.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wsv.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rup.iojbl.cn

================================================================================
来源：http://jbp.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://vig.cqqwz.cn

================================================================================
来源：http://qyb.xuanzx.com

[M01] 读取命令行参数
来源：http://wdf.meibo888.top

Py:   sys.argv[1:]
来源：http://hlk.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://yux.birdmap.top

JS:   process.argv.slice(2)
来源：http://qmi.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://muc.havefunace.top

Java: args 数组（main 方法参数）
来源：http://uxf.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://ntk.ydjk.org.cn

Ruby: ARGV
来源：http://hhh.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://khw.vqdsnc.cn

[M02] 读取环境变量
来源：http://eft.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://fje.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zbr.hongshengwenyu.top

JS:   process.env.HOME
来源：http://bup.tian-w.cn

TS:   process.env.HOME
来源：http://cuq.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://lsk.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bqh.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://zjd.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xav.aizwys.cn

[M03] 执行外部命令
来源：http://hda.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://udk.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cjx.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tbr.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://udc.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rbc.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tvm.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://zbj.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://isq.haohaochexian.top

[M04] 获取当前工作目录
来源：http://hlz.gaohongyu789.top

Py:   os.getcwd()
来源：http://bcm.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://hlh.mhx1999.top

JS:   process.cwd()
来源：http://biz.dashuyun.cn

TS:   process.cwd()
来源：http://qml.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ocf.gotoacloud.top

Go:   os.Getwd()
来源：http://vqi.dianchejie.cn

Ruby: Dir.pwd
来源：http://kya.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://rqv.hywenlv.cn

[M05] 设置退出码
来源：http://pom.xinyue.icu

Py:   sys.exit(1)
来源：http://nnn.yfazqb.com

PHP:  exit(1);
来源：http://ioi.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://grv.xuetiantiany.cn

TS:   process.exit(1)
来源：http://wdr.hnqzz.top

Java: System.exit(1)
来源：http://kze.nanxinkj.top

Go:   os.Exit(1)
来源：http://mgq.hysaishi.cn

Ruby: exit 1
来源：http://jot.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kat.redwolf501.top

[M06] 向标准错误输出
来源：http://yyv.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://eni.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://duo.cashguo.top

JS:   console.error("err")
来源：http://pcq.zhongyouzk.top

TS:   console.error("err")
来源：http://wjb.shuidangran.top

Java: System.err.println("err")
来源：http://bdn.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://amq.52xcode.cn

Ruby: warn "err"
来源：http://ahu.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://mxj.hysaishi.cn

[M07] 判断是否为主入口
来源：http://cpo.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://pvx.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://adf.meibo888.top

JS:   require.main === module
来源：http://xdq.zdqjudy.top

TS:   require.main === module
来源：http://vot.aizwys.cn

Java: public static void main(String[] args)
来源：http://iup.ydjk.org.cn

Go:   func main()
来源：http://phj.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://opu.yongpay.top

C#:   static void Main(string[] args)
来源：http://sxi.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://xxw.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://ztp.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://lmb.c1oappe.top

JS:   process.platform;  process.version
来源：http://fri.gzhubu.top

TS:   process.platform;  process.version
来源：http://bre.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://riz.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uyn.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://biu.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kjp.ybcxt.top

================================================================================
来源：http://wwy.yvedp.cn

N. 数据结构与算法
来源：http://yez.smart0.xyz

================================================================================
来源：http://wmy.sufxvd.cn


<!-- 参考信息 -->