代发 wailian999

[J03] 字符串解析为日期
来源：http://ozr.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lqp.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gdj.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://zhu.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://yrq.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://xis.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://twl.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://nsn.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fnr.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://ocr.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oiy.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nin.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zmp.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vne.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tnn.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rxi.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tpp.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://scy.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://iui.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://lgo.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rjp.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://swu.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ecd.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://yxg.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vcu.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://zwn.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://dpz.gaohongyu789.top

[J06] 计算两时间之差
来源：http://fft.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://rzn.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://cya.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hlq.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ztc.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cre.fzhhl.top

Go:   end.Sub(start).Hours()
来源：http://szu.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://wmk.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://lbu.sweek.top

[J07] 比较两个日期
来源：http://qve.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://wpy.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://avf.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uji.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://aff.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rqp.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://afv.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://dwj.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://hju.xylfe.cn

[J08] 提取年月日与星期
来源：http://yyv.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hjg.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qgu.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://smj.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eqs.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bbq.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wwg.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pqv.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ihq.yuxming.cn

[J09] 时区处理
来源：http://fey.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xbn.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://guw.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjz.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lub.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jkt.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://slc.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pum.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cxd.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://tma.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://who.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zpp.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wrm.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://afh.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://idh.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rhg.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://crx.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tvv.dianchejie.cn

================================================================================
来源：http://fgp.guowangkeji.top

K. JSON 与序列化
来源：http://gmh.fanxiaobao.xyz

================================================================================
来源：http://col.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://iau.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mam.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bdn.cashguo.top

JS:   JSON.stringify(obj)
来源：http://fed.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://pgk.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jpy.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://fxa.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://pdj.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tnl.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://lww.smart0.xyz

Py:   json.loads(s)
来源：http://hmi.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yct.dianchejie.cn

JS:   JSON.parse(s)
来源：http://kya.havefunace.top

TS:   JSON.parse(s)
来源：http://phv.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bdm.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://sxs.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://ilo.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nnp.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://vpz.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oqg.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://paz.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ewp.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oiq.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xsq.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ozh.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://ddb.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ztu.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://qob.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kzf.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aog.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gnh.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bvm.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gxl.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lqn.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mnn.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vzn.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://gim.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://ccq.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://nko.cheryme.top

JS:   structuredClone(obj)
来源：http://vfh.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://uef.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uel.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sjy.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kec.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://iyq.sysykeji.top

[K06] 解析 URL 查询串
来源：http://yye.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kpj.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zvc.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pex.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ztz.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rfw.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://fjq.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mtu.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fvp.wangshuangyany.cn

[K07] 进制转换
来源：http://stt.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ftl.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oqk.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rph.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iwk.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxq.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tey.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bvr.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zmk.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://vhv.birdmap.top

Py:   pickle.dumps(obj)
来源：http://gge.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tfd.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://sfs.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://zsf.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wtm.zhoulong.xyz

Go:   encoding/gob
来源：http://tgo.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://yoj.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hck.cdnleiting.top

================================================================================
来源：http://zke.jinyuanbaomall.cn

L. 网络请求
来源：http://ecn.hfpthk.cn

================================================================================
来源：http://dgo.cheryme.top

[L01] 发送 GET 请求
来源：http://stb.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bnl.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wqn.hcnkem.com

JS:   await fetch(url)
来源：http://zpt.hongshengwenyu.top

TS:   await fetch(url)
来源：http://jqi.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eni.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://pzc.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eqv.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://voy.xinyue.icu

[L02] 发送 POST JSON
来源：http://izf.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://cau.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://czw.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yus.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isg.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vrk.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fkc.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://srj.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://awq.ppjwa.cn

[L03] 设置自定义请求头
来源：http://fbu.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://srt.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xkm.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xqb.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sro.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://esq.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hsy.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ger.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rdy.0kj1m.cn

[L04] 设置超时
来源：http://jyg.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://muc.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hbo.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mkr.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmy.feifeiyinyue.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lsb.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vow.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rqz.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hhf.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://uzl.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nob.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hld.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gkk.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://krf.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dpz.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twp.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vci.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zzn.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://dxz.hysaishi.cn

Py:   resp.json()
来源：http://mwi.bbcook.cn

PHP:  json_decode($body, true);
来源：http://cne.daxiang520.top

JS:   await resp.json()
来源：http://alm.shuidangran.top

TS:   await resp.json()
来源：http://hxz.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ivh.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://myr.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://waz.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blh.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://bsv.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xma.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dtm.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://hjs.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://lla.bbcook.cn

Java: resp.statusCode()
来源：http://epi.birdmap.top

Go:   resp.StatusCode
来源：http://hhx.tarul.cn

Ruby: resp.code.to_i
来源：http://yjp.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://pdc.gotoacloud.top

[L08] 并发请求多个地址
来源：http://fyz.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fjj.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://sdm.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjs.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qoe.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fwd.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lob.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nwe.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jqz.yj20258888.top

================================================================================
来源：http://jup.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://mxi.cashguo.top

================================================================================
来源：http://wlp.yangfankeji.com

[M01] 读取命令行参数
来源：http://sdv.aibaodan.cn

Py:   sys.argv[1:]
来源：http://cvj.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://ghk.yfazqb.com

JS:   process.argv.slice(2)
来源：http://lkl.xylfe.cn

TS:   process.argv.slice(2)
来源：http://ssv.uphjek.com

Java: args 数组（main 方法参数）
来源：http://jyt.aibaodan.cn

Go:   os.Args[1:]
来源：http://wis.sxryk.cn

Ruby: ARGV
来源：http://kwq.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://ptz.snrcjt.cn

[M02] 读取环境变量
来源：http://rfn.meibo888.top

Py:   os.environ.get("HOME")
来源：http://rnk.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vtw.sjlbkw.cn

JS:   process.env.HOME
来源：http://xju.chenjidiqi.icu

TS:   process.env.HOME
来源：http://wvy.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://jle.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pyw.hesvh.cn

Ruby: ENV["HOME"]
来源：http://jua.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://srw.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://acs.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aas.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ged.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gcr.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rne.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ydr.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rfl.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://dtm.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://eht.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://iwp.cucudq.cn

Py:   os.getcwd()
来源：http://abr.nanxuanxn.top

PHP:  getcwd();
来源：http://eue.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://nzc.hnxiangtu.top

TS:   process.cwd()
来源：http://xvy.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://fgu.dashuyun.cn

Go:   os.Getwd()
来源：http://xdl.guannengcc.top

Ruby: Dir.pwd
来源：http://bqh.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://tft.iojbl.cn

[M05] 设置退出码
来源：http://bxx.redwolf501.top

Py:   sys.exit(1)
来源：http://ovn.redwolf501.top

PHP:  exit(1);
来源：http://afz.chenzaomai.com

JS:   process.exit(1)
来源：http://geq.yj20258888.top

TS:   process.exit(1)
来源：http://ymi.ivvv.top

Java: System.exit(1)
来源：http://ytw.jianghu66.top

Go:   os.Exit(1)
来源：http://iuk.nwbrower.top

Ruby: exit 1
来源：http://num.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rgp.epnwcf.com

[M06] 向标准错误输出
来源：http://kch.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://hmm.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zfu.pycfn.com

JS:   console.error("err")
来源：http://fnl.ivvv.top

TS:   console.error("err")
来源：http://ety.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://pro.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bch.ppjwa.cn

Ruby: warn "err"
来源：http://vhz.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://fsi.jyoumei.cn

[M07] 判断是否为主入口
来源：http://xhk.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://nta.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dxo.xuanzx.com

JS:   require.main === module
来源：http://fez.xziqi.cn

TS:   require.main === module
来源：http://syy.ppjwa.cn

Java: public static void main(String[] args)
来源：http://yqd.tarul.cn

Go:   func main()
来源：http://hpj.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mcg.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://wrt.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://pez.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://yhk.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://xxw.shzxlz.cn

JS:   process.platform;  process.version
来源：http://rhc.bbcook.cn

TS:   process.platform;  process.version
来源：http://wtf.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qon.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qly.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nqp.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kys.zdqjudy.top

================================================================================
来源：http://abm.cheryme.top

N. 数据结构与算法
来源：http://nwr.fehbvm.com

================================================================================
来源：http://eds.sweek.top


<!-- 参考信息 -->