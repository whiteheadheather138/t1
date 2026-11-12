代发 wailian999

TS:   new Date("2024-01-02")
来源：http://fbq.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://ywp.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://snf.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://lyj.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tbx.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://cjm.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ncf.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://smk.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://owd.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://syx.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ygv.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fev.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iyt.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vce.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://uxh.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://enu.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipi.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://meh.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xre.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://jcz.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jtp.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://qpk.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://elr.redwolf501.top

[J06] 计算两时间之差
来源：http://nyp.meibo888.top

Py:   (end - start).total_seconds()
来源：http://xod.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://zqb.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qrg.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zil.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://hak.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://yuk.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://dhm.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://nnd.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://sur.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://uuc.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vmm.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ntg.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://gqk.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lpp.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cxp.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://oic.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://srz.epnwcf.com

[J08] 提取年月日与星期
来源：http://dcc.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nxj.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mma.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ywz.zhoulong.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rvk.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aiw.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mbq.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rcx.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ooc.zdqjudy.top

[J09] 时区处理
来源：http://caq.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfr.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://znj.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tom.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eia.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whk.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://abs.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uvw.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://akr.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://kzt.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://kcp.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iiv.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rxb.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xdl.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mrc.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tyv.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vaq.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wxh.iojbl.cn

================================================================================
来源：http://voo.ydzc1.top

K. JSON 与序列化
来源：http://odk.yangfankeji.com

================================================================================
来源：http://xax.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://cfe.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://czj.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hvm.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://jcs.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://pkt.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://msi.mhx1999.top

Go:   json.Marshal(obj)
来源：http://cma.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://kuh.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ylt.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://lnt.cqqwz.cn

Py:   json.loads(s)
来源：http://szu.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hep.tian-w.cn

JS:   JSON.parse(s)
来源：http://rmr.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://xha.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fao.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://ukh.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://lpy.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fmk.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://mwh.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zkj.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gdf.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nnz.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://slr.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dxd.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://osz.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xcx.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bww.yvedp.cn

[K04] 读取 JSON 文件
来源：http://zga.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qtn.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jcx.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zaq.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://djg.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lcb.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ywf.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xbu.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://txh.zhongyouzk.top

[K05] 深拷贝对象
来源：http://bxk.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://klc.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://wxw.ehwqpu.com

JS:   structuredClone(obj)
来源：http://tma.yj20258888.top

TS:   structuredClone(obj)
来源：http://ofu.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gsd.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lty.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://juz.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aem.fktsv.cn

[K06] 解析 URL 查询串
来源：http://sjg.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fcs.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xqc.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://flq.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xxe.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxy.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cbp.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kym.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zft.9152youxi.cn

[K07] 进制转换
来源：http://yzm.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mmn.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cex.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xum.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vvy.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qei.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lms.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tzu.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gyz.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://ufe.birdmap.top

Py:   pickle.dumps(obj)
来源：http://tmk.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sys.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://rkr.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://ake.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ikg.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://mdr.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://uqu.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ubh.316326.xyz

================================================================================
来源：http://zpv.jinghuilouyu.cn

L. 网络请求
来源：http://nrh.zhiwuduotai.top

================================================================================
来源：http://qno.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://jbd.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dsu.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lan.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://mxf.yvedp.cn

TS:   await fetch(url)
来源：http://bkk.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gbo.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://qov.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://exx.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mav.yueranfly.top

[L02] 发送 POST JSON
来源：http://wde.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://rzm.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://scx.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://obq.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gku.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ykq.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hno.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bvk.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nno.cucudq.cn

[L03] 设置自定义请求头
来源：http://ajk.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ney.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rhh.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlt.tian-w.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://skr.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://weh.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ocm.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wmy.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uxo.svipenyu.cn

[L04] 设置超时
来源：http://cxd.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://doh.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kwh.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ajj.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rlz.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nxl.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yxg.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://faw.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yae.bbcook.cn

[L05] 上传文件（multipart）
来源：http://hqa.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ulj.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://frq.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://trn.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fqq.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mez.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tho.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ypx.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovb.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://lup.shanyushiyangtech.top

Py:   resp.json()
来源：http://kwu.xziqi.cn

PHP:  json_decode($body, true);
来源：http://fgx.hysaishi.cn

JS:   await resp.json()
来源：http://ffx.dashuyun.cn

TS:   await resp.json()
来源：http://htb.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ata.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ozz.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://cev.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kby.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://iqi.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ink.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iso.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://idr.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://wlj.yanxiufei.cn

Java: resp.statusCode()
来源：http://cdc.yj20258.top

Go:   resp.StatusCode
来源：http://dya.nanxinkj.top

Ruby: resp.code.to_i
来源：http://cjg.havefunace.top

C#:   (int)resp.StatusCode
来源：http://ctg.hcnkem.com

[L08] 并发请求多个地址
来源：http://inq.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pxx.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://yhq.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://abw.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://roa.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tpa.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wvr.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nln.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tsg.epnwcf.com

================================================================================
来源：http://nxp.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://okv.fehbvm.com

================================================================================
来源：http://xug.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://els.hcnkem.com

Py:   sys.argv[1:]
来源：http://xqd.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://tqc.cheryme.top

JS:   process.argv.slice(2)
来源：http://apj.uphjek.com

TS:   process.argv.slice(2)
来源：http://bqg.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://bpl.dashuyun.cn

Go:   os.Args[1:]
来源：http://vwi.jianghu66.top

Ruby: ARGV
来源：http://dwj.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://ydj.ybcxt.top

[M02] 读取环境变量
来源：http://pzc.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://cfo.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uji.uphjek.com

JS:   process.env.HOME
来源：http://hae.0kj1m.cn

TS:   process.env.HOME
来源：http://vbw.52xcode.cn

Java: System.getenv("HOME")
来源：http://ijl.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cmx.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://gog.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nag.tarul.cn

[M03] 执行外部命令
来源：http://iqw.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jji.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tqp.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mjv.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pqu.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ocs.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://onj.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://lke.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://opa.jianghu66.top

[M04] 获取当前工作目录
来源：http://vnj.hfpthk.cn

Py:   os.getcwd()
来源：http://dcd.guowangkeji.top

PHP:  getcwd();
来源：http://mgl.uphjek.com

JS:   process.cwd()
来源：http://upm.epnwcf.com

TS:   process.cwd()
来源：http://fvk.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://waq.ctjpmb.com

Go:   os.Getwd()
来源：http://ged.redwolf501.top

Ruby: Dir.pwd
来源：http://vfn.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://tmr.yongpay.top

[M05] 设置退出码
来源：http://tug.yj20258888.top

Py:   sys.exit(1)
来源：http://rbr.andypj.xyz

PHP:  exit(1);
来源：http://zxw.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://dku.quarkkingdee.top

TS:   process.exit(1)
来源：http://jlu.hcnkem.com

Java: System.exit(1)
来源：http://vnk.yuanzhike.top

Go:   os.Exit(1)
来源：http://mty.birdmap.top

Ruby: exit 1
来源：http://dys.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cgt.redwolf501.top

[M06] 向标准错误输出
来源：http://zxh.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://txz.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wtu.zhengqikj.top

JS:   console.error("err")
来源：http://vjv.zhijiandao.cn

TS:   console.error("err")
来源：http://ega.jlsjyb.cn

Java: System.err.println("err")
来源：http://uck.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://moa.zhongyouzk.top

Ruby: warn "err"
来源：http://lpo.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://fwg.andypj.xyz

[M07] 判断是否为主入口
来源：http://oct.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://poi.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zei.zhoulong.xyz

JS:   require.main === module
来源：http://lxr.dashuyun.cn

TS:   require.main === module
来源：http://edn.jiagoushi.top

Java: public static void main(String[] args)
来源：http://anw.chenjidiqi.icu

Go:   func main()
来源：http://jtg.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bbr.yj20258.top

C#:   static void Main(string[] args)
来源：http://ecc.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://mvd.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://pvb.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://cca.guannengcc.top

JS:   process.platform;  process.version
来源：http://fvy.sufxvd.cn

TS:   process.platform;  process.version
来源：http://kmo.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sxg.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nxk.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mtn.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uul.kuanghao11.cn

================================================================================
来源：http://qnx.meibo888.top

N. 数据结构与算法
来源：http://guf.fzhhl.top

================================================================================
来源：http://bqp.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://nsk.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dfs.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wnf.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ceu.guowangkeji.top


<!-- 参考信息 -->