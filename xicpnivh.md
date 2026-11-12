代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wql.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jrw.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qjc.dashuyun.cn

TS:   d.toISOString()
来源：http://ubb.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lhv.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jwk.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://are.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oax.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://eae.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zmc.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yns.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://jel.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://ass.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zhl.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xgo.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://yrd.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yrl.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://vev.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://axe.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ydo.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gex.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ohy.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fiq.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hrx.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xyw.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bbe.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://nje.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://epm.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dya.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kvb.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxo.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://yxp.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hpl.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://uug.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://qvj.redwolf501.top

[J06] 计算两时间之差
来源：http://qoc.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://wgh.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://bpq.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iwh.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bbd.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://uat.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://eby.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://cgo.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://xmj.xziqi.cn

[J07] 比较两个日期
来源：http://bks.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://pwl.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yyf.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://vja.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://ygv.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sru.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kdn.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://btr.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://xkn.yongpay.top

[J08] 提取年月日与星期
来源：http://hxd.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://asy.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hmj.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yoi.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zzo.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iib.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fvw.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nny.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dil.jianghu66.top

[J09] 时区处理
来源：http://cxi.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xox.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lqb.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozw.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ufa.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zma.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qph.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cfh.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jyi.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://wdy.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uog.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mao.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gnw.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ver.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fyn.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hyv.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bzt.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ufj.aizwys.cn

================================================================================
来源：http://ydl.wangdashe.top

K. JSON 与序列化
来源：http://wjm.zhijiandao.cn

================================================================================
来源：http://hqe.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://mjk.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fxb.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zsj.yj202588.top

JS:   JSON.stringify(obj)
来源：http://qdp.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://diu.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cin.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://itp.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://pil.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hcw.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://kmo.gzhubu.top

Py:   json.loads(s)
来源：http://dsh.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://omf.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://xsm.birdmap.top

TS:   JSON.parse(s)
来源：http://wfq.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dax.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://atr.wangdashe.top

Ruby: JSON.parse(s)
来源：http://eog.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pst.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://hau.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dxk.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://juu.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://xsh.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nlq.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jan.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mme.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ark.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xqp.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://jno.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eia.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://agf.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aen.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://abc.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vlz.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yqr.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cza.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ezu.52xcode.cn

[K05] 深拷贝对象
来源：http://bhi.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://khx.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://xbv.fehbvm.com

JS:   structuredClone(obj)
来源：http://sei.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://zhd.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://vhe.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://itm.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dng.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gtq.tian-w.cn

[K06] 解析 URL 查询串
来源：http://zyv.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gzl.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hux.yueranfly.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lta.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lmr.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kak.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vap.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mlh.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bpp.jinqigufen.top

[K07] 进制转换
来源：http://vpr.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mtb.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lil.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aif.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://etw.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gua.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lrc.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hva.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fvg.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://ovh.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://sfm.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dmj.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://hxd.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://psl.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rau.xuanzx.com

Go:   encoding/gob
来源：http://jek.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://tnw.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xsf.yj202588.top

================================================================================
来源：http://tbl.vqdsnc.cn

L. 网络请求
来源：http://yxu.c1oappe.top

================================================================================
来源：http://nxs.ivvv.top

[L01] 发送 GET 请求
来源：http://fpy.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uuu.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xrw.sufxvd.cn

JS:   await fetch(url)
来源：http://gny.shuidangran.top

TS:   await fetch(url)
来源：http://fbm.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbp.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://ydx.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tua.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oyt.shzxlz.cn

[L02] 发送 POST JSON
来源：http://wty.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://ubm.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fkp.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eac.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://muv.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sar.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zbn.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nwt.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vzc.hcnkem.com

[L03] 设置自定义请求头
来源：http://ito.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wuy.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mud.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://woz.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cpg.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ost.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yec.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zja.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zze.shuidangran.top

[L04] 设置超时
来源：http://tli.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://xef.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mnv.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ben.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mdw.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vne.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://szx.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lds.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qxu.meibo888.top

[L05] 上传文件（multipart）
来源：http://fjl.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pts.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mqr.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tjk.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kdo.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xjg.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://amj.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xhy.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lci.daria6918.cn

[L06] 解析响应为 JSON
来源：http://npd.quarkkingdee.top

Py:   resp.json()
来源：http://ejh.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://sgp.shangyingyoupin.top

JS:   await resp.json()
来源：http://sgw.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://vwy.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cjg.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gbl.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://tkk.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mtn.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://wba.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qrp.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pug.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://eqq.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://znb.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://tnc.epnwcf.com

Go:   resp.StatusCode
来源：http://lcx.nanxinkj.top

Ruby: resp.code.to_i
来源：http://edm.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://rdw.jiagoushi.top

[L08] 并发请求多个地址
来源：http://jqt.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ueh.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://ukn.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyk.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wku.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bmq.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mvo.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ejt.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lrl.zhoulong.xyz

================================================================================
来源：http://jrl.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://lmz.sweek.top

================================================================================
来源：http://hzw.quarkkingdee.top

[M01] 读取命令行参数
来源：http://rkv.fengsongda.top

Py:   sys.argv[1:]
来源：http://aab.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://aig.bbcook.cn

JS:   process.argv.slice(2)
来源：http://aba.aizwys.cn

TS:   process.argv.slice(2)
来源：http://xcq.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://wwc.daria6918.cn

Go:   os.Args[1:]
来源：http://vro.hcnkem.com

Ruby: ARGV
来源：http://kjw.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://ntg.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://vgg.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://edu.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pim.xuetiantiany.cn

JS:   process.env.HOME
来源：http://dms.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://zrt.yongpay.top

Java: System.getenv("HOME")
来源：http://xnw.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wtg.cucudq.cn

Ruby: ENV["HOME"]
来源：http://wzs.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fup.mhx1999.top

[M03] 执行外部命令
来源：http://cho.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://upc.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zao.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kic.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ioc.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ebh.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://wvd.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://gyf.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://tns.bjfxy.top

[M04] 获取当前工作目录
来源：http://nwl.chenzaomai.com

Py:   os.getcwd()
来源：http://kib.dashuyun.cn

PHP:  getcwd();
来源：http://gid.yuxming.cn

JS:   process.cwd()
来源：http://zsg.dashuyun.cn

TS:   process.cwd()
来源：http://tnb.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://ajv.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://dcz.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://opa.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://awn.hongshengwenyu.top

[M05] 设置退出码
来源：http://hvq.sweek.top

Py:   sys.exit(1)
来源：http://wsh.wangdashe.top

PHP:  exit(1);
来源：http://pyu.yj20258888.top

JS:   process.exit(1)
来源：http://elf.jqgufenzy.top

TS:   process.exit(1)
来源：http://jpo.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://ara.zycfv.cn

Go:   os.Exit(1)
来源：http://blw.cdnleiting.top

Ruby: exit 1
来源：http://vbp.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tce.chenzaomai.com

[M06] 向标准错误输出
来源：http://udw.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://ctm.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aje.sweek.top

JS:   console.error("err")
来源：http://fxb.zycfv.cn

TS:   console.error("err")
来源：http://nsi.haohaochexian.top

Java: System.err.println("err")
来源：http://pni.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ade.jqgufenzy.top

Ruby: warn "err"
来源：http://vex.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://row.fengsongda.top

[M07] 判断是否为主入口
来源：http://tph.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://wgu.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zks.iojbl.cn

JS:   require.main === module
来源：http://sbq.gotoacloud.top

TS:   require.main === module
来源：http://ccx.jyoumei.cn

Java: public static void main(String[] args)
来源：http://vzr.xuetiantiany.cn

Go:   func main()
来源：http://mxy.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xtv.tanke756.top

C#:   static void Main(string[] args)
来源：http://nmm.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://nxz.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://rxl.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://ttw.ivvv.top

JS:   process.platform;  process.version
来源：http://nxy.xylfe.cn


<!-- 参考信息 -->