代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://sx.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://gl.zhonguo6118.cn

TS:   new Date();  Date.now()
来源：https://dv.zhonguo6118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://wb.zhonguo6118.cn

Go:   time.Now()
来源：https://ao.zhonguo2118.cn

Ruby: Time.now
来源：https://in.zhonguo3118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://hj.zhonguo2118.cn

[J02] 格式化输出
来源：https://qn.zhonguo5118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://vu.zhonguo8118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ks.zhonguo4118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://gx.zhonguo2118.cn

TS:   d.toISOString()
来源：https://tc.zhonguo7118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://kj.zhonguo2118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://wn.zhonguo2118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://wt.zhonguo4118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://lf.zhonguo4118.cn

[J03] 字符串解析为日期
来源：https://ha.zhonguo1118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://nn.zhonguo6118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://vj.zhonguo8118.cn

JS:   new Date("2024-01-02")
来源：https://jp.zhonguo2118.cn

TS:   new Date("2024-01-02")
来源：https://lm.zhonguo1118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://nn.zhonguo4118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://th.zhonguo7118.cn

Ruby: Date.parse("2024-01-02")
来源：https://zt.zhonguo3118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://wf.zhonguo8118.cn

[J04] 时间戳与日期互转
来源：https://iw.zhonguo4118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://ix.zhonguo7118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://rv.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://ky.zhonguo2118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://ao.zhonguo4118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://ws.zhonguo8118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://sw.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://wt.zhonguo6118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://gw.zhonguo1118.cn

[J05] 时间加减（加 7 天）
来源：https://ps.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://hk.zhonguo5118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://vq.zhonguo5118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://fq.zhonguo8118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://xy.zhonguo1118.cn

Java: LocalDate.now().plusDays(7)
来源：https://sl.zhonguo6118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://nn.zhonguo8118.cn

Ruby: Time.now + 7 * 86400
来源：https://sj.zhonguo2118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://ks.zhonguo4118.cn

[J06] 计算两时间之差
来源：https://az.zhonguo3118.cn

Py:   (end - start).total_seconds()
来源：https://mk.zhonguo4118.cn

PHP:  $end->diff($start)->days;
来源：https://al.zhonguo5118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://ay.zhonguo4118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://bd.zhonguo3118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://rf.zhonguo8118.cn

Go:   end.Sub(start).Hours()
来源：https://qm.zhonguo8118.cn

Ruby: end - start                 # 返回秒数
来源：https://bp.zhonguo6118.cn

C#:   (end - start).TotalSeconds
来源：https://td.zhonguo5118.cn

[J07] 比较两个日期
来源：https://ol.zhonguo7118.cn

Py:   d1 < d2;  d1 == d2
来源：https://wa.zhonguo5118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://fq.zhonguo4118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ef.zhonguo4118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://xb.zhonguo6118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://hk.zhonguo5118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://ei.zhonguo5118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://kx.zhonguo1118.cn

C#:   d1 < d2;  d1 == d2
来源：https://lm.zhonguo4118.cn

[J08] 提取年月日与星期
来源：https://am.zhonguo7118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://kb.zhonguo6118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://fu.zhonguo2118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://ip.zhonguo8118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://xp.zhonguo8118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://pc.zhonguo4118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://nx.zhonguo2118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://sz.zhonguo6118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://vp.zhonguo7118.cn

[J09] 时区处理
来源：https://ed.zhonguo1118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://mj.zhonguo2118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://gi.zhonguo1118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://jm.zhonguo4118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://lv.zhonguo8118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://hl.zhonguo5118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://vb.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://zh.zhonguo7118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://xb.zhonguo7118.cn

[J10] 取今天 / 本月第一天
来源：https://kn.zhonguo4118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://sf.zhonguo3118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://sa.zhonguo4118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://jb.zhonguo2118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://rz.zhonguo5118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://jb.zhonguo4118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://yt.zhonguo5118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://lq.zhonguo3118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://et.zhonguo2118.cn

================================================================================
来源：https://hz.zhonguo8118.cn

K. JSON 与序列化
来源：https://uc.zhonguo6118.cn

================================================================================
来源：https://jg.zhonguo4118.cn

[K01] 对象转 JSON 字符串
来源：https://iu.zhonguo5118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://qi.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://pl.zhonguo5118.cn

JS:   JSON.stringify(obj)
来源：https://tf.zhonguo1118.cn

TS:   JSON.stringify(obj)
来源：https://cz.zhonguo7118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://mp.zhonguo7118.cn

Go:   json.Marshal(obj)
来源：https://fa.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://fz.zhonguo7118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://jl.zhonguo8118.cn

[K02] JSON 字符串转对象
来源：https://sy.zhonguo2118.cn

Py:   json.loads(s)
来源：https://rb.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://xp.zhonguo3118.cn

JS:   JSON.parse(s)
来源：https://kp.zhonguo1118.cn

TS:   JSON.parse(s)
来源：https://lo.zhonguo4118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://xo.zhonguo3118.cn

Go:   json.Unmarshal(data, &v)
来源：https://ro.zhonguo6118.cn

Ruby: JSON.parse(s)
来源：https://kp.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://sg.zhonguo5118.cn

[K03] JSON 美化输出（带缩进）
来源：https://zs.zhonguo7118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://wi.zhonguo7118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://py.zhonguo3118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://wz.zhonguo3118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://qe.zhonguo6118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://nz.zhonguo5118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://bh.zhonguo3118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://ev.zhonguo7118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://pi.zhonguo6118.cn

[K04] 读取 JSON 文件
来源：https://ja.zhonguo3118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://yx.zhonguo2118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://fm.zhonguo2118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://hu.zhonguo2118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://if.zhonguo8118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://zc.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://ef.zhonguo7118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://gb.zhonguo3118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://pn.zhonguo7118.cn

[K05] 深拷贝对象
来源：https://wz.zhonguo6118.cn

Py:   copy.deepcopy(obj)
来源：https://kj.zhonguo2118.cn

PHP:  unserialize(serialize($obj));
来源：https://wn.zhonguo4118.cn

JS:   structuredClone(obj)
来源：https://bx.zhonguo7118.cn

TS:   structuredClone(obj)
来源：https://jy.zhonguo6118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://wn.zhonguo8118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ob.zhonguo5118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://gs.zhonguo2118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://ud.zhonguo1118.cn

[K06] 解析 URL 查询串
来源：https://eq.zhonguo7118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://qq.zhonguo1118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://em.zhonguo7118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://uz.zhonguo3118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://rn.zhonguo8118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://re.zhonguo8118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://bq.zhonguo1118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://hr.zhonguo8118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://vl.zhonguo6118.cn

[K07] 进制转换
来源：https://sp.zhonguo8118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://ik.zhonguo1118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://na.zhonguo2118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://ao.zhonguo3118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://np.zhonguo5118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://fr.zhonguo6118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://qo.zhonguo3118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://dj.zhonguo2118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://it.zhonguo1118.cn

[K08] 二进制序列化（非 JSON）
来源：https://fe.zhonguo3118.cn

Py:   pickle.dumps(obj)
来源：https://gf.zhonguo2118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://dh.zhonguo1118.cn

JS:   v8.serialize(obj)        // Node
来源：https://lb.zhonguo7118.cn

TS:   v8.serialize(obj)        // Node
来源：https://jq.zhonguo4118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://nz.zhonguo5118.cn

Go:   encoding/gob
来源：https://ep.zhonguo3118.cn

Ruby: Marshal.dump(obj)
来源：https://fj.zhonguo6118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://qj.zhonguo5118.cn

================================================================================
来源：https://qa.zhonguo7118.cn

L. 网络请求
来源：https://ye.zhonguo6118.cn

================================================================================
来源：https://ip.zhonguo3118.cn

[L01] 发送 GET 请求
来源：https://nx.zhonguo2118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://xy.zhonguo6118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://ag.zhonguo2118.cn

JS:   await fetch(url)
来源：https://ts.zhonguo2118.cn

TS:   await fetch(url)
来源：https://bl.zhonguo3118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://ya.zhonguo2118.cn

Go:   resp, err := http.Get(url)
来源：https://cm.zhonguo1118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://au.zhonguo4118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://hn.zhonguo2118.cn

[L02] 发送 POST JSON
来源：https://az.zhonguo3118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://yp.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://it.zhonguo1118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://wk.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://mx.zhonguo7118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://mm.zhonguo6118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://lr.zhonguo4118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://zb.zhonguo7118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://hz.zhonguo6118.cn

[L03] 设置自定义请求头
来源：https://lr.zhonguo8118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://ce.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://vl.zhonguo2118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://cv.zhonguo1118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://gl.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://ir.zhonguo8118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://uc.zhonguo6118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://gu.zhonguo4118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://en.zhonguo1118.cn

[L04] 设置超时
来源：https://zy.zhonguo8118.cn

Py:   requests.get(url, timeout=5)
来源：https://ai.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://yj.zhonguo3118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://ht.zhonguo7118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://zf.zhonguo3118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://vt.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://so.zhonguo7118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://im.zhonguo4118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://uc.zhonguo3118.cn

[L05] 上传文件（multipart）
来源：https://oy.zhonguo7118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://xh.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://lq.zhonguo4118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://kh.zhonguo4118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://gs.zhonguo4118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://cx.zhonguo5118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://yy.zhonguo7118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ac.zhonguo1118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://cc.zhonguo2118.cn

[L06] 解析响应为 JSON
来源：https://xl.zhonguo7118.cn

Py:   resp.json()
来源：https://py.zhonguo2118.cn

PHP:  json_decode($body, true);
来源：https://ir.zhonguo3118.cn

JS:   await resp.json()
来源：https://im.zhonguo3118.cn

TS:   await resp.json()
来源：https://pa.zhonguo8118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://te.zhonguo1118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://jw.zhonguo8118.cn

Ruby: JSON.parse(resp.body)
来源：https://jf.zhonguo5118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://dv.zhonguo1118.cn

[L07] 处理 HTTP 状态码
来源：https://rh.zhonguo4118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://qx.zhonguo2118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://vr.zhonguo2118.cn

JS:   resp.ok;  resp.status
来源：https://pg.zhonguo1118.cn

TS:   resp.ok;  resp.status
来源：https://gt.zhonguo8118.cn

Java: resp.statusCode()
来源：https://oe.zhonguo6118.cn

Go:   resp.StatusCode
来源：https://sn.zhonguo6118.cn

Ruby: resp.code.to_i
来源：https://ys.zhonguo4118.cn

C#:   (int)resp.StatusCode
来源：https://tn.zhonguo1118.cn

[L08] 并发请求多个地址
来源：https://eg.zhonguo1118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://pi.zhonguo8118.cn

PHP:  curl_multi_init() 系列
来源：https://dl.zhonguo4118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://el.zhonguo3118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://zv.zhonguo2118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://ar.zhonguo4118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://lt.zhonguo2118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://dr.zhonguo3118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://pj.zhonguo6118.cn

================================================================================
来源：https://fr.zhonguo3118.cn

M. 命令行 / 进程 / 环境
来源：https://tn.zhonguo3118.cn

================================================================================
来源：https://md.zhonguo8118.cn

[M01] 读取命令行参数
来源：https://pn.zhonguo4118.cn

Py:   sys.argv[1:]
来源：https://zf.zhonguo8118.cn

PHP:  $argv;  $argc;
来源：https://wc.zhonguo8118.cn

JS:   process.argv.slice(2)
来源：https://yc.zhonguo5118.cn

TS:   process.argv.slice(2)
来源：https://qv.zhonguo8118.cn

Java: args 数组（main 方法参数）
来源：https://rg.zhonguo3118.cn

Go:   os.Args[1:]
来源：https://ol.zhonguo1118.cn

Ruby: ARGV
来源：https://ig.zhonguo2118.cn

C#:   args 数组（Main 方法参数）
来源：https://ou.zhonguo4118.cn

[M02] 读取环境变量
来源：https://cc.zhonguo4118.cn

Py:   os.environ.get("HOME")
来源：https://qh.zhonguo5118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://ue.zhonguo4118.cn

JS:   process.env.HOME
来源：https://ja.zhonguo5118.cn

TS:   process.env.HOME
来源：https://zb.zhonguo1118.cn

Java: System.getenv("HOME")
来源：https://oq.zhonguo6118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://cp.zhonguo6118.cn

Ruby: ENV["HOME"]
来源：https://lv.zhonguo5118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://gl.zhonguo2118.cn

[M03] 执行外部命令
来源：https://ri.zhonguo4118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://wh.zhonguo3118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://rj.zhonguo8118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://lm.zhonguo7118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://jp.zhonguo5118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://kj.zhonguo8118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://yh.zhonguo1118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://kq.zhonguo5118.cn

C#:   Process.Start("ls", "-l");
来源：https://xv.zhonguo8118.cn

[M04] 获取当前工作目录
来源：https://yh.zhonguo6118.cn

Py:   os.getcwd()
来源：https://bg.zhonguo4118.cn

PHP:  getcwd();
来源：https://ja.zhonguo5118.cn

JS:   process.cwd()
来源：https://tm.zhonguo1118.cn

TS:   process.cwd()
来源：https://tb.zhonguo6118.cn

Java: Path.of("").toAbsolutePath()
来源：https://bi.zhonguo3118.cn

Go:   os.Getwd()
来源：https://ce.zhonguo1118.cn

Ruby: Dir.pwd
来源：https://md.zhonguo7118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://xx.zhonguo4118.cn

[M05] 设置退出码
来源：https://ju.zhonguo1118.cn

Py:   sys.exit(1)
来源：https://ie.zhonguo3118.cn

PHP:  exit(1);
来源：https://ev.zhonguo2118.cn

JS:   process.exit(1)
来源：https://cr.zhonguo7118.cn

TS:   process.exit(1)
来源：https://vp.zhonguo1118.cn

Java: System.exit(1)
来源：https://cn.zhonguo2118.cn

Go:   os.Exit(1)
来源：https://br.zhonguo4118.cn

Ruby: exit 1
来源：https://um.zhonguo8118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://rt.zhonguo7118.cn

[M06] 向标准错误输出
来源：https://cf.zhonguo8118.cn

Py:   print("err", file=sys.stderr)
来源：https://pi.zhonguo8118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://ns.zhonguo6118.cn

JS:   console.error("err")
来源：https://lw.zhonguo1118.cn

TS:   console.error("err")
来源：https://kp.zhonguo4118.cn

Java: System.err.println("err")
来源：https://sz.zhonguo7118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://ix.zhonguo1118.cn

Ruby: warn "err"
来源：https://cx.zhonguo5118.cn

C#:   Console.Error.WriteLine("err")
来源：https://dd.zhonguo5118.cn

[M07] 判断是否为主入口
来源：https://mz.zhonguo8118.cn

Py:   if __name__ == "__main__":
来源：https://zo.zhonguo4118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://nx.zhonguo5118.cn

JS:   require.main === module
来源：https://bg.zhonguo6118.cn

TS:   require.main === module
来源：https://nb.zhonguo3118.cn


<!-- 参考信息 -->