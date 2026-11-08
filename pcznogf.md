代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：https://ym.zhonguo7118.cn

Go:   end.Sub(start).Hours()
来源：https://bg.zhonguo1118.cn

Ruby: end - start                 # 返回秒数
来源：https://sd.zhonguo6118.cn

C#:   (end - start).TotalSeconds
来源：https://jw.zhonguo7118.cn

[J07] 比较两个日期
来源：https://wm.zhonguo2118.cn

Py:   d1 < d2;  d1 == d2
来源：https://mh.zhonguo2118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://ra.zhonguo1118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://tl.zhonguo7118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://yq.zhonguo6118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://wg.zhonguo5118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://gr.zhonguo3118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://ue.zhonguo1118.cn

C#:   d1 < d2;  d1 == d2
来源：https://wg.zhonguo4118.cn

[J08] 提取年月日与星期
来源：https://ir.zhonguo1118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://av.zhonguo2118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ee.zhonguo2118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://mq.zhonguo5118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://vu.zhonguo6118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://et.zhonguo6118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://nn.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://dj.zhonguo8118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://xx.zhonguo3118.cn

[J09] 时区处理
来源：https://aa.zhonguo2118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://sm.zhonguo1118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://xl.zhonguo5118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://qg.zhonguo3118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://oi.zhonguo8118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://py.zhonguo5118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://sh.zhonguo5118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://fp.zhonguo8118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://gs.zhonguo7118.cn

[J10] 取今天 / 本月第一天
来源：https://bn.zhonguo1118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://wg.zhonguo7118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://mi.zhonguo6118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://rs.zhonguo1118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://me.zhonguo3118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://gf.zhonguo8118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://ve.zhonguo5118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://ft.zhonguo7118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://vd.zhonguo8118.cn

================================================================================
来源：https://go.zhonguo2118.cn

K. JSON 与序列化
来源：https://em.zhonguo6118.cn

================================================================================
来源：https://mo.zhonguo7118.cn

[K01] 对象转 JSON 字符串
来源：https://vf.zhonguo4118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://kr.zhonguo3118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://zm.zhonguo2118.cn

JS:   JSON.stringify(obj)
来源：https://yw.zhonguo5118.cn

TS:   JSON.stringify(obj)
来源：https://wn.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://qe.zhonguo3118.cn

Go:   json.Marshal(obj)
来源：https://gb.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://na.zhonguo6118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://ud.zhonguo4118.cn

[K02] JSON 字符串转对象
来源：https://jx.zhonguo2118.cn

Py:   json.loads(s)
来源：https://in.zhonguo7118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://vr.zhonguo4118.cn

JS:   JSON.parse(s)
来源：https://de.zhonguo3118.cn

TS:   JSON.parse(s)
来源：https://wf.zhonguo6118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://ko.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://wp.zhonguo7118.cn

Ruby: JSON.parse(s)
来源：https://gv.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://hs.zhonguo6118.cn

[K03] JSON 美化输出（带缩进）
来源：https://uh.zhonguo3118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://un.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://te.zhonguo7118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://pz.zhonguo5118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://rg.zhonguo6118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://xp.zhonguo2118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://mg.zhonguo7118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://ur.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://wr.zhonguo5118.cn

[K04] 读取 JSON 文件
来源：https://ff.zhonguo5118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://vr.zhonguo3118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://sk.zhonguo1118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ls.zhonguo2118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ch.zhonguo7118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://lo.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://rn.zhonguo3118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://wu.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://lv.zhonguo8118.cn

[K05] 深拷贝对象
来源：https://hk.zhonguo1118.cn

Py:   copy.deepcopy(obj)
来源：https://it.zhonguo2118.cn

PHP:  unserialize(serialize($obj));
来源：https://nv.zhonguo8118.cn

JS:   structuredClone(obj)
来源：https://gg.zhonguo5118.cn

TS:   structuredClone(obj)
来源：https://zd.zhonguo3118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ys.zhonguo2118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://jj.zhonguo2118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://dd.zhonguo7118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://lq.zhonguo7118.cn

[K06] 解析 URL 查询串
来源：https://ex.zhonguo5118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://nk.zhonguo3118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://uz.zhonguo4118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://bi.zhonguo3118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://nk.zhonguo6118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://sq.zhonguo5118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://vz.zhonguo7118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://dn.zhonguo7118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://ym.zhonguo6118.cn

[K07] 进制转换
来源：https://jg.zhonguo5118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://ox.zhonguo5118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://ga.zhonguo2118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://an.zhonguo3118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://ta.zhonguo7118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://jp.zhonguo5118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://kd.zhonguo2118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://af.zhonguo2118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://db.zhonguo8118.cn

[K08] 二进制序列化（非 JSON）
来源：https://mu.zhonguo4118.cn

Py:   pickle.dumps(obj)
来源：https://ll.zhonguo5118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://kg.zhonguo3118.cn

JS:   v8.serialize(obj)        // Node
来源：https://qa.zhonguo2118.cn

TS:   v8.serialize(obj)        // Node
来源：https://pr.zhonguo5118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://tv.zhonguo2118.cn

Go:   encoding/gob
来源：https://sb.zhonguo3118.cn

Ruby: Marshal.dump(obj)
来源：https://lm.zhonguo7118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://az.zhonguo3118.cn

================================================================================
来源：https://lc.zhonguo6118.cn

L. 网络请求
来源：https://oz.zhonguo7118.cn

================================================================================
来源：https://jb.zhonguo6118.cn

[L01] 发送 GET 请求
来源：https://oq.zhonguo6118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://zy.zhonguo2118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://tb.zhonguo4118.cn

JS:   await fetch(url)
来源：https://oc.zhonguo4118.cn

TS:   await fetch(url)
来源：https://gf.zhonguo2118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://jq.zhonguo8118.cn

Go:   resp, err := http.Get(url)
来源：https://su.zhonguo5118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://su.zhonguo3118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://ca.zhonguo5118.cn

[L02] 发送 POST JSON
来源：https://mu.zhonguo1118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://nr.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://ag.zhonguo3118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://zq.zhonguo3118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://mz.zhonguo6118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://wy.zhonguo4118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://vm.zhonguo5118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://qc.zhonguo6118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://hs.zhonguo4118.cn

[L03] 设置自定义请求头
来源：https://dl.zhonguo3118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://bj.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://hl.zhonguo4118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://rt.zhonguo8118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://li.zhonguo6118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://km.zhonguo2118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://tv.zhonguo8118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://zh.zhonguo6118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://qo.zhonguo5118.cn

[L04] 设置超时
来源：https://xn.zhonguo3118.cn

Py:   requests.get(url, timeout=5)
来源：https://my.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://ma.zhonguo5118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://cy.zhonguo6118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://vm.zhonguo2118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://zl.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://fx.zhonguo1118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://pn.zhonguo1118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://sd.zhonguo5118.cn

[L05] 上传文件（multipart）
来源：https://ob.zhonguo2118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://yf.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://wq.zhonguo7118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://rx.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://rq.zhonguo1118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://bd.zhonguo5118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://rg.zhonguo6118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ls.zhonguo8118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://md.zhonguo5118.cn

[L06] 解析响应为 JSON
来源：https://mr.zhonguo4118.cn

Py:   resp.json()
来源：https://hm.zhonguo2118.cn

PHP:  json_decode($body, true);
来源：https://fx.zhonguo3118.cn

JS:   await resp.json()
来源：https://tf.zhonguo3118.cn

TS:   await resp.json()
来源：https://lp.zhonguo4118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://xy.zhonguo4118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://kq.zhonguo4118.cn

Ruby: JSON.parse(resp.body)
来源：https://fr.zhonguo6118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://or.zhonguo6118.cn

[L07] 处理 HTTP 状态码
来源：https://bf.zhonguo2118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://yn.zhonguo5118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://oa.zhonguo6118.cn

JS:   resp.ok;  resp.status
来源：https://ql.zhonguo2118.cn

TS:   resp.ok;  resp.status
来源：https://at.zhonguo4118.cn

Java: resp.statusCode()
来源：https://bs.zhonguo8118.cn

Go:   resp.StatusCode
来源：https://pq.zhonguo5118.cn

Ruby: resp.code.to_i
来源：https://ya.zhonguo2118.cn

C#:   (int)resp.StatusCode
来源：https://gn.zhonguo8118.cn

[L08] 并发请求多个地址
来源：https://lp.zhonguo4118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://wz.zhonguo7118.cn

PHP:  curl_multi_init() 系列
来源：https://ob.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://jf.zhonguo8118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://xq.zhonguo4118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://fx.zhonguo8118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://py.zhonguo6118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://ri.zhonguo3118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://qq.zhonguo7118.cn

================================================================================
来源：https://am.zhonguo4118.cn

M. 命令行 / 进程 / 环境
来源：https://cd.zhonguo2118.cn

================================================================================
来源：https://wy.zhonguo1118.cn

[M01] 读取命令行参数
来源：https://so.zhonguo4118.cn

Py:   sys.argv[1:]
来源：https://lm.zhonguo6118.cn

PHP:  $argv;  $argc;
来源：https://bb.zhonguo6118.cn

JS:   process.argv.slice(2)
来源：https://ok.zhonguo1118.cn

TS:   process.argv.slice(2)
来源：https://mc.zhonguo8118.cn

Java: args 数组（main 方法参数）
来源：https://sz.zhonguo8118.cn

Go:   os.Args[1:]
来源：https://qc.zhonguo6118.cn

Ruby: ARGV
来源：https://ed.zhonguo1118.cn

C#:   args 数组（Main 方法参数）
来源：https://yq.zhonguo5118.cn

[M02] 读取环境变量
来源：https://fg.zhonguo5118.cn

Py:   os.environ.get("HOME")
来源：https://ol.zhonguo4118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://uz.zhonguo7118.cn

JS:   process.env.HOME
来源：https://kc.zhonguo8118.cn

TS:   process.env.HOME
来源：https://qy.zhonguo8118.cn

Java: System.getenv("HOME")
来源：https://rh.zhonguo4118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://vt.zhonguo8118.cn

Ruby: ENV["HOME"]
来源：https://ax.zhonguo8118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://tj.zhonguo5118.cn

[M03] 执行外部命令
来源：https://em.zhonguo8118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://ev.zhonguo5118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://cx.zhonguo4118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://jc.zhonguo6118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://hg.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://lu.zhonguo7118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://ie.zhonguo7118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://gb.zhonguo6118.cn

C#:   Process.Start("ls", "-l");
来源：https://ou.zhonguo1118.cn

[M04] 获取当前工作目录
来源：https://bz.zhonguo8118.cn

Py:   os.getcwd()
来源：https://xd.zhonguo2118.cn

PHP:  getcwd();
来源：https://co.zhonguo8118.cn

JS:   process.cwd()
来源：https://id.zhonguo5118.cn

TS:   process.cwd()
来源：https://jc.zhonguo4118.cn

Java: Path.of("").toAbsolutePath()
来源：https://qw.zhonguo6118.cn

Go:   os.Getwd()
来源：https://qg.zhonguo5118.cn

Ruby: Dir.pwd
来源：https://lg.zhonguo8118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://pb.zhonguo2118.cn

[M05] 设置退出码
来源：https://sd.zhonguo2118.cn

Py:   sys.exit(1)
来源：https://uc.zhonguo5118.cn

PHP:  exit(1);
来源：https://cn.zhonguo7118.cn

JS:   process.exit(1)
来源：https://ng.zhonguo4118.cn

TS:   process.exit(1)
来源：https://nt.zhonguo8118.cn

Java: System.exit(1)
来源：https://hw.zhonguo3118.cn

Go:   os.Exit(1)
来源：https://eo.zhonguo6118.cn

Ruby: exit 1
来源：https://px.zhonguo2118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://rl.zhonguo4118.cn

[M06] 向标准错误输出
来源：https://bn.zhonguo2118.cn

Py:   print("err", file=sys.stderr)
来源：https://mj.zhonguo4118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://cy.zhonguo5118.cn

JS:   console.error("err")
来源：https://uv.zhonguo5118.cn

TS:   console.error("err")
来源：https://ii.zhonguo5118.cn

Java: System.err.println("err")
来源：https://dl.zhonguo1118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://qh.zhonguo2118.cn

Ruby: warn "err"
来源：https://yw.zhonguo6118.cn

C#:   Console.Error.WriteLine("err")
来源：https://zr.zhonguo5118.cn

[M07] 判断是否为主入口
来源：https://uh.zhonguo2118.cn

Py:   if __name__ == "__main__":
来源：https://mx.zhonguo5118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://qz.zhonguo4118.cn

JS:   require.main === module
来源：https://bk.zhonguo7118.cn

TS:   require.main === module
来源：https://hx.zhonguo4118.cn

Java: public static void main(String[] args)
来源：https://yr.zhonguo7118.cn

Go:   func main()
来源：https://eb.zhonguo6118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://qr.zhonguo1118.cn

C#:   static void Main(string[] args)
来源：https://iq.zhonguo2118.cn

[M08] 获取系统与运行时信息
来源：https://of.zhonguo3118.cn

Py:   platform.system();  platform.python_version()
来源：https://og.zhonguo6118.cn

PHP:  PHP_OS;  phpversion();
来源：https://bd.zhonguo6118.cn

JS:   process.platform;  process.version
来源：https://rx.zhonguo1118.cn

TS:   process.platform;  process.version
来源：https://kg.zhonguo1118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://ft.zhonguo4118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://pa.zhonguo8118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://mo.zhonguo2118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://gr.zhonguo5118.cn

================================================================================
来源：https://xh.zhonguo7118.cn

N. 数据结构与算法
来源：https://fy.zhonguo5118.cn

================================================================================
来源：https://nh.zhonguo4118.cn

[N01] 二分查找（有序数组）
来源：https://ro.zhonguo2118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://zc.zhonguo8118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://rs.zhonguo4118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://pl.zhonguo7118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://gg.zhonguo3118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://yw.zhonguo1118.cn

Go:   sort.SearchInts(arr, x)
来源：https://dx.zhonguo1118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://wb.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://cc.zhonguo6118.cn

[N02] 排序（工程实践用内置实现）
来源：https://ui.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://jg.zhonguo1118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://up.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://uw.zhonguo5118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://vo.zhonguo1118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://gx.zhonguo5118.cn

Go:   slices.Sort(arr)
来源：https://yl.zhonguo7118.cn

Ruby: arr.sort
来源：https://gu.zhonguo1118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://au.zhonguo3118.cn

[N03] 快速排序（分治示例）
来源：https://tg.zhonguo4118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://hg.zhonguo8118.cn

PHP:  // 递归实现，或用 usort
来源：https://lb.zhonguo2118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://lu.zhonguo8118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://gy.zhonguo7118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://tx.zhonguo6118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://xe.zhonguo5118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://mj.zhonguo7118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://ju.zhonguo2118.cn

[N04] 斐波那契数列
来源：https://wi.zhonguo6118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://ki.zhonguo1118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://cr.zhonguo6118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://be.zhonguo5118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://rr.zhonguo3118.cn


<!-- 参考信息 -->