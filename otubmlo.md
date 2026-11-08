代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://sm.zhonguo5118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://tu.zhonguo2118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ot.zhonguo5118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://eo.zhonguo3118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://wm.zhonguo5118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://tv.zhonguo1118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://sv.zhonguo7118.cn

[K05] 深拷贝对象
来源：https://fg.zhonguo5118.cn

Py:   copy.deepcopy(obj)
来源：https://dl.zhonguo5118.cn

PHP:  unserialize(serialize($obj));
来源：https://cw.zhonguo3118.cn

JS:   structuredClone(obj)
来源：https://vc.zhonguo4118.cn

TS:   structuredClone(obj)
来源：https://xj.zhonguo4118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://xq.zhonguo4118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ji.zhonguo2118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://kl.zhonguo3118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://jk.zhonguo6118.cn

[K06] 解析 URL 查询串
来源：https://yg.zhonguo8118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://lj.zhonguo3118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://di.zhonguo1118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://tl.zhonguo7118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://gv.zhonguo4118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://nx.zhonguo2118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://hj.zhonguo8118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://cz.zhonguo7118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://ur.zhonguo5118.cn

[K07] 进制转换
来源：https://tc.zhonguo2118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://ig.zhonguo8118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://da.zhonguo2118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://xm.zhonguo4118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://on.zhonguo5118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://vz.zhonguo5118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ra.zhonguo1118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://rc.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://pm.zhonguo3118.cn

[K08] 二进制序列化（非 JSON）
来源：https://zw.zhonguo2118.cn

Py:   pickle.dumps(obj)
来源：https://hq.zhonguo3118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://il.zhonguo2118.cn

JS:   v8.serialize(obj)        // Node
来源：https://jv.zhonguo2118.cn

TS:   v8.serialize(obj)        // Node
来源：https://re.zhonguo5118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://ox.zhonguo2118.cn

Go:   encoding/gob
来源：https://qk.zhonguo3118.cn

Ruby: Marshal.dump(obj)
来源：https://du.zhonguo3118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://yr.zhonguo2118.cn

================================================================================
来源：https://wd.zhonguo8118.cn

L. 网络请求
来源：https://fi.zhonguo4118.cn

================================================================================
来源：https://ox.zhonguo6118.cn

[L01] 发送 GET 请求
来源：https://tp.zhonguo5118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://jw.zhonguo5118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://gs.zhonguo5118.cn

JS:   await fetch(url)
来源：https://zy.zhonguo2118.cn

TS:   await fetch(url)
来源：https://de.zhonguo3118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://ix.zhonguo1118.cn

Go:   resp, err := http.Get(url)
来源：https://bk.zhonguo6118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://ip.zhonguo1118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://jv.zhonguo7118.cn

[L02] 发送 POST JSON
来源：https://na.zhonguo6118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://ql.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://zd.zhonguo2118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://ks.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://pe.zhonguo6118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://ku.zhonguo8118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://lw.zhonguo5118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://qm.zhonguo3118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://ew.zhonguo8118.cn

[L03] 设置自定义请求头
来源：https://tg.zhonguo1118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://xx.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://tx.zhonguo1118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://tl.zhonguo5118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ku.zhonguo6118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://km.zhonguo2118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://av.zhonguo5118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://vs.zhonguo1118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://iz.zhonguo6118.cn

[L04] 设置超时
来源：https://hz.zhonguo5118.cn

Py:   requests.get(url, timeout=5)
来源：https://dh.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://sx.zhonguo5118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://jt.zhonguo5118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://zx.zhonguo5118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://ip.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://ta.zhonguo1118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://af.zhonguo2118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://wj.zhonguo4118.cn

[L05] 上传文件（multipart）
来源：https://yk.zhonguo1118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://eb.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://wt.zhonguo3118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://pi.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://au.zhonguo8118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://qg.zhonguo5118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://fp.zhonguo3118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://uw.zhonguo7118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://en.zhonguo6118.cn

[L06] 解析响应为 JSON
来源：https://de.zhonguo3118.cn

Py:   resp.json()
来源：https://gh.zhonguo4118.cn

PHP:  json_decode($body, true);
来源：https://on.zhonguo1118.cn

JS:   await resp.json()
来源：https://ya.zhonguo5118.cn

TS:   await resp.json()
来源：https://do.zhonguo5118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://ke.zhonguo2118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://cb.zhonguo6118.cn

Ruby: JSON.parse(resp.body)
来源：https://yx.zhonguo5118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://wl.zhonguo5118.cn

[L07] 处理 HTTP 状态码
来源：https://ue.zhonguo4118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://uo.zhonguo5118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://ao.zhonguo7118.cn

JS:   resp.ok;  resp.status
来源：https://ya.zhonguo7118.cn

TS:   resp.ok;  resp.status
来源：https://rb.zhonguo4118.cn

Java: resp.statusCode()
来源：https://yn.zhonguo6118.cn

Go:   resp.StatusCode
来源：https://sp.zhonguo6118.cn

Ruby: resp.code.to_i
来源：https://on.zhonguo3118.cn

C#:   (int)resp.StatusCode
来源：https://gr.zhonguo5118.cn

[L08] 并发请求多个地址
来源：https://av.zhonguo4118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://xu.zhonguo5118.cn

PHP:  curl_multi_init() 系列
来源：https://ab.zhonguo7118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://lc.zhonguo8118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://mt.zhonguo5118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://so.zhonguo2118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://oi.zhonguo5118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://of.zhonguo4118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://fx.zhonguo1118.cn

================================================================================
来源：https://xn.zhonguo5118.cn

M. 命令行 / 进程 / 环境
来源：https://yl.zhonguo8118.cn

================================================================================
来源：https://nt.zhonguo8118.cn

[M01] 读取命令行参数
来源：https://hj.zhonguo5118.cn

Py:   sys.argv[1:]
来源：https://wf.zhonguo8118.cn

PHP:  $argv;  $argc;
来源：https://dz.zhonguo8118.cn

JS:   process.argv.slice(2)
来源：https://ax.zhonguo2118.cn

TS:   process.argv.slice(2)
来源：https://lz.zhonguo4118.cn

Java: args 数组（main 方法参数）
来源：https://ce.zhonguo2118.cn

Go:   os.Args[1:]
来源：https://bj.zhonguo2118.cn

Ruby: ARGV
来源：https://ke.zhonguo6118.cn

C#:   args 数组（Main 方法参数）
来源：https://mi.zhonguo7118.cn

[M02] 读取环境变量
来源：https://zn.zhonguo5118.cn

Py:   os.environ.get("HOME")
来源：https://kv.zhonguo3118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://vy.zhonguo2118.cn

JS:   process.env.HOME
来源：https://lw.zhonguo1118.cn

TS:   process.env.HOME
来源：https://jx.zhonguo5118.cn

Java: System.getenv("HOME")
来源：https://jv.zhonguo8118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://ie.zhonguo2118.cn

Ruby: ENV["HOME"]
来源：https://lb.zhonguo4118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://cn.zhonguo2118.cn

[M03] 执行外部命令
来源：https://ca.zhonguo7118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://ra.zhonguo6118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://nz.zhonguo4118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://iy.zhonguo3118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://fd.zhonguo2118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://jl.zhonguo5118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://an.zhonguo6118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://yz.zhonguo7118.cn

C#:   Process.Start("ls", "-l");
来源：https://fw.zhonguo6118.cn

[M04] 获取当前工作目录
来源：https://ah.zhonguo2118.cn

Py:   os.getcwd()
来源：https://ys.zhonguo8118.cn

PHP:  getcwd();
来源：https://tw.zhonguo8118.cn

JS:   process.cwd()
来源：https://xh.zhonguo7118.cn

TS:   process.cwd()
来源：https://av.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://ap.zhonguo5118.cn

Go:   os.Getwd()
来源：https://tg.zhonguo4118.cn

Ruby: Dir.pwd
来源：https://al.zhonguo5118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ol.zhonguo7118.cn

[M05] 设置退出码
来源：https://ml.zhonguo3118.cn

Py:   sys.exit(1)
来源：https://kj.zhonguo3118.cn

PHP:  exit(1);
来源：https://ac.zhonguo1118.cn

JS:   process.exit(1)
来源：https://wj.zhonguo4118.cn

TS:   process.exit(1)
来源：https://sm.zhonguo6118.cn

Java: System.exit(1)
来源：https://pn.zhonguo1118.cn

Go:   os.Exit(1)
来源：https://ds.zhonguo2118.cn

Ruby: exit 1
来源：https://pz.zhonguo8118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://qs.zhonguo7118.cn

[M06] 向标准错误输出
来源：https://yd.zhonguo3118.cn

Py:   print("err", file=sys.stderr)
来源：https://cw.zhonguo1118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://vw.zhonguo4118.cn

JS:   console.error("err")
来源：https://yc.zhonguo2118.cn

TS:   console.error("err")
来源：https://ob.zhonguo1118.cn

Java: System.err.println("err")
来源：https://ly.zhonguo3118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://os.zhonguo8118.cn

Ruby: warn "err"
来源：https://kj.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://jo.zhonguo6118.cn

[M07] 判断是否为主入口
来源：https://op.zhonguo8118.cn

Py:   if __name__ == "__main__":
来源：https://pd.zhonguo8118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://pg.zhonguo7118.cn

JS:   require.main === module
来源：https://pi.zhonguo2118.cn

TS:   require.main === module
来源：https://yv.zhonguo8118.cn

Java: public static void main(String[] args)
来源：https://bo.zhonguo3118.cn

Go:   func main()
来源：https://xw.zhonguo8118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://bg.zhonguo6118.cn

C#:   static void Main(string[] args)
来源：https://ll.zhonguo5118.cn

[M08] 获取系统与运行时信息
来源：https://kg.zhonguo7118.cn

Py:   platform.system();  platform.python_version()
来源：https://ws.zhonguo4118.cn

PHP:  PHP_OS;  phpversion();
来源：https://xa.zhonguo3118.cn

JS:   process.platform;  process.version
来源：https://nf.zhonguo7118.cn

TS:   process.platform;  process.version
来源：https://xm.zhonguo6118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://ks.zhonguo8118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://pg.zhonguo3118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://mj.zhonguo4118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://iz.zhonguo6118.cn

================================================================================
来源：https://by.zhonguo4118.cn

N. 数据结构与算法
来源：https://cj.zhonguo4118.cn

================================================================================
来源：https://zr.zhonguo3118.cn

[N01] 二分查找（有序数组）
来源：https://ny.zhonguo2118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://zs.zhonguo8118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://yn.zhonguo3118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://co.zhonguo8118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://nf.zhonguo3118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://bd.zhonguo6118.cn

Go:   sort.SearchInts(arr, x)
来源：https://go.zhonguo1118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://ji.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://dd.zhonguo7118.cn

[N02] 排序（工程实践用内置实现）
来源：https://no.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://hc.zhonguo5118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://yl.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://uz.zhonguo5118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://df.zhonguo1118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://zr.zhonguo7118.cn

Go:   slices.Sort(arr)
来源：https://ha.zhonguo7118.cn

Ruby: arr.sort
来源：https://fn.zhonguo5118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://lt.zhonguo3118.cn

[N03] 快速排序（分治示例）
来源：https://kt.zhonguo2118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://vf.zhonguo4118.cn

PHP:  // 递归实现，或用 usort
来源：https://se.zhonguo7118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://qb.zhonguo7118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://yh.zhonguo1118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://jw.zhonguo1118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://zn.zhonguo3118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://gg.zhonguo8118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://na.zhonguo7118.cn

[N04] 斐波那契数列
来源：https://sl.zhonguo3118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://df.zhonguo6118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://ll.zhonguo1118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://no.zhonguo8118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://hd.zhonguo7118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://hz.zhonguo6118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://vw.zhonguo6118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://ip.zhonguo1118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://xx.zhonguo1118.cn

[N05] 最大公约数
来源：https://gq.zhonguo4118.cn

Py:   math.gcd(a, b)
来源：https://iw.zhonguo4118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://oe.zhonguo8118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://zj.zhonguo6118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://gg.zhonguo5118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://kn.zhonguo7118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://al.zhonguo2118.cn

Ruby: a.gcd(b)
来源：https://hg.zhonguo6118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://qj.zhonguo4118.cn

[N06] 判断回文字符串
来源：https://zl.zhonguo2118.cn

Py:   s == s[::-1]
来源：https://rh.zhonguo6118.cn

PHP:  $s === strrev($s);
来源：https://xz.zhonguo1118.cn

JS:   s === [...s].reverse().join("")
来源：https://vp.zhonguo3118.cn

TS:   s === [...s].reverse().join("")
来源：https://pv.zhonguo2118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://ru.zhonguo3118.cn

Go:   // 双指针从两端比较
来源：https://yz.zhonguo4118.cn

Ruby: s == s.reverse
来源：https://tp.zhonguo2118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://ne.zhonguo3118.cn

[N07] 两数之和（返回下标）
来源：https://ut.zhonguo2118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://rq.zhonguo5118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://si.zhonguo3118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://lb.zhonguo6118.cn

TS:   // 手写 Map<string, number>
来源：https://ay.zhonguo6118.cn

Java: // 手写 HashMap
来源：https://tt.zhonguo3118.cn

Go:   // 手写 map[int]int
来源：https://ft.zhonguo3118.cn

Ruby: // 手写 Hash
来源：https://ch.zhonguo3118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://qu.zhonguo6118.cn

[N08] 生成全排列
来源：https://hp.zhonguo7118.cn

Py:   itertools.permutations(arr)
来源：https://pf.zhonguo5118.cn

PHP:  // 手写递归交换
来源：https://az.zhonguo8118.cn

JS:   // 手写回溯递归
来源：https://le.zhonguo1118.cn

TS:   // 手写回溯递归
来源：https://oy.zhonguo8118.cn

Java: // 手写回溯递归
来源：https://iu.zhonguo3118.cn

Go:   // 手写回溯递归
来源：https://fv.zhonguo1118.cn

Ruby: arr.permutation.to_a
来源：https://oj.zhonguo6118.cn

C#:   // 手写回溯递归
来源：https://qj.zhonguo4118.cn

[N09] 栈与队列
来源：https://nd.zhonguo5118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://ev.zhonguo7118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://no.zhonguo4118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://ur.zhonguo4118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://vy.zhonguo4118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://vz.zhonguo6118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://kx.zhonguo4118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://ld.zhonguo1118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://te.zhonguo1118.cn

[N10] 链表节点定义
来源：https://gc.zhonguo8118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://ej.zhonguo5118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://gn.zhonguo1118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://rb.zhonguo4118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://hh.zhonguo2118.cn

Java: class Node { int v; Node next; }
来源：https://yu.zhonguo4118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://ra.zhonguo8118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://xb.zhonguo2118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://tp.zhonguo3118.cn

[N11] 二叉树中序遍历
来源：https://us.zhonguo3118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://ce.zhonguo8118.cn

PHP:  // 手写递归函数
来源：https://is.zhonguo6118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://sj.zhonguo6118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://yk.zhonguo5118.cn

Java: // 手写递归
来源：https://xz.zhonguo6118.cn

Go:   // 手写递归
来源：https://vp.zhonguo7118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://ae.zhonguo8118.cn

C#:   // 手写递归
来源：https://zn.zhonguo4118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://vo.zhonguo1118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://nf.zhonguo7118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://pi.zhonguo6118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://kn.zhonguo4118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://rf.zhonguo1118.cn


<!-- 参考信息 -->