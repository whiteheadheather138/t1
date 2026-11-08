代发 wailian999

TS:   new Date("2024-01-02")
来源：https://jg.zhonguo5118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://sg.zhonguo8118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://iy.zhonguo2118.cn

Ruby: Date.parse("2024-01-02")
来源：https://as.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://lt.zhonguo6118.cn

[J04] 时间戳与日期互转
来源：https://zs.zhonguo2118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://vn.zhonguo4118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://br.zhonguo4118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://ll.zhonguo2118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://rr.zhonguo6118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://lr.zhonguo6118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://os.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://vz.zhonguo5118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ch.zhonguo2118.cn

[J05] 时间加减（加 7 天）
来源：https://id.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://yr.zhonguo7118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://ec.zhonguo8118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://vv.zhonguo6118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://kb.zhonguo5118.cn

Java: LocalDate.now().plusDays(7)
来源：https://rv.zhonguo3118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://vg.zhonguo7118.cn

Ruby: Time.now + 7 * 86400
来源：https://to.zhonguo5118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://vl.zhonguo2118.cn

[J06] 计算两时间之差
来源：https://ed.zhonguo4118.cn

Py:   (end - start).total_seconds()
来源：https://vs.zhonguo7118.cn

PHP:  $end->diff($start)->days;
来源：https://pi.zhonguo5118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://pj.zhonguo8118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://de.zhonguo1118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://et.zhonguo8118.cn

Go:   end.Sub(start).Hours()
来源：https://nl.zhonguo4118.cn

Ruby: end - start                 # 返回秒数
来源：https://sz.zhonguo8118.cn

C#:   (end - start).TotalSeconds
来源：https://ok.zhonguo7118.cn

[J07] 比较两个日期
来源：https://ws.zhonguo8118.cn

Py:   d1 < d2;  d1 == d2
来源：https://mn.zhonguo1118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://bc.zhonguo4118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://rj.zhonguo8118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://fi.zhonguo2118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://js.zhonguo1118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://qy.zhonguo7118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://ok.zhonguo2118.cn

C#:   d1 < d2;  d1 == d2
来源：https://ir.zhonguo1118.cn

[J08] 提取年月日与星期
来源：https://vp.zhonguo8118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://ej.zhonguo5118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://kj.zhonguo5118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://vn.zhonguo7118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://hb.zhonguo8118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://jj.zhonguo8118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://ix.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://dw.zhonguo6118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://dr.zhonguo5118.cn

[J09] 时区处理
来源：https://bb.zhonguo3118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://gx.zhonguo7118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://wg.zhonguo6118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://rh.zhonguo6118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://wz.zhonguo5118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://wv.zhonguo2118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://kd.zhonguo5118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://rd.zhonguo7118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://hu.zhonguo6118.cn

[J10] 取今天 / 本月第一天
来源：https://yl.zhonguo4118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ep.zhonguo1118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://kv.zhonguo5118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://mj.zhonguo5118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://mm.zhonguo5118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://kh.zhonguo7118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://sr.zhonguo1118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://gb.zhonguo7118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://pv.zhonguo5118.cn

================================================================================
来源：https://xc.zhonguo4118.cn

K. JSON 与序列化
来源：https://zd.zhonguo4118.cn

================================================================================
来源：https://ep.zhonguo8118.cn

[K01] 对象转 JSON 字符串
来源：https://xb.zhonguo6118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://vh.zhonguo6118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://fv.zhonguo3118.cn

JS:   JSON.stringify(obj)
来源：https://ei.zhonguo2118.cn

TS:   JSON.stringify(obj)
来源：https://hh.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://ho.zhonguo8118.cn

Go:   json.Marshal(obj)
来源：https://gl.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://yu.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://jx.zhonguo7118.cn

[K02] JSON 字符串转对象
来源：https://kn.zhonguo3118.cn

Py:   json.loads(s)
来源：https://xh.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://dt.zhonguo1118.cn

JS:   JSON.parse(s)
来源：https://bk.zhonguo5118.cn

TS:   JSON.parse(s)
来源：https://ei.zhonguo1118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://au.zhonguo7118.cn

Go:   json.Unmarshal(data, &v)
来源：https://sn.zhonguo3118.cn

Ruby: JSON.parse(s)
来源：https://vi.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://tw.zhonguo7118.cn

[K03] JSON 美化输出（带缩进）
来源：https://mg.zhonguo5118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://wn.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://de.zhonguo1118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://mx.zhonguo7118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://ms.zhonguo4118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://ab.zhonguo3118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://zy.zhonguo3118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://ea.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://od.zhonguo4118.cn

[K04] 读取 JSON 文件
来源：https://ak.zhonguo1118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://of.zhonguo7118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://fw.zhonguo1118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://sc.zhonguo1118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://vc.zhonguo3118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://lv.zhonguo1118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://kx.zhonguo5118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://tn.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://pm.zhonguo3118.cn

[K05] 深拷贝对象
来源：https://rm.zhonguo7118.cn

Py:   copy.deepcopy(obj)
来源：https://ja.zhonguo7118.cn

PHP:  unserialize(serialize($obj));
来源：https://xp.zhonguo5118.cn

JS:   structuredClone(obj)
来源：https://jd.zhonguo1118.cn

TS:   structuredClone(obj)
来源：https://qh.zhonguo2118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://mf.zhonguo6118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ul.zhonguo4118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://ua.zhonguo4118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://hl.zhonguo3118.cn

[K06] 解析 URL 查询串
来源：https://hc.zhonguo6118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://qe.zhonguo8118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://bf.zhonguo4118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://wy.zhonguo1118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://oi.zhonguo5118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://ad.zhonguo2118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://ct.zhonguo7118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://ti.zhonguo4118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://um.zhonguo1118.cn

[K07] 进制转换
来源：https://po.zhonguo7118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://qc.zhonguo4118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://ft.zhonguo7118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://xk.zhonguo5118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://oh.zhonguo6118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://wr.zhonguo8118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://se.zhonguo6118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://ix.zhonguo6118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://fr.zhonguo2118.cn

[K08] 二进制序列化（非 JSON）
来源：https://te.zhonguo3118.cn

Py:   pickle.dumps(obj)
来源：https://we.zhonguo3118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://gv.zhonguo6118.cn

JS:   v8.serialize(obj)        // Node
来源：https://bp.zhonguo4118.cn

TS:   v8.serialize(obj)        // Node
来源：https://hh.zhonguo2118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://br.zhonguo2118.cn

Go:   encoding/gob
来源：https://zq.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://je.zhonguo1118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://lg.zhonguo5118.cn

================================================================================
来源：https://yf.zhonguo6118.cn

L. 网络请求
来源：https://yk.zhonguo5118.cn

================================================================================
来源：https://ls.zhonguo1118.cn

[L01] 发送 GET 请求
来源：https://zv.zhonguo3118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://bt.zhonguo7118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://jf.zhonguo1118.cn

JS:   await fetch(url)
来源：https://ll.zhonguo7118.cn

TS:   await fetch(url)
来源：https://fl.zhonguo3118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://bh.zhonguo7118.cn

Go:   resp, err := http.Get(url)
来源：https://wx.zhonguo6118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://ef.zhonguo2118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://oe.zhonguo8118.cn

[L02] 发送 POST JSON
来源：https://ox.zhonguo4118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://cp.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://nb.zhonguo2118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://kb.zhonguo8118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://up.zhonguo6118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://ci.zhonguo3118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://hc.zhonguo3118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://rw.zhonguo3118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://mf.zhonguo3118.cn

[L03] 设置自定义请求头
来源：https://qg.zhonguo8118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://nf.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://gw.zhonguo3118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://oq.zhonguo6118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ax.zhonguo5118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://wz.zhonguo4118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://rg.zhonguo8118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://ao.zhonguo6118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://sd.zhonguo2118.cn

[L04] 设置超时
来源：https://jr.zhonguo6118.cn

Py:   requests.get(url, timeout=5)
来源：https://we.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://gb.zhonguo8118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://vc.zhonguo8118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://mr.zhonguo3118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://ex.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://tb.zhonguo7118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://hi.zhonguo5118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://ca.zhonguo4118.cn

[L05] 上传文件（multipart）
来源：https://hg.zhonguo3118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://gn.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://zc.zhonguo6118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://pl.zhonguo8118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://um.zhonguo5118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://vn.zhonguo2118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://fr.zhonguo6118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://fm.zhonguo2118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://hs.zhonguo7118.cn

[L06] 解析响应为 JSON
来源：https://ok.zhonguo3118.cn

Py:   resp.json()
来源：https://ux.zhonguo6118.cn

PHP:  json_decode($body, true);
来源：https://rf.zhonguo8118.cn

JS:   await resp.json()
来源：https://xu.zhonguo7118.cn

TS:   await resp.json()
来源：https://hn.zhonguo4118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://nh.zhonguo4118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://gu.zhonguo1118.cn

Ruby: JSON.parse(resp.body)
来源：https://wt.zhonguo1118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://xl.zhonguo1118.cn

[L07] 处理 HTTP 状态码
来源：https://fr.zhonguo7118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://wc.zhonguo1118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://ji.zhonguo3118.cn

JS:   resp.ok;  resp.status
来源：https://rc.zhonguo6118.cn

TS:   resp.ok;  resp.status
来源：https://rl.zhonguo4118.cn

Java: resp.statusCode()
来源：https://ee.zhonguo5118.cn

Go:   resp.StatusCode
来源：https://jp.zhonguo2118.cn

Ruby: resp.code.to_i
来源：https://xs.zhonguo1118.cn

C#:   (int)resp.StatusCode
来源：https://hh.zhonguo8118.cn

[L08] 并发请求多个地址
来源：https://jf.zhonguo2118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://mh.zhonguo6118.cn

PHP:  curl_multi_init() 系列
来源：https://hk.zhonguo7118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://xe.zhonguo1118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://oh.zhonguo4118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://jl.zhonguo3118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://dt.zhonguo6118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://jz.zhonguo4118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://qj.zhonguo6118.cn

================================================================================
来源：https://rr.zhonguo1118.cn

M. 命令行 / 进程 / 环境
来源：https://bh.zhonguo7118.cn

================================================================================
来源：https://sn.zhonguo7118.cn

[M01] 读取命令行参数
来源：https://ek.zhonguo1118.cn

Py:   sys.argv[1:]
来源：https://ak.zhonguo2118.cn

PHP:  $argv;  $argc;
来源：https://jw.zhonguo1118.cn

JS:   process.argv.slice(2)
来源：https://ef.zhonguo1118.cn

TS:   process.argv.slice(2)
来源：https://bn.zhonguo2118.cn

Java: args 数组（main 方法参数）
来源：https://ri.zhonguo7118.cn

Go:   os.Args[1:]
来源：https://qc.zhonguo6118.cn

Ruby: ARGV
来源：https://ok.zhonguo7118.cn

C#:   args 数组（Main 方法参数）
来源：https://bi.zhonguo8118.cn

[M02] 读取环境变量
来源：https://wr.zhonguo5118.cn

Py:   os.environ.get("HOME")
来源：https://ac.zhonguo7118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://ud.zhonguo6118.cn

JS:   process.env.HOME
来源：https://wx.zhonguo6118.cn

TS:   process.env.HOME
来源：https://jg.zhonguo2118.cn

Java: System.getenv("HOME")
来源：https://jf.zhonguo2118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://ze.zhonguo3118.cn

Ruby: ENV["HOME"]
来源：https://an.zhonguo7118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://ct.zhonguo4118.cn

[M03] 执行外部命令
来源：https://kx.zhonguo2118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://rj.zhonguo2118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://jq.zhonguo7118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://wq.zhonguo1118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://cy.zhonguo6118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://id.zhonguo1118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://wr.zhonguo3118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://ld.zhonguo2118.cn

C#:   Process.Start("ls", "-l");
来源：https://ww.zhonguo5118.cn

[M04] 获取当前工作目录
来源：https://qt.zhonguo8118.cn

Py:   os.getcwd()
来源：https://sr.zhonguo8118.cn

PHP:  getcwd();
来源：https://aq.zhonguo6118.cn

JS:   process.cwd()
来源：https://hy.zhonguo1118.cn

TS:   process.cwd()
来源：https://dm.zhonguo4118.cn

Java: Path.of("").toAbsolutePath()
来源：https://ty.zhonguo6118.cn

Go:   os.Getwd()
来源：https://qv.zhonguo7118.cn

Ruby: Dir.pwd
来源：https://ie.zhonguo2118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://rw.zhonguo6118.cn

[M05] 设置退出码
来源：https://ap.zhonguo4118.cn

Py:   sys.exit(1)
来源：https://yk.zhonguo7118.cn

PHP:  exit(1);
来源：https://qk.zhonguo6118.cn

JS:   process.exit(1)
来源：https://yb.zhonguo1118.cn

TS:   process.exit(1)
来源：https://fv.zhonguo1118.cn

Java: System.exit(1)
来源：https://nu.zhonguo2118.cn

Go:   os.Exit(1)
来源：https://je.zhonguo6118.cn

Ruby: exit 1
来源：https://vx.zhonguo5118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://ej.zhonguo6118.cn

[M06] 向标准错误输出
来源：https://uf.zhonguo2118.cn

Py:   print("err", file=sys.stderr)
来源：https://vw.zhonguo5118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://sq.zhonguo1118.cn

JS:   console.error("err")
来源：https://xq.zhonguo1118.cn

TS:   console.error("err")
来源：https://av.zhonguo1118.cn

Java: System.err.println("err")
来源：https://kc.zhonguo4118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://nw.zhonguo8118.cn

Ruby: warn "err"
来源：https://ts.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://qk.zhonguo2118.cn

[M07] 判断是否为主入口
来源：https://te.zhonguo3118.cn

Py:   if __name__ == "__main__":
来源：https://aj.zhonguo1118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://sg.zhonguo3118.cn

JS:   require.main === module
来源：https://mh.zhonguo4118.cn

TS:   require.main === module
来源：https://an.zhonguo8118.cn

Java: public static void main(String[] args)
来源：https://ad.zhonguo4118.cn

Go:   func main()
来源：https://uy.zhonguo5118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://mp.zhonguo8118.cn

C#:   static void Main(string[] args)
来源：https://gs.zhonguo3118.cn

[M08] 获取系统与运行时信息
来源：https://ar.zhonguo6118.cn

Py:   platform.system();  platform.python_version()
来源：https://vm.zhonguo3118.cn

PHP:  PHP_OS;  phpversion();
来源：https://ou.zhonguo8118.cn

JS:   process.platform;  process.version
来源：https://zd.zhonguo7118.cn

TS:   process.platform;  process.version
来源：https://qr.zhonguo3118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://hh.zhonguo2118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://gn.zhonguo3118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://ps.zhonguo8118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://du.zhonguo5118.cn

================================================================================
来源：https://ll.zhonguo7118.cn

N. 数据结构与算法
来源：https://hh.zhonguo2118.cn

================================================================================
来源：https://ac.zhonguo5118.cn

[N01] 二分查找（有序数组）
来源：https://ah.zhonguo6118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://zq.zhonguo8118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://et.zhonguo1118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://tj.zhonguo3118.cn


<!-- 参考信息 -->