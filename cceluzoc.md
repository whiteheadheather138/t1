代发 wailian999

TS:   new Date("2024-01-02")
来源：http://ass.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ugh.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tdn.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://flq.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://puk.yuxming.cn

[J04] 时间戳与日期互转
来源：http://gfe.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://khn.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://auk.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ztd.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ylv.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bho.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uqs.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://slk.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tnx.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://omp.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://sgv.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yqd.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bma.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nud.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://wdy.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dbi.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://eqz.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ggp.fzhhl.top

[J06] 计算两时间之差
来源：http://oau.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://kbv.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://jyp.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ofj.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qpl.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://mle.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://sfq.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://hob.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://lzc.uphjek.com

[J07] 比较两个日期
来源：http://sif.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://tag.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iuv.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://zat.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ptp.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fuv.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ntc.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qvg.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://jhy.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://wjp.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://huw.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vca.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgu.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nze.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mdm.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dez.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://stg.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fwx.fzhhl.top

[J09] 时区处理
来源：http://vet.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vzv.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ydx.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mgz.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sje.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xbf.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tue.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qiy.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://njt.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://wvk.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bnn.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://som.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xrv.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ref.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tel.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xmm.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jmn.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zkq.quarkkingdee.top

================================================================================
来源：http://xlo.tanke756.top

K. JSON 与序列化
来源：http://xdu.feifeiyinyue.top

================================================================================
来源：http://itc.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://sdp.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bqs.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ooy.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://qxc.yj202588.top

TS:   JSON.stringify(obj)
来源：http://xpc.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iov.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://bzm.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://prq.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qpi.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://xqp.nwbrower.top

Py:   json.loads(s)
来源：http://qbr.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jon.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://uuc.redwolf501.top

TS:   JSON.parse(s)
来源：http://gqa.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kbv.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://yhm.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://sgx.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tzk.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://sfr.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cln.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yij.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://rpc.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://fcd.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wak.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pbr.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://nfn.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nix.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://esb.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tou.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://son.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wst.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fdu.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rdy.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://avr.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://txb.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rts.tanke756.top

[K05] 深拷贝对象
来源：http://sed.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://ahg.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://ust.ybcxt.top

JS:   structuredClone(obj)
来源：http://twl.yangfankeji.com

TS:   structuredClone(obj)
来源：http://ebr.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xpu.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://noy.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://snf.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cbb.cashguo.top

[K06] 解析 URL 查询串
来源：http://rlj.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://chh.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dto.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cqj.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pdj.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://noq.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bgo.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wtv.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://laq.cdnleiting.top

[K07] 进制转换
来源：http://tly.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zmv.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bih.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rns.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nqi.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ohq.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pdl.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://psr.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://abv.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://wdu.havefunace.top

Py:   pickle.dumps(obj)
来源：http://iyz.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zup.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://ueu.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://sqk.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gkc.yj20258888.top

Go:   encoding/gob
来源：http://qwc.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://bmg.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qlv.ydzc1.top

================================================================================
来源：http://bny.zhongyouzk.top

L. 网络请求
来源：http://jxo.guowangkeji.top

================================================================================
来源：http://ypc.ydzc1.top

[L01] 发送 GET 请求
来源：http://ypr.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iiu.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cta.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://hbw.andypj.xyz

TS:   await fetch(url)
来源：http://teb.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rmd.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://xmq.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ksm.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vse.yvedp.cn

[L02] 发送 POST JSON
来源：http://fqg.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mks.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tbt.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mhb.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ydl.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pbq.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qwq.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://snx.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cng.ppjwa.cn

[L03] 设置自定义请求头
来源：http://gfc.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uzx.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pjq.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irt.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gak.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vcq.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ihq.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://huk.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qxq.fehbvm.com

[L04] 设置超时
来源：http://uzj.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://cgp.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://src.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xaa.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aes.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://taf.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ncq.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gek.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bmg.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://uph.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uca.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ulp.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ecg.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jex.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nbb.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://phi.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://prz.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ura.yvedp.cn

[L06] 解析响应为 JSON
来源：http://hag.fengsongda.top

Py:   resp.json()
来源：http://yqy.gotoacloud.top

PHP:  json_decode($body, true);
来源：http://pba.jinqigfzy.top

JS:   await resp.json()
来源：http://djs.yonumen.top

TS:   await resp.json()
来源：http://vnm.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dlc.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ysq.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://hpg.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rvt.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://vfs.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lji.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uqx.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://zaj.cashguo.top

TS:   resp.ok;  resp.status
来源：http://uwg.hnxiangtu.top

Java: resp.statusCode()
来源：http://ffe.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://orc.tianlin.xyz

Ruby: resp.code.to_i
来源：http://xqf.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://npw.snrcjt.cn

[L08] 并发请求多个地址
来源：http://pvv.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gjr.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://nsw.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uww.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzf.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vce.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vlc.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wqa.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zwb.ywan-chungtsiang.top

================================================================================
来源：http://cee.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://rth.andypj.xyz

================================================================================
来源：http://spr.cashguo.top

[M01] 读取命令行参数
来源：http://bqf.tarul.cn

Py:   sys.argv[1:]
来源：http://ymg.yonumen.top

PHP:  $argv;  $argc;
来源：http://iwn.fehbvm.com

JS:   process.argv.slice(2)
来源：http://oqk.uphjek.com

TS:   process.argv.slice(2)
来源：http://gzy.meibo888.top

Java: args 数组（main 方法参数）
来源：http://int.yueranfly.top

Go:   os.Args[1:]
来源：http://oxh.shanyushiyangkeji.top

Ruby: ARGV
来源：http://oim.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://wwu.hnqzz.top

[M02] 读取环境变量
来源：http://zds.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://pxg.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ygg.xuetiantiany.cn

JS:   process.env.HOME
来源：http://fad.sweek.top

TS:   process.env.HOME
来源：http://rwk.daria6918.cn

Java: System.getenv("HOME")
来源：http://jkn.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mtl.guannengcc.top

Ruby: ENV["HOME"]
来源：http://ccd.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wcv.ivvv.top

[M03] 执行外部命令
来源：http://chs.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xjs.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://htt.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://def.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://czm.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bdp.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vpk.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ehr.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://vww.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://ilm.guowangkeji.top

Py:   os.getcwd()
来源：http://pdb.cheryme.top

PHP:  getcwd();
来源：http://dud.hywenlv.cn

JS:   process.cwd()
来源：http://ars.fengsongda.top

TS:   process.cwd()
来源：http://wsm.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://gzv.cashguo.top

Go:   os.Getwd()
来源：http://afk.snrcjt.cn

Ruby: Dir.pwd
来源：http://xic.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qkx.hfpthk.cn

[M05] 设置退出码
来源：http://vui.0kj1m.cn

Py:   sys.exit(1)
来源：http://mfd.hongshengwenyu.top

PHP:  exit(1);
来源：http://qxv.cdnleiting.top

JS:   process.exit(1)
来源：http://pjl.iojbl.cn

TS:   process.exit(1)
来源：http://dgd.yj20258888.top

Java: System.exit(1)
来源：http://qwf.tianlin.xyz

Go:   os.Exit(1)
来源：http://vow.pycfn.com

Ruby: exit 1
来源：http://tpz.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qph.gzhubu.top

[M06] 向标准错误输出
来源：http://lrt.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://ixo.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ffd.fktsv.cn

JS:   console.error("err")
来源：http://hqb.chenjidiqi.icu

TS:   console.error("err")
来源：http://gck.yj202588.top

Java: System.err.println("err")
来源：http://mhg.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vxa.yj20258888.top

Ruby: warn "err"
来源：http://icn.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://lyn.316326.xyz

[M07] 判断是否为主入口
来源：http://ooe.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://obl.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jfl.hfpthk.cn

JS:   require.main === module
来源：http://zku.hfpthk.cn

TS:   require.main === module
来源：http://axc.hnqzz.top

Java: public static void main(String[] args)
来源：http://kxc.svipenyu.cn

Go:   func main()
来源：http://giq.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jpo.vehdjk.com

C#:   static void Main(string[] args)
来源：http://xtg.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://cab.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://sml.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://mkf.ydzc1.top

JS:   process.platform;  process.version
来源：http://tsz.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://lkb.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://onl.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://gmb.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://alv.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ryj.havefunace.top

================================================================================
来源：http://uah.gogol.net.cn

N. 数据结构与算法
来源：http://kfx.pengpengdd.cyou

================================================================================
来源：http://klp.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://cov.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://qhc.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://swd.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sxd.shangyingyoupin.top


<!-- 参考信息 -->