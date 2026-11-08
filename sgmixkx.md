代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ve.zhonguo3118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://ck.zhonguo7118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://rd.zhonguo6118.cn

[J10] 取今天 / 本月第一天
来源：https://an.zhonguo5118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://zr.zhonguo2118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://lr.zhonguo6118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://vk.zhonguo5118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://vz.zhonguo4118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://xl.zhonguo8118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://fw.zhonguo6118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://kl.zhonguo4118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://cg.zhonguo5118.cn

================================================================================
来源：https://ya.zhonguo1118.cn

K. JSON 与序列化
来源：https://zp.zhonguo1118.cn

================================================================================
来源：https://jk.zhonguo2118.cn

[K01] 对象转 JSON 字符串
来源：https://xt.zhonguo5118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://rt.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://jg.zhonguo5118.cn

JS:   JSON.stringify(obj)
来源：https://jz.zhonguo2118.cn

TS:   JSON.stringify(obj)
来源：https://ba.zhonguo3118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://ts.zhonguo8118.cn

Go:   json.Marshal(obj)
来源：https://ag.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://in.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://wp.zhonguo3118.cn

[K02] JSON 字符串转对象
来源：https://fe.zhonguo2118.cn

Py:   json.loads(s)
来源：https://ue.zhonguo8118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://jv.zhonguo7118.cn

JS:   JSON.parse(s)
来源：https://zj.zhonguo2118.cn

TS:   JSON.parse(s)
来源：https://do.zhonguo3118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://kd.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://pw.zhonguo7118.cn

Ruby: JSON.parse(s)
来源：https://ij.zhonguo7118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://ls.zhonguo5118.cn

[K03] JSON 美化输出（带缩进）
来源：https://gr.zhonguo6118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://bj.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://tx.zhonguo8118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://ub.zhonguo3118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://bs.zhonguo8118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://sd.zhonguo5118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://vk.zhonguo8118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://pq.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://nl.zhonguo7118.cn

[K04] 读取 JSON 文件
来源：https://rl.zhonguo8118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://qd.zhonguo4118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://kf.zhonguo5118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://qp.zhonguo5118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://sr.zhonguo1118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://el.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://ei.zhonguo3118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://qd.zhonguo3118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://gt.zhonguo6118.cn

[K05] 深拷贝对象
来源：https://jr.zhonguo2118.cn

Py:   copy.deepcopy(obj)
来源：https://pt.zhonguo3118.cn

PHP:  unserialize(serialize($obj));
来源：https://ef.zhonguo5118.cn

JS:   structuredClone(obj)
来源：https://vo.zhonguo8118.cn

TS:   structuredClone(obj)
来源：https://na.zhonguo7118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ks.zhonguo2118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ra.zhonguo8118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://kw.zhonguo4118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://sp.zhonguo7118.cn

[K06] 解析 URL 查询串
来源：https://ms.zhonguo4118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://oe.zhonguo5118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://bv.zhonguo1118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://tn.zhonguo5118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ms.zhonguo8118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://bf.zhonguo2118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://si.zhonguo2118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://sx.zhonguo5118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://zd.zhonguo4118.cn

[K07] 进制转换
来源：https://kj.zhonguo8118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://mv.zhonguo1118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://wz.zhonguo3118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://ur.zhonguo1118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://xv.zhonguo6118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://wo.zhonguo7118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://pw.zhonguo4118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://sv.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://qi.zhonguo2118.cn

[K08] 二进制序列化（非 JSON）
来源：https://qd.zhonguo8118.cn

Py:   pickle.dumps(obj)
来源：https://zc.zhonguo1118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://lv.zhonguo8118.cn

JS:   v8.serialize(obj)        // Node
来源：https://sg.zhonguo5118.cn

TS:   v8.serialize(obj)        // Node
来源：https://au.zhonguo8118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://te.zhonguo3118.cn

Go:   encoding/gob
来源：https://fv.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://bw.zhonguo4118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://sz.zhonguo1118.cn

================================================================================
来源：https://ue.zhonguo3118.cn

L. 网络请求
来源：https://wu.zhonguo1118.cn

================================================================================
来源：https://ne.zhonguo8118.cn

[L01] 发送 GET 请求
来源：https://hf.zhonguo5118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://cb.zhonguo3118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://le.zhonguo8118.cn

JS:   await fetch(url)
来源：https://rn.zhonguo3118.cn

TS:   await fetch(url)
来源：https://ft.zhonguo8118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://qy.zhonguo2118.cn

Go:   resp, err := http.Get(url)
来源：https://ld.zhonguo2118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://ei.zhonguo8118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://qd.zhonguo5118.cn

[L02] 发送 POST JSON
来源：https://yh.zhonguo7118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://vi.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://tg.zhonguo6118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://kc.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://ge.zhonguo5118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://jr.zhonguo4118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://ut.zhonguo1118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://xh.zhonguo3118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://pl.zhonguo3118.cn

[L03] 设置自定义请求头
来源：https://qu.zhonguo4118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://om.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://co.zhonguo3118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://fq.zhonguo1118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://gm.zhonguo5118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://ud.zhonguo5118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://pn.zhonguo7118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://ki.zhonguo4118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://vd.zhonguo1118.cn

[L04] 设置超时
来源：https://gx.zhonguo8118.cn

Py:   requests.get(url, timeout=5)
来源：https://kk.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://ts.zhonguo8118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://wc.zhonguo6118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://rf.zhonguo4118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://xv.zhonguo8118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://jq.zhonguo6118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://zr.zhonguo6118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://ks.zhonguo5118.cn

[L05] 上传文件（multipart）
来源：https://ze.zhonguo8118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://za.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://mj.zhonguo7118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://bu.zhonguo3118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://sc.zhonguo2118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://xz.zhonguo3118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://tu.zhonguo4118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ua.zhonguo6118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://ot.zhonguo2118.cn

[L06] 解析响应为 JSON
来源：https://na.zhonguo7118.cn

Py:   resp.json()
来源：https://na.zhonguo3118.cn

PHP:  json_decode($body, true);
来源：https://fc.zhonguo8118.cn

JS:   await resp.json()
来源：https://mf.zhonguo3118.cn

TS:   await resp.json()
来源：https://yy.zhonguo8118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://fg.zhonguo5118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://jx.zhonguo3118.cn

Ruby: JSON.parse(resp.body)
来源：https://ev.zhonguo5118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://nf.zhonguo3118.cn

[L07] 处理 HTTP 状态码
来源：https://ts.zhonguo4118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://ab.zhonguo3118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://et.zhonguo8118.cn

JS:   resp.ok;  resp.status
来源：https://oh.zhonguo1118.cn

TS:   resp.ok;  resp.status
来源：https://zk.zhonguo4118.cn

Java: resp.statusCode()
来源：https://sf.zhonguo8118.cn

Go:   resp.StatusCode
来源：https://hd.zhonguo2118.cn

Ruby: resp.code.to_i
来源：https://an.zhonguo4118.cn

C#:   (int)resp.StatusCode
来源：https://ya.zhonguo7118.cn

[L08] 并发请求多个地址
来源：https://ze.zhonguo5118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://ix.zhonguo1118.cn

PHP:  curl_multi_init() 系列
来源：https://qs.zhonguo7118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ri.zhonguo5118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ly.zhonguo1118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://hw.zhonguo4118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://sl.zhonguo1118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://cb.zhonguo1118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://ur.zhonguo8118.cn

================================================================================
来源：https://dh.zhonguo2118.cn

M. 命令行 / 进程 / 环境
来源：https://ao.zhonguo4118.cn

================================================================================
来源：https://rz.zhonguo2118.cn

[M01] 读取命令行参数
来源：https://hl.zhonguo3118.cn

Py:   sys.argv[1:]
来源：https://nz.zhonguo2118.cn

PHP:  $argv;  $argc;
来源：https://kc.zhonguo1118.cn

JS:   process.argv.slice(2)
来源：https://xo.zhonguo4118.cn

TS:   process.argv.slice(2)
来源：https://yy.zhonguo8118.cn

Java: args 数组（main 方法参数）
来源：https://ml.zhonguo4118.cn

Go:   os.Args[1:]
来源：https://ys.zhonguo5118.cn

Ruby: ARGV
来源：https://uo.zhonguo3118.cn

C#:   args 数组（Main 方法参数）
来源：https://mp.zhonguo5118.cn

[M02] 读取环境变量
来源：https://xn.zhonguo8118.cn

Py:   os.environ.get("HOME")
来源：https://uh.zhonguo4118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://kc.zhonguo8118.cn

JS:   process.env.HOME
来源：https://dq.zhonguo2118.cn

TS:   process.env.HOME
来源：https://bo.zhonguo6118.cn

Java: System.getenv("HOME")
来源：https://ev.zhonguo8118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://io.zhonguo1118.cn

Ruby: ENV["HOME"]
来源：https://rf.zhonguo7118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://wb.zhonguo6118.cn

[M03] 执行外部命令
来源：https://mq.zhonguo7118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://ok.zhonguo3118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://mn.zhonguo6118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://ey.zhonguo1118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://ww.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://oc.zhonguo4118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://hm.zhonguo6118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://ex.zhonguo4118.cn

C#:   Process.Start("ls", "-l");
来源：https://jf.zhonguo3118.cn

[M04] 获取当前工作目录
来源：https://uz.zhonguo7118.cn

Py:   os.getcwd()
来源：https://do.zhonguo4118.cn

PHP:  getcwd();
来源：https://hf.zhonguo3118.cn

JS:   process.cwd()
来源：https://uv.zhonguo7118.cn

TS:   process.cwd()
来源：https://kp.zhonguo4118.cn

Java: Path.of("").toAbsolutePath()
来源：https://nx.zhonguo6118.cn

Go:   os.Getwd()
来源：https://xu.zhonguo3118.cn

Ruby: Dir.pwd
来源：https://bh.zhonguo4118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://sr.zhonguo6118.cn

[M05] 设置退出码
来源：https://vk.zhonguo8118.cn

Py:   sys.exit(1)
来源：https://pv.zhonguo6118.cn

PHP:  exit(1);
来源：https://eb.zhonguo1118.cn

JS:   process.exit(1)
来源：https://eu.zhonguo1118.cn

TS:   process.exit(1)
来源：https://tt.zhonguo7118.cn

Java: System.exit(1)
来源：https://pc.zhonguo6118.cn

Go:   os.Exit(1)
来源：https://yw.zhonguo7118.cn

Ruby: exit 1
来源：https://bd.zhonguo2118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://pq.zhonguo5118.cn

[M06] 向标准错误输出
来源：https://lu.zhonguo2118.cn

Py:   print("err", file=sys.stderr)
来源：https://rj.zhonguo1118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://fw.zhonguo1118.cn

JS:   console.error("err")
来源：https://ev.zhonguo2118.cn

TS:   console.error("err")
来源：https://iz.zhonguo2118.cn

Java: System.err.println("err")
来源：https://xo.zhonguo7118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://wk.zhonguo2118.cn

Ruby: warn "err"
来源：https://me.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://zm.zhonguo6118.cn

[M07] 判断是否为主入口
来源：https://cy.zhonguo2118.cn

Py:   if __name__ == "__main__":
来源：https://ov.zhonguo8118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://em.zhonguo2118.cn

JS:   require.main === module
来源：https://hv.zhonguo4118.cn

TS:   require.main === module
来源：https://gt.zhonguo2118.cn

Java: public static void main(String[] args)
来源：https://dg.zhonguo8118.cn

Go:   func main()
来源：https://il.zhonguo1118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://fh.zhonguo6118.cn

C#:   static void Main(string[] args)
来源：https://wv.zhonguo4118.cn

[M08] 获取系统与运行时信息
来源：https://sc.zhonguo3118.cn

Py:   platform.system();  platform.python_version()
来源：https://dg.zhonguo4118.cn

PHP:  PHP_OS;  phpversion();
来源：https://mi.zhonguo6118.cn

JS:   process.platform;  process.version
来源：https://aq.zhonguo2118.cn

TS:   process.platform;  process.version
来源：https://ds.zhonguo5118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://yh.zhonguo7118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://nk.zhonguo8118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://bh.zhonguo7118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://kc.zhonguo3118.cn

================================================================================
来源：https://oe.zhonguo2118.cn

N. 数据结构与算法
来源：https://sn.zhonguo1118.cn

================================================================================
来源：https://gu.zhonguo2118.cn

[N01] 二分查找（有序数组）
来源：https://sj.zhonguo4118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://yr.zhonguo5118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://mo.zhonguo5118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://ka.zhonguo6118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://ve.zhonguo3118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://ls.zhonguo5118.cn

Go:   sort.SearchInts(arr, x)
来源：https://xr.zhonguo6118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://ax.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://od.zhonguo7118.cn

[N02] 排序（工程实践用内置实现）
来源：https://of.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://lw.zhonguo4118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://og.zhonguo7118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://fd.zhonguo3118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://ki.zhonguo4118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://kk.zhonguo3118.cn

Go:   slices.Sort(arr)
来源：https://in.zhonguo7118.cn

Ruby: arr.sort
来源：https://ts.zhonguo7118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://mb.zhonguo3118.cn

[N03] 快速排序（分治示例）
来源：https://hz.zhonguo4118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://oo.zhonguo7118.cn

PHP:  // 递归实现，或用 usort
来源：https://yd.zhonguo7118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://we.zhonguo1118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://nq.zhonguo7118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://me.zhonguo4118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://tr.zhonguo5118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://hm.zhonguo6118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://iv.zhonguo3118.cn

[N04] 斐波那契数列
来源：https://wl.zhonguo6118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://ge.zhonguo8118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://yq.zhonguo7118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ai.zhonguo6118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://rk.zhonguo1118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://iy.zhonguo3118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://sm.zhonguo2118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://mo.zhonguo2118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://wo.zhonguo1118.cn

[N05] 最大公约数
来源：https://db.zhonguo3118.cn

Py:   math.gcd(a, b)
来源：https://gi.zhonguo3118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://vh.zhonguo3118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://rt.zhonguo6118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://mz.zhonguo4118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://jo.zhonguo7118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://bt.zhonguo4118.cn

Ruby: a.gcd(b)
来源：https://lp.zhonguo6118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://av.zhonguo4118.cn

[N06] 判断回文字符串
来源：https://wr.zhonguo3118.cn

Py:   s == s[::-1]
来源：https://nk.zhonguo3118.cn

PHP:  $s === strrev($s);
来源：https://yg.zhonguo6118.cn

JS:   s === [...s].reverse().join("")
来源：https://uz.zhonguo3118.cn

TS:   s === [...s].reverse().join("")
来源：https://cc.zhonguo5118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://xh.zhonguo7118.cn

Go:   // 双指针从两端比较
来源：https://tg.zhonguo5118.cn

Ruby: s == s.reverse
来源：https://wz.zhonguo6118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://gq.zhonguo3118.cn

[N07] 两数之和（返回下标）
来源：https://fy.zhonguo7118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://yc.zhonguo4118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://dl.zhonguo7118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://ip.zhonguo4118.cn

TS:   // 手写 Map<string, number>
来源：https://uj.zhonguo2118.cn

Java: // 手写 HashMap
来源：https://eg.zhonguo1118.cn


<!-- 参考信息 -->