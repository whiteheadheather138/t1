代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://vs.zhonguo6118.cn

[K03] JSON 美化输出（带缩进）
来源：https://nf.zhonguo3118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://jb.zhonguo2118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://vq.zhonguo5118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://wx.zhonguo2118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://gc.zhonguo6118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://es.zhonguo1118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://ll.zhonguo8118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://nl.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://hy.zhonguo7118.cn

[K04] 读取 JSON 文件
来源：https://yh.zhonguo8118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://pu.zhonguo3118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://ro.zhonguo5118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ab.zhonguo5118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://rr.zhonguo3118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://hf.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://qb.zhonguo2118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://is.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://cu.zhonguo5118.cn

[K05] 深拷贝对象
来源：https://zv.zhonguo8118.cn

Py:   copy.deepcopy(obj)
来源：https://tv.zhonguo3118.cn

PHP:  unserialize(serialize($obj));
来源：https://jx.zhonguo2118.cn

JS:   structuredClone(obj)
来源：https://jj.zhonguo3118.cn

TS:   structuredClone(obj)
来源：https://yq.zhonguo3118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://rj.zhonguo8118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://xa.zhonguo3118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://fp.zhonguo8118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://hj.zhonguo4118.cn

[K06] 解析 URL 查询串
来源：https://dd.zhonguo1118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://or.zhonguo2118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://ef.zhonguo3118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://qe.zhonguo7118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://pt.zhonguo1118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://il.zhonguo8118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://lh.zhonguo1118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://vy.zhonguo5118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://vu.zhonguo1118.cn

[K07] 进制转换
来源：https://az.zhonguo1118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://ih.zhonguo2118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://fi.zhonguo3118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://uc.zhonguo5118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://xf.zhonguo5118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://lk.zhonguo5118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ht.zhonguo3118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://fw.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://qd.zhonguo5118.cn

[K08] 二进制序列化（非 JSON）
来源：https://nv.zhonguo6118.cn

Py:   pickle.dumps(obj)
来源：https://ty.zhonguo5118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://sy.zhonguo3118.cn

JS:   v8.serialize(obj)        // Node
来源：https://ct.zhonguo5118.cn

TS:   v8.serialize(obj)        // Node
来源：https://gw.zhonguo8118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://gv.zhonguo2118.cn

Go:   encoding/gob
来源：https://ib.zhonguo5118.cn

Ruby: Marshal.dump(obj)
来源：https://gk.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://xw.zhonguo2118.cn

================================================================================
来源：https://db.zhonguo5118.cn

L. 网络请求
来源：https://ex.zhonguo6118.cn

================================================================================
来源：https://ek.zhonguo2118.cn

[L01] 发送 GET 请求
来源：https://fj.zhonguo3118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://xr.zhonguo1118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://oi.zhonguo3118.cn

JS:   await fetch(url)
来源：https://kt.zhonguo6118.cn

TS:   await fetch(url)
来源：https://ln.zhonguo4118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://pv.zhonguo5118.cn

Go:   resp, err := http.Get(url)
来源：https://tz.zhonguo1118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://uf.zhonguo6118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://rv.zhonguo5118.cn

[L02] 发送 POST JSON
来源：https://se.zhonguo8118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://jy.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://mz.zhonguo7118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://cr.zhonguo5118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://ii.zhonguo4118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://mi.zhonguo5118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://gc.zhonguo7118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://xs.zhonguo1118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://vf.zhonguo4118.cn

[L03] 设置自定义请求头
来源：https://zi.zhonguo5118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://nq.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://cy.zhonguo1118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ln.zhonguo7118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://da.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://ez.zhonguo5118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://cl.zhonguo4118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://ah.zhonguo4118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://sx.zhonguo8118.cn

[L04] 设置超时
来源：https://hs.zhonguo6118.cn

Py:   requests.get(url, timeout=5)
来源：https://mc.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://xu.zhonguo2118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://ql.zhonguo1118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://bb.zhonguo5118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://pg.zhonguo6118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://wk.zhonguo3118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://fc.zhonguo8118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://mg.zhonguo7118.cn

[L05] 上传文件（multipart）
来源：https://sh.zhonguo6118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://gd.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://zi.zhonguo8118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://wu.zhonguo3118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://qa.zhonguo4118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://co.zhonguo7118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://bp.zhonguo1118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://im.zhonguo6118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://bp.zhonguo4118.cn

[L06] 解析响应为 JSON
来源：https://bd.zhonguo5118.cn

Py:   resp.json()
来源：https://lp.zhonguo6118.cn

PHP:  json_decode($body, true);
来源：https://oz.zhonguo1118.cn

JS:   await resp.json()
来源：https://gy.zhonguo2118.cn

TS:   await resp.json()
来源：https://oo.zhonguo5118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://lt.zhonguo7118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://jd.zhonguo7118.cn

Ruby: JSON.parse(resp.body)
来源：https://te.zhonguo2118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://hf.zhonguo7118.cn

[L07] 处理 HTTP 状态码
来源：https://tg.zhonguo3118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://gb.zhonguo5118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://rj.zhonguo1118.cn

JS:   resp.ok;  resp.status
来源：https://se.zhonguo3118.cn

TS:   resp.ok;  resp.status
来源：https://aj.zhonguo5118.cn

Java: resp.statusCode()
来源：https://jt.zhonguo4118.cn

Go:   resp.StatusCode
来源：https://oo.zhonguo2118.cn

Ruby: resp.code.to_i
来源：https://ch.zhonguo1118.cn

C#:   (int)resp.StatusCode
来源：https://ou.zhonguo2118.cn

[L08] 并发请求多个地址
来源：https://zo.zhonguo4118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://pc.zhonguo6118.cn

PHP:  curl_multi_init() 系列
来源：https://sd.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://uc.zhonguo1118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://jk.zhonguo6118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://vk.zhonguo7118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://ey.zhonguo3118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://ty.zhonguo4118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://ki.zhonguo2118.cn

================================================================================
来源：https://oq.zhonguo7118.cn

M. 命令行 / 进程 / 环境
来源：https://hz.zhonguo3118.cn

================================================================================
来源：https://hy.zhonguo7118.cn

[M01] 读取命令行参数
来源：https://ns.zhonguo1118.cn

Py:   sys.argv[1:]
来源：https://hs.zhonguo5118.cn

PHP:  $argv;  $argc;
来源：https://jq.zhonguo4118.cn

JS:   process.argv.slice(2)
来源：https://uk.zhonguo1118.cn

TS:   process.argv.slice(2)
来源：https://ux.zhonguo5118.cn

Java: args 数组（main 方法参数）
来源：https://au.zhonguo6118.cn

Go:   os.Args[1:]
来源：https://jw.zhonguo7118.cn

Ruby: ARGV
来源：https://bt.zhonguo5118.cn

C#:   args 数组（Main 方法参数）
来源：https://ow.zhonguo6118.cn

[M02] 读取环境变量
来源：https://sq.zhonguo2118.cn

Py:   os.environ.get("HOME")
来源：https://zh.zhonguo4118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://gb.zhonguo1118.cn

JS:   process.env.HOME
来源：https://nc.zhonguo6118.cn

TS:   process.env.HOME
来源：https://so.zhonguo3118.cn

Java: System.getenv("HOME")
来源：https://ah.zhonguo6118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://il.zhonguo6118.cn

Ruby: ENV["HOME"]
来源：https://vr.zhonguo8118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://si.zhonguo3118.cn

[M03] 执行外部命令
来源：https://xt.zhonguo7118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://he.zhonguo5118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://rp.zhonguo2118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://xs.zhonguo4118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://jh.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://ou.zhonguo3118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://ld.zhonguo7118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://bs.zhonguo1118.cn

C#:   Process.Start("ls", "-l");
来源：https://ej.zhonguo8118.cn

[M04] 获取当前工作目录
来源：https://yi.zhonguo3118.cn

Py:   os.getcwd()
来源：https://lc.zhonguo1118.cn

PHP:  getcwd();
来源：https://wm.zhonguo7118.cn

JS:   process.cwd()
来源：https://to.zhonguo3118.cn

TS:   process.cwd()
来源：https://sx.zhonguo5118.cn

Java: Path.of("").toAbsolutePath()
来源：https://cn.zhonguo4118.cn

Go:   os.Getwd()
来源：https://xn.zhonguo5118.cn

Ruby: Dir.pwd
来源：https://bk.zhonguo5118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://lh.zhonguo8118.cn

[M05] 设置退出码
来源：https://po.zhonguo4118.cn

Py:   sys.exit(1)
来源：https://nx.zhonguo6118.cn

PHP:  exit(1);
来源：https://ts.zhonguo7118.cn

JS:   process.exit(1)
来源：https://tp.zhonguo5118.cn

TS:   process.exit(1)
来源：https://yt.zhonguo7118.cn

Java: System.exit(1)
来源：https://db.zhonguo1118.cn

Go:   os.Exit(1)
来源：https://yp.zhonguo2118.cn

Ruby: exit 1
来源：https://nu.zhonguo7118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://ii.zhonguo6118.cn

[M06] 向标准错误输出
来源：https://ve.zhonguo3118.cn

Py:   print("err", file=sys.stderr)
来源：https://qp.zhonguo5118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://am.zhonguo8118.cn

JS:   console.error("err")
来源：https://wk.zhonguo2118.cn

TS:   console.error("err")
来源：https://rv.zhonguo4118.cn

Java: System.err.println("err")
来源：https://ax.zhonguo3118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://uo.zhonguo7118.cn

Ruby: warn "err"
来源：https://fz.zhonguo7118.cn

C#:   Console.Error.WriteLine("err")
来源：https://zo.zhonguo4118.cn

[M07] 判断是否为主入口
来源：https://zp.zhonguo3118.cn

Py:   if __name__ == "__main__":
来源：https://iq.zhonguo5118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://ta.zhonguo2118.cn

JS:   require.main === module
来源：https://rw.zhonguo1118.cn

TS:   require.main === module
来源：https://ru.zhonguo7118.cn

Java: public static void main(String[] args)
来源：https://gj.zhonguo4118.cn

Go:   func main()
来源：https://vw.zhonguo4118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://jm.zhonguo1118.cn

C#:   static void Main(string[] args)
来源：https://ke.zhonguo8118.cn

[M08] 获取系统与运行时信息
来源：https://we.zhonguo8118.cn

Py:   platform.system();  platform.python_version()
来源：https://lc.zhonguo8118.cn

PHP:  PHP_OS;  phpversion();
来源：https://jp.zhonguo7118.cn

JS:   process.platform;  process.version
来源：https://oq.zhonguo2118.cn

TS:   process.platform;  process.version
来源：https://jd.zhonguo6118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://fa.zhonguo8118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://sh.zhonguo8118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://qa.zhonguo1118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://gt.zhonguo8118.cn

================================================================================
来源：https://yj.zhonguo8118.cn

N. 数据结构与算法
来源：https://gl.zhonguo4118.cn

================================================================================
来源：https://qf.zhonguo8118.cn

[N01] 二分查找（有序数组）
来源：https://zs.zhonguo5118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://pt.zhonguo1118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://vw.zhonguo1118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://eu.zhonguo2118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://qn.zhonguo4118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://lp.zhonguo5118.cn

Go:   sort.SearchInts(arr, x)
来源：https://ew.zhonguo3118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://ew.zhonguo7118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://st.zhonguo2118.cn

[N02] 排序（工程实践用内置实现）
来源：https://ns.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://oh.zhonguo3118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://qc.zhonguo5118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://vz.zhonguo5118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://dy.zhonguo8118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://sx.zhonguo8118.cn

Go:   slices.Sort(arr)
来源：https://ku.zhonguo5118.cn

Ruby: arr.sort
来源：https://tt.zhonguo1118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://ui.zhonguo6118.cn

[N03] 快速排序（分治示例）
来源：https://ef.zhonguo8118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://ku.zhonguo3118.cn

PHP:  // 递归实现，或用 usort
来源：https://pn.zhonguo4118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://ui.zhonguo3118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://lc.zhonguo2118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://ce.zhonguo1118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://uc.zhonguo8118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://cf.zhonguo1118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://vf.zhonguo8118.cn

[N04] 斐波那契数列
来源：https://jm.zhonguo2118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://ok.zhonguo3118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://ok.zhonguo7118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://es.zhonguo2118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://uc.zhonguo5118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://cu.zhonguo5118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://te.zhonguo1118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://kl.zhonguo3118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://ea.zhonguo8118.cn

[N05] 最大公约数
来源：https://qu.zhonguo7118.cn

Py:   math.gcd(a, b)
来源：https://xc.zhonguo3118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://xy.zhonguo1118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://hc.zhonguo1118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://vm.zhonguo7118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://zo.zhonguo1118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://fb.zhonguo3118.cn

Ruby: a.gcd(b)
来源：https://kz.zhonguo8118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://uw.zhonguo7118.cn

[N06] 判断回文字符串
来源：https://lu.zhonguo6118.cn

Py:   s == s[::-1]
来源：https://wc.zhonguo1118.cn

PHP:  $s === strrev($s);
来源：https://sm.zhonguo2118.cn

JS:   s === [...s].reverse().join("")
来源：https://sc.zhonguo8118.cn

TS:   s === [...s].reverse().join("")
来源：https://zi.zhonguo8118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://nv.zhonguo1118.cn

Go:   // 双指针从两端比较
来源：https://mq.zhonguo1118.cn

Ruby: s == s.reverse
来源：https://yq.zhonguo1118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://mf.zhonguo1118.cn

[N07] 两数之和（返回下标）
来源：https://kc.zhonguo2118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://mn.zhonguo6118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://fm.zhonguo6118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://hr.zhonguo2118.cn

TS:   // 手写 Map<string, number>
来源：https://bk.zhonguo1118.cn

Java: // 手写 HashMap
来源：https://zo.zhonguo8118.cn

Go:   // 手写 map[int]int
来源：https://wi.zhonguo4118.cn

Ruby: // 手写 Hash
来源：https://cr.zhonguo3118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://ib.zhonguo7118.cn

[N08] 生成全排列
来源：https://jw.zhonguo7118.cn

Py:   itertools.permutations(arr)
来源：https://fb.zhonguo6118.cn

PHP:  // 手写递归交换
来源：https://qk.zhonguo7118.cn

JS:   // 手写回溯递归
来源：https://yi.zhonguo3118.cn

TS:   // 手写回溯递归
来源：https://mv.zhonguo8118.cn

Java: // 手写回溯递归
来源：https://xv.zhonguo4118.cn

Go:   // 手写回溯递归
来源：https://iu.zhonguo4118.cn

Ruby: arr.permutation.to_a
来源：https://kr.zhonguo4118.cn

C#:   // 手写回溯递归
来源：https://il.zhonguo1118.cn

[N09] 栈与队列
来源：https://kj.zhonguo7118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://yl.zhonguo2118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://dt.zhonguo7118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://bd.zhonguo5118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://tu.zhonguo5118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://cj.zhonguo5118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://sy.zhonguo6118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://vf.zhonguo6118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://su.zhonguo3118.cn

[N10] 链表节点定义
来源：https://qw.zhonguo4118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://uw.zhonguo6118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://fh.zhonguo4118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://fh.zhonguo1118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://tm.zhonguo3118.cn

Java: class Node { int v; Node next; }
来源：https://es.zhonguo6118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://mk.zhonguo5118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://cg.zhonguo1118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://xi.zhonguo8118.cn

[N11] 二叉树中序遍历
来源：https://gn.zhonguo7118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://hc.zhonguo6118.cn


<!-- 参考信息 -->