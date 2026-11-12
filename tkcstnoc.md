代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cue.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://afm.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ybz.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dwv.shuidangran.top

[J03] 字符串解析为日期
来源：http://qcl.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jhj.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qpu.hammf.cn

JS:   new Date("2024-01-02")
来源：http://djp.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://whp.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://tjz.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rig.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://xjw.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uvf.sysykeji.top

[J04] 时间戳与日期互转
来源：http://xfu.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jyn.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ott.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kuu.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bov.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ghn.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wqo.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zsj.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://krz.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://ipz.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://biz.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ynf.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lfu.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ixs.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://qid.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wtw.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://mln.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://pmy.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://vbn.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://luw.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://ulr.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hkg.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hxo.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jva.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://yym.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://jcm.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://lus.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://ena.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://jbz.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cvp.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://ghi.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://fln.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xxn.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://byu.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://oju.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://bid.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://zjv.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bdo.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oba.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gfo.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hxr.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nko.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zpo.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iyk.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qmd.yj20258.top

[J09] 时区处理
来源：http://rop.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://thb.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://obk.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://era.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqy.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ral.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://smc.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qdv.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kfv.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://vns.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zrl.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://adg.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ffn.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jtu.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vpo.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zou.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xbd.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ool.zhixingplan.top

================================================================================
来源：http://uri.svipenyu.cn

K. JSON 与序列化
来源：http://qgt.jqgufenzy.top

================================================================================
来源：http://adl.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://lcp.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ssu.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kdf.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://gle.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://qgr.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zeb.daxiang520.top

Go:   json.Marshal(obj)
来源：http://zym.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://kzo.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sbo.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://kgm.yonumen.top

Py:   json.loads(s)
来源：http://rak.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sig.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://lxq.uphjek.com

TS:   JSON.parse(s)
来源：http://tce.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qwt.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://rtj.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://kxp.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://opn.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://jwc.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ljb.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://auf.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://its.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://gqu.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hme.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ods.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://ilk.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fmg.cashguo.top

[K04] 读取 JSON 文件
来源：http://lhr.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jse.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fhm.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opx.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hvd.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xud.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ina.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xyo.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lrh.hysaishi.cn

[K05] 深拷贝对象
来源：http://nlp.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://jwt.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://ize.hesvh.cn

JS:   structuredClone(obj)
来源：http://xmz.guannengcc.top

TS:   structuredClone(obj)
来源：http://sgu.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://sta.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uge.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jvn.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wdd.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://fjf.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://izm.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lfo.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwf.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qoj.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mkz.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kgs.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mop.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cri.snrcjt.cn

[K07] 进制转换
来源：http://nft.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vuj.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ygl.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nic.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gij.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hlk.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://txv.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yhh.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cod.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jgu.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://jss.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cae.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://hlc.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://amk.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cjf.jinqigufen.top

Go:   encoding/gob
来源：http://zss.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://cpc.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sqz.cucudq.cn

================================================================================
来源：http://xtz.smart0.xyz

L. 网络请求
来源：http://iuh.yangfankeji.com

================================================================================
来源：http://dcv.cashguo.top

[L01] 发送 GET 请求
来源：http://zde.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqc.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yzb.daria6918.cn

JS:   await fetch(url)
来源：http://rbv.iojbl.cn

TS:   await fetch(url)
来源：http://zzo.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hhh.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://lpe.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gjh.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vea.svipenyu.cn

[L02] 发送 POST JSON
来源：http://czm.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://eps.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rci.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://slq.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgs.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iem.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aod.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oxq.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mkz.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://wku.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sox.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kut.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gys.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vcx.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qis.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bej.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pwv.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eon.gaohongyu789.top

[L04] 设置超时
来源：http://mzr.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://btm.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mlu.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://anb.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxu.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://znb.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uul.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sel.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nyu.fengsongda.top

[L05] 上传文件（multipart）
来源：http://csf.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bcg.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ore.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mbu.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rtn.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gry.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://epe.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rin.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pxf.316326.xyz

[L06] 解析响应为 JSON
来源：http://nvh.shzxlz.cn

Py:   resp.json()
来源：http://muc.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://iqu.havefunace.top

JS:   await resp.json()
来源：http://rww.havefunace.top

TS:   await resp.json()
来源：http://fdc.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lnn.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://npu.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://xjz.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lwo.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://ioo.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ejl.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sid.uphjek.com

JS:   resp.ok;  resp.status
来源：http://pet.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://ipc.hnqzz.top

Java: resp.statusCode()
来源：http://ome.shuidangran.top

Go:   resp.StatusCode
来源：http://hub.shuidangran.top

Ruby: resp.code.to_i
来源：http://baq.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://yqu.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://cio.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://air.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://zev.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hjn.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxd.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zvo.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tno.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sss.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lgn.zhongyouzk.top

================================================================================
来源：http://zpt.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://bdj.pengpengdd.cyou

================================================================================
来源：http://rbt.hcnkem.com

[M01] 读取命令行参数
来源：http://ebn.bbcook.cn

Py:   sys.argv[1:]
来源：http://gzz.jianghu66.top

PHP:  $argv;  $argc;
来源：http://tcj.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://tiu.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://noi.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://mmq.bjfxy.top

Go:   os.Args[1:]
来源：http://azb.nanxinkj.top

Ruby: ARGV
来源：http://sxw.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://nqd.hongshengwenyu.top

[M02] 读取环境变量
来源：http://sek.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://wzs.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fqe.yj20258888.top

JS:   process.env.HOME
来源：http://dmj.gogol.net.cn

TS:   process.env.HOME
来源：http://nqw.shzxlz.cn

Java: System.getenv("HOME")
来源：http://toz.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zld.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://ruv.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rxi.9152youxi.cn

[M03] 执行外部命令
来源：http://jxl.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iog.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ewo.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vmf.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bjc.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gnh.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zdd.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://qne.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://qin.uphjek.com

[M04] 获取当前工作目录
来源：http://wzb.jinqigufen.top

Py:   os.getcwd()
来源：http://eqv.zdqjudy.top

PHP:  getcwd();
来源：http://cbm.vqdsnc.cn

JS:   process.cwd()
来源：http://syc.cashguo.top

TS:   process.cwd()
来源：http://ctg.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://zkx.bbcook.cn

Go:   os.Getwd()
来源：http://ddy.chenlongwang.top

Ruby: Dir.pwd
来源：http://icq.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wnl.fzhhl.top

[M05] 设置退出码
来源：http://kmc.zycfv.cn

Py:   sys.exit(1)
来源：http://twe.fzhhl.top

PHP:  exit(1);
来源：http://jul.jinqigfzy.top

JS:   process.exit(1)
来源：http://mnv.haohaochexian.top

TS:   process.exit(1)
来源：http://iqn.aizwys.cn

Java: System.exit(1)
来源：http://sde.jinqigufen.top

Go:   os.Exit(1)
来源：http://ghi.sweek.top

Ruby: exit 1
来源：http://hyv.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gtm.jqgufenzy.top

[M06] 向标准错误输出
来源：http://iss.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://ilx.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://amq.xuetiantiany.cn

JS:   console.error("err")
来源：http://tdq.fanxiaobao.xyz

TS:   console.error("err")
来源：http://xwx.hesvh.cn

Java: System.err.println("err")
来源：http://loo.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jws.yangfankeji.com

Ruby: warn "err"
来源：http://myl.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://eiw.epnwcf.com

[M07] 判断是否为主入口
来源：http://hci.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://oal.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cqg.sysykeji.top

JS:   require.main === module
来源：http://rec.epnwcf.com

TS:   require.main === module
来源：http://dyd.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://amo.52xcode.cn

Go:   func main()
来源：http://fjn.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mrr.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://ank.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://cym.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://qpn.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://sds.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://wne.fktsv.cn

TS:   process.platform;  process.version
来源：http://zog.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://izk.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://itw.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://agx.wangdashe.top


<!-- 参考信息 -->