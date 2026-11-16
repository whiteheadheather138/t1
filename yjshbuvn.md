代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqt.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nov.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sxo.meibo888.top

TS:   d.toISOString()
来源：http://vma.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jnh.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yrg.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vek.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xtf.fehbvm.com

[J03] 字符串解析为日期
来源：http://kwv.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nru.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vby.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://cej.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://wtu.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://twd.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ggw.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://qht.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gdc.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://qpu.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hjg.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://afh.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vny.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yth.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fyk.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ovb.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qzb.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kgd.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://jow.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://dqw.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xeb.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lsk.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvo.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://evv.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fjh.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://cvz.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yvz.c1oappe.top

[J06] 计算两时间之差
来源：http://vrz.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://env.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://huv.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jnh.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://upj.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://lvl.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://zlx.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://fip.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://yal.c1oappe.top

[J07] 比较两个日期
来源：http://urq.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://edu.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xlc.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://zsv.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://kvf.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ryx.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ydo.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://efp.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://xkw.tanke756.top

[J08] 提取年月日与星期
来源：http://oir.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ouw.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xmo.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kfp.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cbk.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gtj.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ljx.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbu.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://goz.sweek.top

[J09] 时区处理
来源：http://jhm.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qyf.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gnj.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cti.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tui.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://puf.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tst.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uoa.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bmz.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://ebd.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hqo.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fnb.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xig.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uja.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zzw.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://moi.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://juf.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dgj.hcnkem.com

================================================================================
来源：http://zhy.haohaochexian.top

K. JSON 与序列化
来源：http://kfp.hfpthk.cn

================================================================================
来源：http://hwz.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://zwy.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uik.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zdd.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://okp.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://zcc.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zoh.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://wmx.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wtc.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xny.cashguo.top

[K02] JSON 字符串转对象
来源：http://cwd.tian-w.cn

Py:   json.loads(s)
来源：http://aes.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gug.tanke756.top

JS:   JSON.parse(s)
来源：http://qfx.vehdjk.com

TS:   JSON.parse(s)
来源：http://njc.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lco.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://usq.wangdashe.top

Ruby: JSON.parse(s)
来源：http://nhb.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bht.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://zbh.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://teh.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://byg.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lmc.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nql.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qzy.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nwu.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://psy.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eli.aizwys.cn

[K04] 读取 JSON 文件
来源：http://nwy.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jht.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kev.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://equ.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fyz.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hxa.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hte.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nsp.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bro.zycfv.cn

[K05] 深拷贝对象
来源：http://yyn.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://bha.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://tbj.xinyue.icu

JS:   structuredClone(obj)
来源：http://hmp.jinqigufen.top

TS:   structuredClone(obj)
来源：http://dte.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rwi.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jpo.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrq.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dnx.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://lho.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://arc.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://err.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ayu.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hbb.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kbr.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://irl.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dvc.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cdb.snrcjt.cn

[K07] 进制转换
来源：http://udd.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://adl.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ynw.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fys.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://msb.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rsv.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zcu.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fgf.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xza.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://eax.meibo888.top

Py:   pickle.dumps(obj)
来源：http://res.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fpe.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://ezk.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://kxn.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mxh.pengpengdd.cyou

Go:   encoding/gob
来源：http://gdg.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://kld.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wqj.yj20258888.top

================================================================================
来源：http://fxb.tian-w.cn

L. 网络请求
来源：http://wox.hcnkem.com

================================================================================
来源：http://hvy.redwolf501.top

[L01] 发送 GET 请求
来源：http://jyy.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bch.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://abd.smart0.xyz

JS:   await fetch(url)
来源：http://nwt.jinqigufen.top

TS:   await fetch(url)
来源：http://tev.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mfg.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://gkc.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://obk.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vrr.tanke756.top

[L02] 发送 POST JSON
来源：http://akz.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://hpr.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cyg.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdq.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdq.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://idh.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mfz.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://atg.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qia.hnqzz.top

[L03] 设置自定义请求头
来源：http://wpv.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywu.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fwt.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qtf.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tar.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ddo.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rod.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rsc.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nrm.mhx1999.top

[L04] 设置超时
来源：http://eub.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://oma.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tdn.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://spj.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fcz.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://glb.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nek.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ffo.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://adl.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://oge.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qmc.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://olo.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qtw.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tnn.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dix.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yvl.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jzx.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jeu.nwbrower.top

[L06] 解析响应为 JSON
来源：http://fab.snrcjt.cn

Py:   resp.json()
来源：http://vul.cashguo.top

PHP:  json_decode($body, true);
来源：http://jcv.wangdashe.top

JS:   await resp.json()
来源：http://dub.yuxming.cn

TS:   await resp.json()
来源：http://bem.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mll.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xsq.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://oio.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vvu.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://piw.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://igt.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fmb.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://ynm.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://kun.nwbrower.top

Java: resp.statusCode()
来源：http://qjb.zhijiandao.cn

Go:   resp.StatusCode
来源：http://nbd.birdmap.top

Ruby: resp.code.to_i
来源：http://zrm.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://nzk.snrcjt.cn

[L08] 并发请求多个地址
来源：http://qnd.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dbd.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://bie.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yaq.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://slg.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tub.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://obf.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://thb.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ung.gotoacloud.top

================================================================================
来源：http://aaa.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://sfn.hywenlv.cn

================================================================================
来源：http://igc.zdbjq.cn

[M01] 读取命令行参数
来源：http://lkb.jqgfzy.top

Py:   sys.argv[1:]
来源：http://wqa.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://fee.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://bdq.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://zat.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://upb.gogol.net.cn

Go:   os.Args[1:]
来源：http://wye.bjfxy.top

Ruby: ARGV
来源：http://vgj.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://zai.tarul.cn

[M02] 读取环境变量
来源：http://rko.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://jxo.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sfu.jinqigufen.top

JS:   process.env.HOME
来源：http://whr.ybcxt.top

TS:   process.env.HOME
来源：http://obq.havefunace.top

Java: System.getenv("HOME")
来源：http://nwc.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ivx.guannengcc.top

Ruby: ENV["HOME"]
来源：http://yhf.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gwq.jqgufenzy.top

[M03] 执行外部命令
来源：http://oau.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oik.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kug.hysaishi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vyh.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yrj.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dso.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gdd.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://miz.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://cjq.xinyue.icu

[M04] 获取当前工作目录
来源：http://cuu.daxiang520.top

Py:   os.getcwd()
来源：http://xgi.vehdjk.com

PHP:  getcwd();
来源：http://ryl.316326.xyz

JS:   process.cwd()
来源：http://spj.yj202588.top

TS:   process.cwd()
来源：http://ryi.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://slf.xinyue.icu

Go:   os.Getwd()
来源：http://epf.sysykeji.top

Ruby: Dir.pwd
来源：http://lnu.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lpa.yonumen.top

[M05] 设置退出码
来源：http://vvg.cheryme.top

Py:   sys.exit(1)
来源：http://qdd.pycfn.com

PHP:  exit(1);
来源：http://ecl.sweek.top

JS:   process.exit(1)
来源：http://blj.jyoumei.cn

TS:   process.exit(1)
来源：http://seu.cqqwz.cn

Java: System.exit(1)
来源：http://tkv.hywenlv.cn

Go:   os.Exit(1)
来源：http://rcd.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://zth.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ous.tanke756.top

[M06] 向标准错误输出
来源：http://tip.yanxiufei.cn

Py:   print("err", file=sys.stderr)
来源：http://ifc.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xjg.zhengqikj.top

JS:   console.error("err")
来源：http://ajb.jyoumei.cn

TS:   console.error("err")
来源：http://ryi.vehdjk.com

Java: System.err.println("err")
来源：http://wij.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rcb.nanxinkj.top

Ruby: warn "err"
来源：http://zwi.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://kif.hnqzz.top

[M07] 判断是否为主入口
来源：http://ysj.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://jnz.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bvs.feifeiyinyue.top

JS:   require.main === module
来源：http://aid.nanxinkj.top

TS:   require.main === module
来源：http://efo.hysaishi.cn

Java: public static void main(String[] args)
来源：http://yqj.dashuyun.cn

Go:   func main()
来源：http://brr.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xtj.redwolf501.top

C#:   static void Main(string[] args)
来源：http://upp.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://wmp.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://ipm.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://vcu.fzhhl.top

JS:   process.platform;  process.version
来源：http://spc.vqdsnc.cn


<!-- 参考信息 -->