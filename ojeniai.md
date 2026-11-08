代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://cg.zhonguo3118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://oa.zhonguo3118.cn

[J05] 时间加减（加 7 天）
来源：https://mh.zhonguo8118.cn

Py:   now + timedelta(days=7)
来源：https://mi.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://oe.zhonguo2118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://hc.zhonguo6118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://zz.zhonguo2118.cn

Java: LocalDate.now().plusDays(7)
来源：https://pl.zhonguo1118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://rv.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://qe.zhonguo2118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://pu.zhonguo1118.cn

[J06] 计算两时间之差
来源：https://lh.zhonguo3118.cn

Py:   (end - start).total_seconds()
来源：https://zb.zhonguo5118.cn

PHP:  $end->diff($start)->days;
来源：https://yg.zhonguo4118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://ei.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://dl.zhonguo2118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://vk.zhonguo6118.cn

Go:   end.Sub(start).Hours()
来源：https://ts.zhonguo8118.cn

Ruby: end - start                 # 返回秒数
来源：https://xn.zhonguo1118.cn

C#:   (end - start).TotalSeconds
来源：https://qz.zhonguo7118.cn

[J07] 比较两个日期
来源：https://kf.zhonguo5118.cn

Py:   d1 < d2;  d1 == d2
来源：https://bf.zhonguo1118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://vu.zhonguo7118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ur.zhonguo1118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://cr.zhonguo7118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://vw.zhonguo1118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://gp.zhonguo6118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://dd.zhonguo8118.cn

C#:   d1 < d2;  d1 == d2
来源：https://xp.zhonguo2118.cn

[J08] 提取年月日与星期
来源：https://qp.zhonguo2118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://ao.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://dc.zhonguo3118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://td.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://nb.zhonguo6118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://iv.zhonguo5118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://lo.zhonguo2118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://pp.zhonguo4118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ha.zhonguo5118.cn

[J09] 时区处理
来源：https://hg.zhonguo3118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://oz.zhonguo3118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://xg.zhonguo1118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://gr.zhonguo2118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://uc.zhonguo5118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://bb.zhonguo6118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://gm.zhonguo4118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://mp.zhonguo4118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://fx.zhonguo4118.cn

[J10] 取今天 / 本月第一天
来源：https://fe.zhonguo3118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ds.zhonguo2118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://xc.zhonguo1118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://uf.zhonguo7118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://av.zhonguo1118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://cm.zhonguo4118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://oc.zhonguo3118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://jp.zhonguo2118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://xa.zhonguo1118.cn

================================================================================
来源：https://zj.zhonguo8118.cn

K. JSON 与序列化
来源：https://cg.zhonguo5118.cn

================================================================================
来源：https://rd.zhonguo7118.cn

[K01] 对象转 JSON 字符串
来源：https://wa.zhonguo1118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://yq.zhonguo3118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://vx.zhonguo2118.cn

JS:   JSON.stringify(obj)
来源：https://bp.zhonguo7118.cn

TS:   JSON.stringify(obj)
来源：https://ng.zhonguo3118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://gm.zhonguo2118.cn

Go:   json.Marshal(obj)
来源：https://dz.zhonguo5118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://ys.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://cl.zhonguo1118.cn

[K02] JSON 字符串转对象
来源：https://pg.zhonguo7118.cn

Py:   json.loads(s)
来源：https://jn.zhonguo5118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://ut.zhonguo4118.cn

JS:   JSON.parse(s)
来源：https://jo.zhonguo1118.cn

TS:   JSON.parse(s)
来源：https://yv.zhonguo5118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://as.zhonguo5118.cn

Go:   json.Unmarshal(data, &v)
来源：https://aj.zhonguo4118.cn

Ruby: JSON.parse(s)
来源：https://vd.zhonguo1118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://ge.zhonguo7118.cn

[K03] JSON 美化输出（带缩进）
来源：https://ty.zhonguo3118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://tp.zhonguo5118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://ok.zhonguo8118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://kl.zhonguo3118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://rv.zhonguo1118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://sz.zhonguo2118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://it.zhonguo6118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://gh.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://ur.zhonguo8118.cn

[K04] 读取 JSON 文件
来源：https://mv.zhonguo2118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://nm.zhonguo6118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://fz.zhonguo7118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://re.zhonguo8118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://nl.zhonguo7118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://uc.zhonguo1118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://mz.zhonguo2118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://ki.zhonguo3118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://vh.zhonguo1118.cn

[K05] 深拷贝对象
来源：https://ie.zhonguo5118.cn

Py:   copy.deepcopy(obj)
来源：https://ne.zhonguo6118.cn

PHP:  unserialize(serialize($obj));
来源：https://bj.zhonguo1118.cn

JS:   structuredClone(obj)
来源：https://nj.zhonguo6118.cn

TS:   structuredClone(obj)
来源：https://qu.zhonguo5118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://vq.zhonguo6118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://cy.zhonguo6118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://ur.zhonguo6118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://mb.zhonguo4118.cn

[K06] 解析 URL 查询串
来源：https://ws.zhonguo3118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://es.zhonguo1118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://kn.zhonguo6118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://oq.zhonguo3118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://xs.zhonguo8118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://wt.zhonguo4118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://vg.zhonguo6118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://nf.zhonguo2118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://jy.zhonguo7118.cn

[K07] 进制转换
来源：https://ud.zhonguo3118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://lx.zhonguo3118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://jr.zhonguo5118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://mf.zhonguo7118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://qq.zhonguo7118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://em.zhonguo1118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://fv.zhonguo3118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://re.zhonguo8118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://lv.zhonguo3118.cn

[K08] 二进制序列化（非 JSON）
来源：https://bz.zhonguo5118.cn

Py:   pickle.dumps(obj)
来源：https://fj.zhonguo5118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://pt.zhonguo2118.cn

JS:   v8.serialize(obj)        // Node
来源：https://fa.zhonguo3118.cn

TS:   v8.serialize(obj)        // Node
来源：https://bv.zhonguo6118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://hf.zhonguo4118.cn

Go:   encoding/gob
来源：https://hb.zhonguo3118.cn

Ruby: Marshal.dump(obj)
来源：https://he.zhonguo3118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://ny.zhonguo7118.cn

================================================================================
来源：https://po.zhonguo4118.cn

L. 网络请求
来源：https://rz.zhonguo2118.cn

================================================================================
来源：https://rc.zhonguo5118.cn

[L01] 发送 GET 请求
来源：https://cz.zhonguo1118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://og.zhonguo5118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://qc.zhonguo6118.cn

JS:   await fetch(url)
来源：https://zl.zhonguo7118.cn

TS:   await fetch(url)
来源：https://cl.zhonguo7118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://gg.zhonguo8118.cn

Go:   resp, err := http.Get(url)
来源：https://tk.zhonguo4118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://ml.zhonguo5118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://kb.zhonguo7118.cn

[L02] 发送 POST JSON
来源：https://cl.zhonguo4118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://ur.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://ki.zhonguo4118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://mx.zhonguo8118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://er.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://fz.zhonguo1118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://oc.zhonguo4118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://kk.zhonguo8118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://qc.zhonguo3118.cn

[L03] 设置自定义请求头
来源：https://it.zhonguo7118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://sx.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://wf.zhonguo4118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://tw.zhonguo2118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://by.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://rm.zhonguo5118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://fx.zhonguo7118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://tl.zhonguo5118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://dw.zhonguo5118.cn

[L04] 设置超时
来源：https://gb.zhonguo2118.cn

Py:   requests.get(url, timeout=5)
来源：https://bi.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://bz.zhonguo2118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://qd.zhonguo7118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://xi.zhonguo6118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://pm.zhonguo6118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://ie.zhonguo2118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://oj.zhonguo6118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://et.zhonguo4118.cn

[L05] 上传文件（multipart）
来源：https://mn.zhonguo6118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://sq.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://ep.zhonguo6118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://kf.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://ew.zhonguo3118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://ng.zhonguo4118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://rz.zhonguo6118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://zj.zhonguo2118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://hv.zhonguo8118.cn

[L06] 解析响应为 JSON
来源：https://wt.zhonguo5118.cn

Py:   resp.json()
来源：https://ko.zhonguo5118.cn

PHP:  json_decode($body, true);
来源：https://xl.zhonguo2118.cn

JS:   await resp.json()
来源：https://yh.zhonguo5118.cn

TS:   await resp.json()
来源：https://ef.zhonguo3118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://tl.zhonguo1118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://mk.zhonguo6118.cn

Ruby: JSON.parse(resp.body)
来源：https://bk.zhonguo5118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://cp.zhonguo7118.cn

[L07] 处理 HTTP 状态码
来源：https://tn.zhonguo3118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://fa.zhonguo1118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://sh.zhonguo3118.cn

JS:   resp.ok;  resp.status
来源：https://po.zhonguo8118.cn

TS:   resp.ok;  resp.status
来源：https://xp.zhonguo6118.cn

Java: resp.statusCode()
来源：https://po.zhonguo4118.cn

Go:   resp.StatusCode
来源：https://qz.zhonguo6118.cn

Ruby: resp.code.to_i
来源：https://lp.zhonguo5118.cn

C#:   (int)resp.StatusCode
来源：https://eh.zhonguo3118.cn

[L08] 并发请求多个地址
来源：https://ez.zhonguo5118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://ju.zhonguo8118.cn

PHP:  curl_multi_init() 系列
来源：https://zn.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://df.zhonguo4118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ai.zhonguo1118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://sr.zhonguo5118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://uy.zhonguo3118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://xe.zhonguo7118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://bi.zhonguo2118.cn

================================================================================
来源：https://kk.zhonguo7118.cn

M. 命令行 / 进程 / 环境
来源：https://zc.zhonguo2118.cn

================================================================================
来源：https://js.zhonguo4118.cn

[M01] 读取命令行参数
来源：https://va.zhonguo8118.cn

Py:   sys.argv[1:]
来源：https://vl.zhonguo5118.cn

PHP:  $argv;  $argc;
来源：https://cq.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://di.zhonguo5118.cn

TS:   process.argv.slice(2)
来源：https://yk.zhonguo5118.cn

Java: args 数组（main 方法参数）
来源：https://xa.zhonguo6118.cn

Go:   os.Args[1:]
来源：https://ir.zhonguo8118.cn

Ruby: ARGV
来源：https://qp.zhonguo1118.cn

C#:   args 数组（Main 方法参数）
来源：https://ss.zhonguo3118.cn

[M02] 读取环境变量
来源：https://xx.zhonguo2118.cn

Py:   os.environ.get("HOME")
来源：https://rq.zhonguo5118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://bs.zhonguo8118.cn

JS:   process.env.HOME
来源：https://rt.zhonguo3118.cn

TS:   process.env.HOME
来源：https://rv.zhonguo5118.cn

Java: System.getenv("HOME")
来源：https://tr.zhonguo6118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://od.zhonguo8118.cn

Ruby: ENV["HOME"]
来源：https://eb.zhonguo2118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://ry.zhonguo4118.cn

[M03] 执行外部命令
来源：https://ry.zhonguo8118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://ys.zhonguo4118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://xy.zhonguo7118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://qw.zhonguo8118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://fp.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://ja.zhonguo6118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://yd.zhonguo4118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://fg.zhonguo4118.cn

C#:   Process.Start("ls", "-l");
来源：https://qh.zhonguo8118.cn

[M04] 获取当前工作目录
来源：https://nk.zhonguo1118.cn

Py:   os.getcwd()
来源：https://so.zhonguo8118.cn

PHP:  getcwd();
来源：https://lg.zhonguo4118.cn

JS:   process.cwd()
来源：https://ky.zhonguo7118.cn

TS:   process.cwd()
来源：https://bl.zhonguo5118.cn

Java: Path.of("").toAbsolutePath()
来源：https://ii.zhonguo6118.cn

Go:   os.Getwd()
来源：https://zr.zhonguo4118.cn

Ruby: Dir.pwd
来源：https://lq.zhonguo4118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://hm.zhonguo1118.cn

[M05] 设置退出码
来源：https://ip.zhonguo7118.cn

Py:   sys.exit(1)
来源：https://cl.zhonguo3118.cn

PHP:  exit(1);
来源：https://ex.zhonguo4118.cn

JS:   process.exit(1)
来源：https://tw.zhonguo5118.cn

TS:   process.exit(1)
来源：https://pg.zhonguo2118.cn

Java: System.exit(1)
来源：https://fw.zhonguo1118.cn

Go:   os.Exit(1)
来源：https://rf.zhonguo5118.cn

Ruby: exit 1
来源：https://lo.zhonguo6118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://nk.zhonguo3118.cn

[M06] 向标准错误输出
来源：https://nu.zhonguo4118.cn

Py:   print("err", file=sys.stderr)
来源：https://vn.zhonguo3118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://ro.zhonguo4118.cn

JS:   console.error("err")
来源：https://mx.zhonguo2118.cn

TS:   console.error("err")
来源：https://po.zhonguo5118.cn

Java: System.err.println("err")
来源：https://df.zhonguo6118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://jx.zhonguo5118.cn

Ruby: warn "err"
来源：https://wm.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://sp.zhonguo8118.cn

[M07] 判断是否为主入口
来源：https://lu.zhonguo7118.cn

Py:   if __name__ == "__main__":
来源：https://bh.zhonguo7118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://fg.zhonguo5118.cn

JS:   require.main === module
来源：https://os.zhonguo1118.cn

TS:   require.main === module
来源：https://ky.zhonguo6118.cn

Java: public static void main(String[] args)
来源：https://so.zhonguo1118.cn

Go:   func main()
来源：https://vb.zhonguo1118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://ym.zhonguo3118.cn

C#:   static void Main(string[] args)
来源：https://ft.zhonguo2118.cn

[M08] 获取系统与运行时信息
来源：https://sa.zhonguo5118.cn

Py:   platform.system();  platform.python_version()
来源：https://zt.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://xx.zhonguo4118.cn

JS:   process.platform;  process.version
来源：https://vv.zhonguo1118.cn

TS:   process.platform;  process.version
来源：https://uu.zhonguo2118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://tx.zhonguo3118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://mz.zhonguo3118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://xw.zhonguo7118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://eg.zhonguo6118.cn

================================================================================
来源：https://go.zhonguo8118.cn

N. 数据结构与算法
来源：https://vh.zhonguo5118.cn

================================================================================
来源：https://hr.zhonguo3118.cn

[N01] 二分查找（有序数组）
来源：https://mw.zhonguo7118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://pe.zhonguo8118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://pp.zhonguo2118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://nh.zhonguo4118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://xj.zhonguo5118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://gz.zhonguo1118.cn

Go:   sort.SearchInts(arr, x)
来源：https://bb.zhonguo2118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://id.zhonguo7118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://zf.zhonguo7118.cn

[N02] 排序（工程实践用内置实现）
来源：https://zu.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://ir.zhonguo2118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://gk.zhonguo2118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://fe.zhonguo4118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://pm.zhonguo3118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://qo.zhonguo8118.cn

Go:   slices.Sort(arr)
来源：https://ah.zhonguo7118.cn


<!-- 参考信息 -->