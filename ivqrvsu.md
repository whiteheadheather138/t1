代发 wailian999

================================================================================
来源：https://ss.zhonguo7118.cn

K. JSON 与序列化
来源：https://vp.zhonguo4118.cn

================================================================================
来源：https://si.zhonguo8118.cn

[K01] 对象转 JSON 字符串
来源：https://qx.zhonguo1118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://xs.zhonguo5118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://ko.zhonguo2118.cn

JS:   JSON.stringify(obj)
来源：https://fx.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://sn.zhonguo5118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://rj.zhonguo4118.cn

Go:   json.Marshal(obj)
来源：https://dn.zhonguo5118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://sq.zhonguo7118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://wv.zhonguo1118.cn

[K02] JSON 字符串转对象
来源：https://tv.zhonguo7118.cn

Py:   json.loads(s)
来源：https://kq.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://fb.zhonguo2118.cn

JS:   JSON.parse(s)
来源：https://uo.zhonguo1118.cn

TS:   JSON.parse(s)
来源：https://pe.zhonguo7118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://in.zhonguo1118.cn

Go:   json.Unmarshal(data, &v)
来源：https://ef.zhonguo6118.cn

Ruby: JSON.parse(s)
来源：https://ct.zhonguo1118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://iu.zhonguo7118.cn

[K03] JSON 美化输出（带缩进）
来源：https://ul.zhonguo3118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://fd.zhonguo6118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://id.zhonguo1118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://ez.zhonguo7118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://qw.zhonguo7118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://ni.zhonguo4118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://gu.zhonguo6118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://oq.zhonguo8118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://ut.zhonguo5118.cn

[K04] 读取 JSON 文件
来源：https://ms.zhonguo1118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://fc.zhonguo5118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://an.zhonguo7118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://jq.zhonguo5118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://sp.zhonguo6118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://bm.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://ld.zhonguo8118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://fc.zhonguo7118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://na.zhonguo4118.cn

[K05] 深拷贝对象
来源：https://xx.zhonguo7118.cn

Py:   copy.deepcopy(obj)
来源：https://ed.zhonguo5118.cn

PHP:  unserialize(serialize($obj));
来源：https://bq.zhonguo4118.cn

JS:   structuredClone(obj)
来源：https://qy.zhonguo5118.cn

TS:   structuredClone(obj)
来源：https://gf.zhonguo8118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ay.zhonguo8118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ro.zhonguo1118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://lg.zhonguo2118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://rp.zhonguo3118.cn

[K06] 解析 URL 查询串
来源：https://fm.zhonguo4118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://fz.zhonguo6118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://ek.zhonguo1118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://st.zhonguo2118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://qb.zhonguo1118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://py.zhonguo3118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://pj.zhonguo5118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://ek.zhonguo1118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://fy.zhonguo3118.cn

[K07] 进制转换
来源：https://nc.zhonguo2118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://pb.zhonguo3118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://mz.zhonguo5118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://vj.zhonguo1118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://bl.zhonguo7118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://rc.zhonguo4118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://de.zhonguo1118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://kw.zhonguo8118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://ca.zhonguo6118.cn

[K08] 二进制序列化（非 JSON）
来源：https://vb.zhonguo4118.cn

Py:   pickle.dumps(obj)
来源：https://lf.zhonguo1118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://bk.zhonguo8118.cn

JS:   v8.serialize(obj)        // Node
来源：https://hs.zhonguo4118.cn

TS:   v8.serialize(obj)        // Node
来源：https://sg.zhonguo2118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://nc.zhonguo4118.cn

Go:   encoding/gob
来源：https://jw.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://yn.zhonguo1118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://fy.zhonguo3118.cn

================================================================================
来源：https://ed.zhonguo8118.cn

L. 网络请求
来源：https://ix.zhonguo6118.cn

================================================================================
来源：https://jx.zhonguo4118.cn

[L01] 发送 GET 请求
来源：https://ql.zhonguo2118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://hv.zhonguo3118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://ra.zhonguo7118.cn

JS:   await fetch(url)
来源：https://mq.zhonguo3118.cn

TS:   await fetch(url)
来源：https://ct.zhonguo2118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://ol.zhonguo5118.cn

Go:   resp, err := http.Get(url)
来源：https://jn.zhonguo6118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://do.zhonguo1118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://li.zhonguo1118.cn

[L02] 发送 POST JSON
来源：https://sw.zhonguo3118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://cn.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://jp.zhonguo4118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://qq.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://gz.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://cf.zhonguo4118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://lm.zhonguo1118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://ae.zhonguo2118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://di.zhonguo2118.cn

[L03] 设置自定义请求头
来源：https://am.zhonguo3118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://iy.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://kb.zhonguo7118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://zw.zhonguo4118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://wc.zhonguo4118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://oy.zhonguo4118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://fe.zhonguo6118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://vt.zhonguo5118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://lb.zhonguo6118.cn

[L04] 设置超时
来源：https://yo.zhonguo6118.cn

Py:   requests.get(url, timeout=5)
来源：https://ve.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://iy.zhonguo2118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://mi.zhonguo5118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://nj.zhonguo6118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://rr.zhonguo6118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://lw.zhonguo5118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://zs.zhonguo4118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://bk.zhonguo2118.cn

[L05] 上传文件（multipart）
来源：https://cv.zhonguo4118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://hr.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://ue.zhonguo5118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://ro.zhonguo1118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://om.zhonguo6118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://zp.zhonguo2118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://jg.zhonguo4118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://hp.zhonguo1118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://dn.zhonguo6118.cn

[L06] 解析响应为 JSON
来源：https://dx.zhonguo3118.cn

Py:   resp.json()
来源：https://vk.zhonguo5118.cn

PHP:  json_decode($body, true);
来源：https://ss.zhonguo8118.cn

JS:   await resp.json()
来源：https://tz.zhonguo1118.cn

TS:   await resp.json()
来源：https://ru.zhonguo6118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://fr.zhonguo4118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://fz.zhonguo5118.cn

Ruby: JSON.parse(resp.body)
来源：https://fn.zhonguo8118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://xh.zhonguo5118.cn

[L07] 处理 HTTP 状态码
来源：https://dq.zhonguo6118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://gq.zhonguo6118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://ef.zhonguo7118.cn

JS:   resp.ok;  resp.status
来源：https://xw.zhonguo2118.cn

TS:   resp.ok;  resp.status
来源：https://vs.zhonguo5118.cn

Java: resp.statusCode()
来源：https://vw.zhonguo5118.cn

Go:   resp.StatusCode
来源：https://bq.zhonguo2118.cn

Ruby: resp.code.to_i
来源：https://js.zhonguo1118.cn

C#:   (int)resp.StatusCode
来源：https://xi.zhonguo8118.cn

[L08] 并发请求多个地址
来源：https://co.zhonguo4118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://ku.zhonguo1118.cn

PHP:  curl_multi_init() 系列
来源：https://kf.zhonguo3118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://bz.zhonguo3118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://fz.zhonguo5118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://iu.zhonguo7118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://tz.zhonguo5118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://xv.zhonguo1118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://sb.zhonguo4118.cn

================================================================================
来源：https://pw.zhonguo3118.cn

M. 命令行 / 进程 / 环境
来源：https://ec.zhonguo2118.cn

================================================================================
来源：https://sa.zhonguo5118.cn

[M01] 读取命令行参数
来源：https://qg.zhonguo4118.cn

Py:   sys.argv[1:]
来源：https://yn.zhonguo3118.cn

PHP:  $argv;  $argc;
来源：https://yw.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://wq.zhonguo7118.cn

TS:   process.argv.slice(2)
来源：https://qv.zhonguo1118.cn

Java: args 数组（main 方法参数）
来源：https://dm.zhonguo4118.cn

Go:   os.Args[1:]
来源：https://ar.zhonguo3118.cn

Ruby: ARGV
来源：https://vk.zhonguo7118.cn

C#:   args 数组（Main 方法参数）
来源：https://ix.zhonguo7118.cn

[M02] 读取环境变量
来源：https://rb.zhonguo8118.cn

Py:   os.environ.get("HOME")
来源：https://gp.zhonguo8118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://qj.zhonguo1118.cn

JS:   process.env.HOME
来源：https://yh.zhonguo2118.cn

TS:   process.env.HOME
来源：https://er.zhonguo2118.cn

Java: System.getenv("HOME")
来源：https://pk.zhonguo4118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://qj.zhonguo5118.cn

Ruby: ENV["HOME"]
来源：https://cg.zhonguo4118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://gb.zhonguo8118.cn

[M03] 执行外部命令
来源：https://qk.zhonguo7118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://sz.zhonguo7118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://mb.zhonguo4118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://hy.zhonguo1118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://mw.zhonguo2118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://zg.zhonguo1118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://mb.zhonguo1118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://ff.zhonguo4118.cn

C#:   Process.Start("ls", "-l");
来源：https://xs.zhonguo7118.cn

[M04] 获取当前工作目录
来源：https://ql.zhonguo5118.cn

Py:   os.getcwd()
来源：https://je.zhonguo4118.cn

PHP:  getcwd();
来源：https://cr.zhonguo3118.cn

JS:   process.cwd()
来源：https://xd.zhonguo8118.cn

TS:   process.cwd()
来源：https://at.zhonguo3118.cn

Java: Path.of("").toAbsolutePath()
来源：https://le.zhonguo8118.cn

Go:   os.Getwd()
来源：https://pm.zhonguo2118.cn

Ruby: Dir.pwd
来源：https://ry.zhonguo6118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ch.zhonguo2118.cn

[M05] 设置退出码
来源：https://yw.zhonguo3118.cn

Py:   sys.exit(1)
来源：https://yq.zhonguo2118.cn

PHP:  exit(1);
来源：https://fg.zhonguo2118.cn

JS:   process.exit(1)
来源：https://gz.zhonguo6118.cn

TS:   process.exit(1)
来源：https://dp.zhonguo6118.cn

Java: System.exit(1)
来源：https://fr.zhonguo5118.cn

Go:   os.Exit(1)
来源：https://vf.zhonguo6118.cn

Ruby: exit 1
来源：https://kz.zhonguo4118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://ov.zhonguo8118.cn

[M06] 向标准错误输出
来源：https://fd.zhonguo6118.cn

Py:   print("err", file=sys.stderr)
来源：https://xg.zhonguo3118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://eu.zhonguo5118.cn

JS:   console.error("err")
来源：https://an.zhonguo6118.cn

TS:   console.error("err")
来源：https://rl.zhonguo7118.cn

Java: System.err.println("err")
来源：https://fk.zhonguo6118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://el.zhonguo3118.cn

Ruby: warn "err"
来源：https://tz.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://am.zhonguo2118.cn

[M07] 判断是否为主入口
来源：https://wz.zhonguo1118.cn

Py:   if __name__ == "__main__":
来源：https://fs.zhonguo4118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://re.zhonguo3118.cn

JS:   require.main === module
来源：https://ux.zhonguo6118.cn

TS:   require.main === module
来源：https://gm.zhonguo8118.cn

Java: public static void main(String[] args)
来源：https://ds.zhonguo4118.cn

Go:   func main()
来源：https://sy.zhonguo4118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://yu.zhonguo5118.cn

C#:   static void Main(string[] args)
来源：https://yc.zhonguo8118.cn

[M08] 获取系统与运行时信息
来源：https://cx.zhonguo4118.cn

Py:   platform.system();  platform.python_version()
来源：https://qy.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://wt.zhonguo4118.cn

JS:   process.platform;  process.version
来源：https://lm.zhonguo8118.cn

TS:   process.platform;  process.version
来源：https://ba.zhonguo6118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://st.zhonguo6118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://ij.zhonguo4118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://up.zhonguo6118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://ot.zhonguo2118.cn

================================================================================
来源：https://md.zhonguo1118.cn

N. 数据结构与算法
来源：https://lc.zhonguo8118.cn

================================================================================
来源：https://zn.zhonguo4118.cn

[N01] 二分查找（有序数组）
来源：https://ss.zhonguo6118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://es.zhonguo8118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://jo.zhonguo2118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://vu.zhonguo8118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://dd.zhonguo2118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://pc.zhonguo4118.cn

Go:   sort.SearchInts(arr, x)
来源：https://xh.zhonguo1118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://uy.zhonguo6118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://bf.zhonguo5118.cn

[N02] 排序（工程实践用内置实现）
来源：https://tv.zhonguo5118.cn

Py:   sorted(arr);  arr.sort()
来源：https://dx.zhonguo2118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://zx.zhonguo4118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://wf.zhonguo2118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://gf.zhonguo8118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://fk.zhonguo2118.cn

Go:   slices.Sort(arr)
来源：https://do.zhonguo1118.cn

Ruby: arr.sort
来源：https://xs.zhonguo6118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://ln.zhonguo2118.cn

[N03] 快速排序（分治示例）
来源：https://qv.zhonguo3118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://li.zhonguo7118.cn

PHP:  // 递归实现，或用 usort
来源：https://bv.zhonguo8118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://zw.zhonguo3118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://qj.zhonguo4118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://wi.zhonguo7118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://gq.zhonguo3118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://yw.zhonguo7118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://mv.zhonguo2118.cn

[N04] 斐波那契数列
来源：https://if.zhonguo4118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://fx.zhonguo3118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://mx.zhonguo3118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://bo.zhonguo7118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://wu.zhonguo5118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://gd.zhonguo6118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://cq.zhonguo7118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://qk.zhonguo2118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://xg.zhonguo3118.cn

[N05] 最大公约数
来源：https://ae.zhonguo7118.cn

Py:   math.gcd(a, b)
来源：https://bz.zhonguo7118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://gr.zhonguo4118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://xq.zhonguo2118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://xn.zhonguo6118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://fx.zhonguo7118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://lu.zhonguo1118.cn

Ruby: a.gcd(b)
来源：https://hv.zhonguo8118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://fb.zhonguo7118.cn

[N06] 判断回文字符串
来源：https://bv.zhonguo2118.cn

Py:   s == s[::-1]
来源：https://dn.zhonguo1118.cn

PHP:  $s === strrev($s);
来源：https://wv.zhonguo6118.cn

JS:   s === [...s].reverse().join("")
来源：https://vh.zhonguo2118.cn

TS:   s === [...s].reverse().join("")
来源：https://nx.zhonguo2118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://fn.zhonguo8118.cn

Go:   // 双指针从两端比较
来源：https://rp.zhonguo1118.cn

Ruby: s == s.reverse
来源：https://in.zhonguo4118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://up.zhonguo5118.cn

[N07] 两数之和（返回下标）
来源：https://jn.zhonguo3118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://cb.zhonguo3118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://zw.zhonguo3118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://fx.zhonguo2118.cn

TS:   // 手写 Map<string, number>
来源：https://mg.zhonguo4118.cn

Java: // 手写 HashMap
来源：https://um.zhonguo3118.cn

Go:   // 手写 map[int]int
来源：https://sv.zhonguo2118.cn

Ruby: // 手写 Hash
来源：https://dv.zhonguo3118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://jy.zhonguo6118.cn

[N08] 生成全排列
来源：https://xt.zhonguo1118.cn

Py:   itertools.permutations(arr)
来源：https://mp.zhonguo2118.cn

PHP:  // 手写递归交换
来源：https://db.zhonguo6118.cn

JS:   // 手写回溯递归
来源：https://wd.zhonguo3118.cn

TS:   // 手写回溯递归
来源：https://uk.zhonguo5118.cn

Java: // 手写回溯递归
来源：https://hw.zhonguo8118.cn

Go:   // 手写回溯递归
来源：https://px.zhonguo2118.cn

Ruby: arr.permutation.to_a
来源：https://kw.zhonguo1118.cn

C#:   // 手写回溯递归
来源：https://jh.zhonguo4118.cn


<!-- 参考信息 -->