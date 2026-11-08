代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://ed.zhonguo1118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://lj.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://zg.zhonguo6118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ao.zhonguo5118.cn

[J03] 字符串解析为日期
来源：https://md.zhonguo2118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://gu.zhonguo7118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://dc.zhonguo1118.cn

JS:   new Date("2024-01-02")
来源：https://nd.zhonguo4118.cn

TS:   new Date("2024-01-02")
来源：https://jb.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://iy.zhonguo8118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://tg.zhonguo3118.cn

Ruby: Date.parse("2024-01-02")
来源：https://gb.zhonguo7118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://yb.zhonguo6118.cn

[J04] 时间戳与日期互转
来源：https://rl.zhonguo3118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://os.zhonguo2118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://de.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://zo.zhonguo1118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://gl.zhonguo1118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://ns.zhonguo7118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://oc.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://ll.zhonguo4118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://pk.zhonguo8118.cn

[J05] 时间加减（加 7 天）
来源：https://ch.zhonguo8118.cn

Py:   now + timedelta(days=7)
来源：https://el.zhonguo6118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://kq.zhonguo8118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://sn.zhonguo8118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://yv.zhonguo7118.cn

Java: LocalDate.now().plusDays(7)
来源：https://rj.zhonguo1118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://cf.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://kq.zhonguo1118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://ts.zhonguo3118.cn

[J06] 计算两时间之差
来源：https://gb.zhonguo4118.cn

Py:   (end - start).total_seconds()
来源：https://ro.zhonguo3118.cn

PHP:  $end->diff($start)->days;
来源：https://hr.zhonguo2118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://ru.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://ab.zhonguo8118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://cq.zhonguo4118.cn

Go:   end.Sub(start).Hours()
来源：https://wu.zhonguo7118.cn

Ruby: end - start                 # 返回秒数
来源：https://to.zhonguo7118.cn

C#:   (end - start).TotalSeconds
来源：https://cl.zhonguo1118.cn

[J07] 比较两个日期
来源：https://qw.zhonguo7118.cn

Py:   d1 < d2;  d1 == d2
来源：https://br.zhonguo3118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://uu.zhonguo5118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://jd.zhonguo2118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://ju.zhonguo5118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://yj.zhonguo5118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://yn.zhonguo8118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://fv.zhonguo2118.cn

C#:   d1 < d2;  d1 == d2
来源：https://cc.zhonguo8118.cn

[J08] 提取年月日与星期
来源：https://cz.zhonguo6118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://jm.zhonguo1118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://rd.zhonguo8118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://cd.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://xf.zhonguo5118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://qo.zhonguo1118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://xd.zhonguo3118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://gn.zhonguo2118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://go.zhonguo2118.cn

[J09] 时区处理
来源：https://rn.zhonguo7118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://hv.zhonguo4118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://vd.zhonguo6118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://db.zhonguo5118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ee.zhonguo8118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://sw.zhonguo7118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ud.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://ui.zhonguo1118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://ew.zhonguo6118.cn

[J10] 取今天 / 本月第一天
来源：https://na.zhonguo3118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://sd.zhonguo6118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://bf.zhonguo1118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://sj.zhonguo6118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://aw.zhonguo8118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://eb.zhonguo7118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://um.zhonguo8118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://ag.zhonguo4118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://hg.zhonguo5118.cn

================================================================================
来源：https://gk.zhonguo4118.cn

K. JSON 与序列化
来源：https://ij.zhonguo8118.cn

================================================================================
来源：https://si.zhonguo4118.cn

[K01] 对象转 JSON 字符串
来源：https://or.zhonguo4118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://pq.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://og.zhonguo2118.cn

JS:   JSON.stringify(obj)
来源：https://ew.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://he.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://nt.zhonguo2118.cn

Go:   json.Marshal(obj)
来源：https://zn.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://ms.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://zs.zhonguo3118.cn

[K02] JSON 字符串转对象
来源：https://mo.zhonguo4118.cn

Py:   json.loads(s)
来源：https://hv.zhonguo1118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://qc.zhonguo4118.cn

JS:   JSON.parse(s)
来源：https://qt.zhonguo8118.cn

TS:   JSON.parse(s)
来源：https://ii.zhonguo2118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://jp.zhonguo5118.cn

Go:   json.Unmarshal(data, &v)
来源：https://mi.zhonguo6118.cn

Ruby: JSON.parse(s)
来源：https://vh.zhonguo5118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://fk.zhonguo6118.cn

[K03] JSON 美化输出（带缩进）
来源：https://rd.zhonguo4118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://qy.zhonguo1118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://rk.zhonguo3118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://fy.zhonguo5118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://yx.zhonguo3118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://xw.zhonguo1118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://iu.zhonguo2118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://av.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://ca.zhonguo5118.cn

[K04] 读取 JSON 文件
来源：https://il.zhonguo4118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://ud.zhonguo8118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://lq.zhonguo8118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://xs.zhonguo3118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ha.zhonguo1118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://ou.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://cr.zhonguo6118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://po.zhonguo4118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://jl.zhonguo4118.cn

[K05] 深拷贝对象
来源：https://rq.zhonguo8118.cn

Py:   copy.deepcopy(obj)
来源：https://yk.zhonguo1118.cn

PHP:  unserialize(serialize($obj));
来源：https://hh.zhonguo6118.cn

JS:   structuredClone(obj)
来源：https://ix.zhonguo3118.cn

TS:   structuredClone(obj)
来源：https://sy.zhonguo7118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://xd.zhonguo3118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://wu.zhonguo8118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://yo.zhonguo5118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://nj.zhonguo4118.cn

[K06] 解析 URL 查询串
来源：https://er.zhonguo1118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://yo.zhonguo4118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://wb.zhonguo2118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://pg.zhonguo5118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://vd.zhonguo3118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://do.zhonguo1118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://rs.zhonguo3118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://hg.zhonguo3118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://sg.zhonguo7118.cn

[K07] 进制转换
来源：https://jb.zhonguo5118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://rm.zhonguo3118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://ra.zhonguo8118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://fj.zhonguo5118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://ur.zhonguo4118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://ld.zhonguo2118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://wt.zhonguo7118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://ic.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://el.zhonguo2118.cn

[K08] 二进制序列化（非 JSON）
来源：https://tm.zhonguo5118.cn

Py:   pickle.dumps(obj)
来源：https://dt.zhonguo7118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://uu.zhonguo1118.cn

JS:   v8.serialize(obj)        // Node
来源：https://sy.zhonguo5118.cn

TS:   v8.serialize(obj)        // Node
来源：https://va.zhonguo8118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://wf.zhonguo8118.cn

Go:   encoding/gob
来源：https://va.zhonguo1118.cn

Ruby: Marshal.dump(obj)
来源：https://lp.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://ns.zhonguo4118.cn

================================================================================
来源：https://jl.zhonguo8118.cn

L. 网络请求
来源：https://vv.zhonguo2118.cn

================================================================================
来源：https://dl.zhonguo2118.cn

[L01] 发送 GET 请求
来源：https://tl.zhonguo3118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://pb.zhonguo5118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://lu.zhonguo5118.cn

JS:   await fetch(url)
来源：https://xg.zhonguo5118.cn

TS:   await fetch(url)
来源：https://vw.zhonguo5118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://ul.zhonguo5118.cn

Go:   resp, err := http.Get(url)
来源：https://nm.zhonguo6118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://cm.zhonguo7118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://xf.zhonguo2118.cn

[L02] 发送 POST JSON
来源：https://dv.zhonguo4118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://kt.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://nz.zhonguo8118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://pj.zhonguo4118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://lg.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://nc.zhonguo7118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://jo.zhonguo7118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://zi.zhonguo6118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://ya.zhonguo6118.cn

[L03] 设置自定义请求头
来源：https://sd.zhonguo5118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://vd.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://he.zhonguo3118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://dd.zhonguo6118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ic.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://gm.zhonguo8118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://wn.zhonguo8118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://xh.zhonguo4118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://os.zhonguo3118.cn

[L04] 设置超时
来源：https://tq.zhonguo6118.cn

Py:   requests.get(url, timeout=5)
来源：https://ay.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://ig.zhonguo7118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://ms.zhonguo5118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://hq.zhonguo8118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://tx.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://sb.zhonguo4118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://eo.zhonguo8118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://bj.zhonguo6118.cn

[L05] 上传文件（multipart）
来源：https://mg.zhonguo4118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://to.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://gw.zhonguo1118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://gt.zhonguo4118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://mk.zhonguo3118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://gg.zhonguo2118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://cv.zhonguo5118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ti.zhonguo2118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://dp.zhonguo3118.cn

[L06] 解析响应为 JSON
来源：https://um.zhonguo8118.cn

Py:   resp.json()
来源：https://ar.zhonguo4118.cn

PHP:  json_decode($body, true);
来源：https://zj.zhonguo2118.cn

JS:   await resp.json()
来源：https://tj.zhonguo7118.cn

TS:   await resp.json()
来源：https://lu.zhonguo8118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://er.zhonguo7118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://wz.zhonguo5118.cn

Ruby: JSON.parse(resp.body)
来源：https://bl.zhonguo2118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://sx.zhonguo3118.cn

[L07] 处理 HTTP 状态码
来源：https://jo.zhonguo4118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://zg.zhonguo3118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://pj.zhonguo2118.cn

JS:   resp.ok;  resp.status
来源：https://pr.zhonguo6118.cn

TS:   resp.ok;  resp.status
来源：https://py.zhonguo5118.cn

Java: resp.statusCode()
来源：https://mn.zhonguo4118.cn

Go:   resp.StatusCode
来源：https://ax.zhonguo5118.cn

Ruby: resp.code.to_i
来源：https://tl.zhonguo7118.cn

C#:   (int)resp.StatusCode
来源：https://cu.zhonguo5118.cn

[L08] 并发请求多个地址
来源：https://ha.zhonguo8118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://vi.zhonguo8118.cn

PHP:  curl_multi_init() 系列
来源：https://up.zhonguo7118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ce.zhonguo1118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://fw.zhonguo4118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://mz.zhonguo6118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://ze.zhonguo8118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://dg.zhonguo1118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://lu.zhonguo2118.cn

================================================================================
来源：https://od.zhonguo5118.cn

M. 命令行 / 进程 / 环境
来源：https://on.zhonguo1118.cn

================================================================================
来源：https://sf.zhonguo2118.cn

[M01] 读取命令行参数
来源：https://ja.zhonguo2118.cn

Py:   sys.argv[1:]
来源：https://ig.zhonguo4118.cn

PHP:  $argv;  $argc;
来源：https://ec.zhonguo5118.cn

JS:   process.argv.slice(2)
来源：https://qb.zhonguo2118.cn

TS:   process.argv.slice(2)
来源：https://ly.zhonguo1118.cn

Java: args 数组（main 方法参数）
来源：https://tm.zhonguo6118.cn

Go:   os.Args[1:]
来源：https://qj.zhonguo3118.cn

Ruby: ARGV
来源：https://pu.zhonguo5118.cn

C#:   args 数组（Main 方法参数）
来源：https://gt.zhonguo1118.cn

[M02] 读取环境变量
来源：https://xn.zhonguo4118.cn

Py:   os.environ.get("HOME")
来源：https://bq.zhonguo5118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://di.zhonguo1118.cn

JS:   process.env.HOME
来源：https://wv.zhonguo8118.cn

TS:   process.env.HOME
来源：https://pj.zhonguo4118.cn

Java: System.getenv("HOME")
来源：https://mt.zhonguo3118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://oq.zhonguo7118.cn

Ruby: ENV["HOME"]
来源：https://iy.zhonguo4118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://ma.zhonguo2118.cn

[M03] 执行外部命令
来源：https://jd.zhonguo1118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://de.zhonguo1118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://wj.zhonguo2118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://jk.zhonguo1118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://mv.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://ln.zhonguo4118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://fq.zhonguo8118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://rg.zhonguo3118.cn

C#:   Process.Start("ls", "-l");
来源：https://ap.zhonguo4118.cn

[M04] 获取当前工作目录
来源：https://ux.zhonguo6118.cn

Py:   os.getcwd()
来源：https://hl.zhonguo3118.cn

PHP:  getcwd();
来源：https://ho.zhonguo5118.cn

JS:   process.cwd()
来源：https://hy.zhonguo1118.cn

TS:   process.cwd()
来源：https://py.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://oa.zhonguo6118.cn

Go:   os.Getwd()
来源：https://mk.zhonguo3118.cn

Ruby: Dir.pwd
来源：https://ha.zhonguo1118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ei.zhonguo3118.cn

[M05] 设置退出码
来源：https://rt.zhonguo4118.cn

Py:   sys.exit(1)
来源：https://bg.zhonguo4118.cn

PHP:  exit(1);
来源：https://wo.zhonguo7118.cn

JS:   process.exit(1)
来源：https://rc.zhonguo2118.cn

TS:   process.exit(1)
来源：https://ea.zhonguo2118.cn

Java: System.exit(1)
来源：https://tv.zhonguo1118.cn

Go:   os.Exit(1)
来源：https://cv.zhonguo2118.cn

Ruby: exit 1
来源：https://sk.zhonguo1118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://fz.zhonguo1118.cn

[M06] 向标准错误输出
来源：https://gt.zhonguo6118.cn

Py:   print("err", file=sys.stderr)
来源：https://jy.zhonguo1118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://xt.zhonguo4118.cn

JS:   console.error("err")
来源：https://zj.zhonguo2118.cn

TS:   console.error("err")
来源：https://ud.zhonguo1118.cn

Java: System.err.println("err")
来源：https://qd.zhonguo7118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://zh.zhonguo3118.cn

Ruby: warn "err"
来源：https://ys.zhonguo4118.cn

C#:   Console.Error.WriteLine("err")
来源：https://ds.zhonguo8118.cn

[M07] 判断是否为主入口
来源：https://nb.zhonguo3118.cn

Py:   if __name__ == "__main__":
来源：https://kp.zhonguo7118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://iu.zhonguo4118.cn

JS:   require.main === module
来源：https://qw.zhonguo6118.cn

TS:   require.main === module
来源：https://ln.zhonguo3118.cn

Java: public static void main(String[] args)
来源：https://an.zhonguo3118.cn

Go:   func main()
来源：https://my.zhonguo7118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://le.zhonguo1118.cn

C#:   static void Main(string[] args)
来源：https://hg.zhonguo1118.cn

[M08] 获取系统与运行时信息
来源：https://xw.zhonguo2118.cn

Py:   platform.system();  platform.python_version()
来源：https://pz.zhonguo8118.cn

PHP:  PHP_OS;  phpversion();
来源：https://kg.zhonguo8118.cn

JS:   process.platform;  process.version
来源：https://cd.zhonguo8118.cn

TS:   process.platform;  process.version
来源：https://ou.zhonguo1118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://hb.zhonguo1118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://is.zhonguo7118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://hp.zhonguo7118.cn


<!-- 参考信息 -->