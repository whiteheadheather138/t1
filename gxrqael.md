代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://vz.zhonguo1118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://mg.zhonguo3118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://kj.zhonguo1118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://bs.zhonguo8118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://bw.zhonguo8118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://az.zhonguo3118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://cg.zhonguo1118.cn

[J10] 取今天 / 本月第一天
来源：https://hq.zhonguo6118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://dn.zhonguo4118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://it.zhonguo4118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://zz.zhonguo6118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://rn.zhonguo6118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://ho.zhonguo8118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://fx.zhonguo5118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://to.zhonguo4118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://aj.zhonguo5118.cn

================================================================================
来源：https://wm.zhonguo1118.cn

K. JSON 与序列化
来源：https://cl.zhonguo5118.cn

================================================================================
来源：https://pt.zhonguo5118.cn

[K01] 对象转 JSON 字符串
来源：https://be.zhonguo7118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://fq.zhonguo2118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://ua.zhonguo2118.cn

JS:   JSON.stringify(obj)
来源：https://rj.zhonguo3118.cn

TS:   JSON.stringify(obj)
来源：https://cx.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://xm.zhonguo4118.cn

Go:   json.Marshal(obj)
来源：https://oa.zhonguo4118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://og.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://ad.zhonguo8118.cn

[K02] JSON 字符串转对象
来源：https://kp.zhonguo8118.cn

Py:   json.loads(s)
来源：https://ql.zhonguo7118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://ix.zhonguo1118.cn

JS:   JSON.parse(s)
来源：https://fl.zhonguo5118.cn

TS:   JSON.parse(s)
来源：https://ll.zhonguo3118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://ji.zhonguo3118.cn

Go:   json.Unmarshal(data, &v)
来源：https://lf.zhonguo1118.cn

Ruby: JSON.parse(s)
来源：https://ob.zhonguo1118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://tg.zhonguo4118.cn

[K03] JSON 美化输出（带缩进）
来源：https://fm.zhonguo1118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://qj.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://pl.zhonguo8118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://ei.zhonguo8118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://es.zhonguo2118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://mz.zhonguo7118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://ic.zhonguo5118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://ie.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://zs.zhonguo5118.cn

[K04] 读取 JSON 文件
来源：https://uu.zhonguo2118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://xs.zhonguo2118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://np.zhonguo5118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://en.zhonguo8118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://me.zhonguo5118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://cd.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://bw.zhonguo3118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://ib.zhonguo4118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://vt.zhonguo5118.cn

[K05] 深拷贝对象
来源：https://cm.zhonguo1118.cn

Py:   copy.deepcopy(obj)
来源：https://uu.zhonguo7118.cn

PHP:  unserialize(serialize($obj));
来源：https://ff.zhonguo8118.cn

JS:   structuredClone(obj)
来源：https://qe.zhonguo5118.cn

TS:   structuredClone(obj)
来源：https://gl.zhonguo7118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://jd.zhonguo1118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://hu.zhonguo3118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://gh.zhonguo7118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://es.zhonguo1118.cn

[K06] 解析 URL 查询串
来源：https://hz.zhonguo1118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://tb.zhonguo8118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://cb.zhonguo2118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://yu.zhonguo5118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ki.zhonguo5118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://ug.zhonguo8118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://oc.zhonguo4118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://qs.zhonguo7118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://yg.zhonguo8118.cn

[K07] 进制转换
来源：https://py.zhonguo6118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://ir.zhonguo2118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://yr.zhonguo2118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://qc.zhonguo6118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://wz.zhonguo2118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://za.zhonguo2118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ck.zhonguo7118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://xk.zhonguo6118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://qe.zhonguo1118.cn

[K08] 二进制序列化（非 JSON）
来源：https://yi.zhonguo5118.cn

Py:   pickle.dumps(obj)
来源：https://nf.zhonguo1118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://rn.zhonguo6118.cn

JS:   v8.serialize(obj)        // Node
来源：https://pv.zhonguo4118.cn

TS:   v8.serialize(obj)        // Node
来源：https://qr.zhonguo2118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://rg.zhonguo6118.cn

Go:   encoding/gob
来源：https://xf.zhonguo8118.cn

Ruby: Marshal.dump(obj)
来源：https://rp.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://wc.zhonguo6118.cn

================================================================================
来源：https://iz.zhonguo2118.cn

L. 网络请求
来源：https://qv.zhonguo5118.cn

================================================================================
来源：https://lc.zhonguo7118.cn

[L01] 发送 GET 请求
来源：https://ci.zhonguo3118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://sv.zhonguo1118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://tu.zhonguo6118.cn

JS:   await fetch(url)
来源：https://xq.zhonguo5118.cn

TS:   await fetch(url)
来源：https://re.zhonguo3118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://ya.zhonguo5118.cn

Go:   resp, err := http.Get(url)
来源：https://kl.zhonguo3118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://ts.zhonguo3118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://yt.zhonguo7118.cn

[L02] 发送 POST JSON
来源：https://ep.zhonguo2118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://mf.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://lm.zhonguo1118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://tc.zhonguo6118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://ut.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://fc.zhonguo7118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://du.zhonguo5118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://ch.zhonguo4118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://py.zhonguo2118.cn

[L03] 设置自定义请求头
来源：https://be.zhonguo5118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://nu.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://nc.zhonguo7118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://wv.zhonguo4118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ex.zhonguo8118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://ub.zhonguo4118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://qx.zhonguo7118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://el.zhonguo8118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://pb.zhonguo4118.cn

[L04] 设置超时
来源：https://yw.zhonguo8118.cn

Py:   requests.get(url, timeout=5)
来源：https://pp.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://ul.zhonguo1118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://wq.zhonguo7118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://fu.zhonguo3118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://fg.zhonguo4118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://li.zhonguo8118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://mv.zhonguo5118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://tv.zhonguo4118.cn

[L05] 上传文件（multipart）
来源：https://aq.zhonguo1118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://bs.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://sl.zhonguo8118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://sl.zhonguo7118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://mu.zhonguo5118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://wn.zhonguo3118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://xd.zhonguo5118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://lo.zhonguo6118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://jt.zhonguo3118.cn

[L06] 解析响应为 JSON
来源：https://pq.zhonguo7118.cn

Py:   resp.json()
来源：https://cx.zhonguo6118.cn

PHP:  json_decode($body, true);
来源：https://qk.zhonguo5118.cn

JS:   await resp.json()
来源：https://ce.zhonguo8118.cn

TS:   await resp.json()
来源：https://sr.zhonguo2118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://jr.zhonguo2118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://sd.zhonguo6118.cn

Ruby: JSON.parse(resp.body)
来源：https://cy.zhonguo5118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://ol.zhonguo3118.cn

[L07] 处理 HTTP 状态码
来源：https://yk.zhonguo3118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://jg.zhonguo4118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://ma.zhonguo8118.cn

JS:   resp.ok;  resp.status
来源：https://qs.zhonguo4118.cn

TS:   resp.ok;  resp.status
来源：https://pf.zhonguo3118.cn

Java: resp.statusCode()
来源：https://iw.zhonguo7118.cn

Go:   resp.StatusCode
来源：https://mf.zhonguo7118.cn

Ruby: resp.code.to_i
来源：https://jd.zhonguo8118.cn

C#:   (int)resp.StatusCode
来源：https://te.zhonguo8118.cn

[L08] 并发请求多个地址
来源：https://cf.zhonguo8118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://zc.zhonguo1118.cn

PHP:  curl_multi_init() 系列
来源：https://yp.zhonguo3118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ef.zhonguo5118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://po.zhonguo3118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://pt.zhonguo5118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://mz.zhonguo4118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://pb.zhonguo8118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://mj.zhonguo4118.cn

================================================================================
来源：https://yw.zhonguo8118.cn

M. 命令行 / 进程 / 环境
来源：https://bb.zhonguo1118.cn

================================================================================
来源：https://af.zhonguo7118.cn

[M01] 读取命令行参数
来源：https://hw.zhonguo1118.cn

Py:   sys.argv[1:]
来源：https://rc.zhonguo1118.cn

PHP:  $argv;  $argc;
来源：https://vh.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://ny.zhonguo7118.cn

TS:   process.argv.slice(2)
来源：https://kj.zhonguo5118.cn

Java: args 数组（main 方法参数）
来源：https://va.zhonguo7118.cn

Go:   os.Args[1:]
来源：https://xv.zhonguo2118.cn

Ruby: ARGV
来源：https://mt.zhonguo1118.cn

C#:   args 数组（Main 方法参数）
来源：https://wh.zhonguo5118.cn

[M02] 读取环境变量
来源：https://nu.zhonguo4118.cn

Py:   os.environ.get("HOME")
来源：https://qo.zhonguo3118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://jc.zhonguo5118.cn

JS:   process.env.HOME
来源：https://yc.zhonguo6118.cn

TS:   process.env.HOME
来源：https://mx.zhonguo7118.cn

Java: System.getenv("HOME")
来源：https://ze.zhonguo3118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://ar.zhonguo6118.cn

Ruby: ENV["HOME"]
来源：https://pb.zhonguo2118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://xw.zhonguo6118.cn

[M03] 执行外部命令
来源：https://wm.zhonguo8118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://kh.zhonguo3118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://bi.zhonguo3118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://qz.zhonguo7118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://zv.zhonguo1118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://gl.zhonguo2118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://tj.zhonguo7118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://bp.zhonguo2118.cn

C#:   Process.Start("ls", "-l");
来源：https://wj.zhonguo3118.cn

[M04] 获取当前工作目录
来源：https://rf.zhonguo7118.cn

Py:   os.getcwd()
来源：https://ei.zhonguo8118.cn

PHP:  getcwd();
来源：https://bz.zhonguo3118.cn

JS:   process.cwd()
来源：https://ex.zhonguo1118.cn

TS:   process.cwd()
来源：https://ab.zhonguo7118.cn

Java: Path.of("").toAbsolutePath()
来源：https://mi.zhonguo7118.cn

Go:   os.Getwd()
来源：https://ka.zhonguo8118.cn

Ruby: Dir.pwd
来源：https://ib.zhonguo6118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ei.zhonguo1118.cn

[M05] 设置退出码
来源：https://hw.zhonguo4118.cn

Py:   sys.exit(1)
来源：https://pd.zhonguo4118.cn

PHP:  exit(1);
来源：https://zs.zhonguo1118.cn

JS:   process.exit(1)
来源：https://gt.zhonguo1118.cn

TS:   process.exit(1)
来源：https://sq.zhonguo2118.cn

Java: System.exit(1)
来源：https://zv.zhonguo5118.cn

Go:   os.Exit(1)
来源：https://jc.zhonguo2118.cn

Ruby: exit 1
来源：https://qn.zhonguo8118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://mh.zhonguo2118.cn

[M06] 向标准错误输出
来源：https://yv.zhonguo8118.cn

Py:   print("err", file=sys.stderr)
来源：https://ex.zhonguo7118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://fv.zhonguo4118.cn

JS:   console.error("err")
来源：https://hu.zhonguo8118.cn

TS:   console.error("err")
来源：https://tf.zhonguo3118.cn

Java: System.err.println("err")
来源：https://pg.zhonguo8118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://ad.zhonguo5118.cn

Ruby: warn "err"
来源：https://rm.zhonguo6118.cn

C#:   Console.Error.WriteLine("err")
来源：https://zq.zhonguo6118.cn

[M07] 判断是否为主入口
来源：https://jr.zhonguo1118.cn

Py:   if __name__ == "__main__":
来源：https://kh.zhonguo6118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://et.zhonguo1118.cn

JS:   require.main === module
来源：https://lg.zhonguo7118.cn

TS:   require.main === module
来源：https://ca.zhonguo7118.cn

Java: public static void main(String[] args)
来源：https://za.zhonguo1118.cn

Go:   func main()
来源：https://oc.zhonguo6118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://er.zhonguo3118.cn

C#:   static void Main(string[] args)
来源：https://aa.zhonguo6118.cn

[M08] 获取系统与运行时信息
来源：https://kd.zhonguo5118.cn

Py:   platform.system();  platform.python_version()
来源：https://xl.zhonguo2118.cn

PHP:  PHP_OS;  phpversion();
来源：https://ob.zhonguo6118.cn

JS:   process.platform;  process.version
来源：https://le.zhonguo4118.cn

TS:   process.platform;  process.version
来源：https://bu.zhonguo8118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://et.zhonguo1118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://es.zhonguo1118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://ux.zhonguo5118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://zq.zhonguo5118.cn

================================================================================
来源：https://ym.zhonguo7118.cn

N. 数据结构与算法
来源：https://lb.zhonguo6118.cn

================================================================================
来源：https://tv.zhonguo1118.cn

[N01] 二分查找（有序数组）
来源：https://lh.zhonguo2118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://lx.zhonguo4118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://cb.zhonguo4118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://rl.zhonguo2118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://mw.zhonguo6118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://bs.zhonguo2118.cn

Go:   sort.SearchInts(arr, x)
来源：https://qo.zhonguo2118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://gg.zhonguo7118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://mi.zhonguo2118.cn

[N02] 排序（工程实践用内置实现）
来源：https://jh.zhonguo5118.cn

Py:   sorted(arr);  arr.sort()
来源：https://pk.zhonguo6118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://lj.zhonguo4118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://ko.zhonguo7118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://zo.zhonguo5118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://mo.zhonguo8118.cn

Go:   slices.Sort(arr)
来源：https://mp.zhonguo5118.cn

Ruby: arr.sort
来源：https://zn.zhonguo7118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://mt.zhonguo5118.cn

[N03] 快速排序（分治示例）
来源：https://af.zhonguo1118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://os.zhonguo5118.cn

PHP:  // 递归实现，或用 usort
来源：https://co.zhonguo1118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://vp.zhonguo7118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://da.zhonguo1118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://gc.zhonguo2118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://vr.zhonguo2118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://tt.zhonguo2118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://qo.zhonguo8118.cn

[N04] 斐波那契数列
来源：https://jg.zhonguo6118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://ox.zhonguo1118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://sn.zhonguo1118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://rz.zhonguo1118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://sa.zhonguo1118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://sy.zhonguo8118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://he.zhonguo5118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://sk.zhonguo8118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://bv.zhonguo2118.cn

[N05] 最大公约数
来源：https://fo.zhonguo5118.cn

Py:   math.gcd(a, b)
来源：https://vw.zhonguo8118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://hx.zhonguo1118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://oy.zhonguo4118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://go.zhonguo1118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://cu.zhonguo1118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://dr.zhonguo7118.cn

Ruby: a.gcd(b)
来源：https://jl.zhonguo2118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://vq.zhonguo8118.cn

[N06] 判断回文字符串
来源：https://nd.zhonguo2118.cn

Py:   s == s[::-1]
来源：https://db.zhonguo5118.cn

PHP:  $s === strrev($s);
来源：https://ye.zhonguo5118.cn

JS:   s === [...s].reverse().join("")
来源：https://lu.zhonguo7118.cn

TS:   s === [...s].reverse().join("")
来源：https://cc.zhonguo3118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://uq.zhonguo6118.cn

Go:   // 双指针从两端比较
来源：https://cn.zhonguo3118.cn

Ruby: s == s.reverse
来源：https://tm.zhonguo7118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://wq.zhonguo5118.cn

[N07] 两数之和（返回下标）
来源：https://sa.zhonguo4118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://my.zhonguo5118.cn


<!-- 参考信息 -->