代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://ck.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://hg.zhonguo6118.cn

[K08] 二进制序列化（非 JSON）
来源：https://dv.zhonguo1118.cn

Py:   pickle.dumps(obj)
来源：https://as.zhonguo3118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://us.zhonguo6118.cn

JS:   v8.serialize(obj)        // Node
来源：https://lm.zhonguo2118.cn

TS:   v8.serialize(obj)        // Node
来源：https://px.zhonguo6118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://yy.zhonguo5118.cn

Go:   encoding/gob
来源：https://an.zhonguo3118.cn

Ruby: Marshal.dump(obj)
来源：https://am.zhonguo5118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://im.zhonguo7118.cn

================================================================================
来源：https://ph.zhonguo6118.cn

L. 网络请求
来源：https://jl.zhonguo6118.cn

================================================================================
来源：https://kb.zhonguo2118.cn

[L01] 发送 GET 请求
来源：https://dz.zhonguo5118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://xt.zhonguo2118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://kf.zhonguo7118.cn

JS:   await fetch(url)
来源：https://jv.zhonguo4118.cn

TS:   await fetch(url)
来源：https://xn.zhonguo8118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://et.zhonguo2118.cn

Go:   resp, err := http.Get(url)
来源：https://ud.zhonguo5118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://sx.zhonguo8118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://md.zhonguo3118.cn

[L02] 发送 POST JSON
来源：https://pt.zhonguo8118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://bb.zhonguo8118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://ux.zhonguo7118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://qv.zhonguo4118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://jk.zhonguo4118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://ox.zhonguo3118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://dw.zhonguo6118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://id.zhonguo8118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://wa.zhonguo6118.cn

[L03] 设置自定义请求头
来源：https://cv.zhonguo8118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://vg.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://sw.zhonguo7118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://qk.zhonguo8118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://id.zhonguo8118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://cl.zhonguo4118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://gh.zhonguo5118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://kq.zhonguo4118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://fa.zhonguo1118.cn

[L04] 设置超时
来源：https://wl.zhonguo4118.cn

Py:   requests.get(url, timeout=5)
来源：https://ls.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://gu.zhonguo2118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://sn.zhonguo2118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://eg.zhonguo7118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://vo.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://pt.zhonguo8118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://ep.zhonguo1118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://nu.zhonguo1118.cn

[L05] 上传文件（multipart）
来源：https://ws.zhonguo3118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://fj.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://sa.zhonguo7118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://ai.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://qd.zhonguo5118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://sh.zhonguo6118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://lq.zhonguo6118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://go.zhonguo6118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://rd.zhonguo7118.cn

[L06] 解析响应为 JSON
来源：https://zh.zhonguo7118.cn

Py:   resp.json()
来源：https://qm.zhonguo6118.cn

PHP:  json_decode($body, true);
来源：https://st.zhonguo6118.cn

JS:   await resp.json()
来源：https://oj.zhonguo2118.cn

TS:   await resp.json()
来源：https://ec.zhonguo5118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://iz.zhonguo4118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://xa.zhonguo4118.cn

Ruby: JSON.parse(resp.body)
来源：https://vl.zhonguo2118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://gi.zhonguo8118.cn

[L07] 处理 HTTP 状态码
来源：https://dh.zhonguo8118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://lj.zhonguo2118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://wj.zhonguo7118.cn

JS:   resp.ok;  resp.status
来源：https://uv.zhonguo4118.cn

TS:   resp.ok;  resp.status
来源：https://ye.zhonguo3118.cn

Java: resp.statusCode()
来源：https://in.zhonguo1118.cn

Go:   resp.StatusCode
来源：https://wq.zhonguo1118.cn

Ruby: resp.code.to_i
来源：https://ed.zhonguo1118.cn

C#:   (int)resp.StatusCode
来源：https://hk.zhonguo6118.cn

[L08] 并发请求多个地址
来源：https://wl.zhonguo6118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://qa.zhonguo1118.cn

PHP:  curl_multi_init() 系列
来源：https://pm.zhonguo7118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://pa.zhonguo7118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://xq.zhonguo8118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://pn.zhonguo6118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://st.zhonguo7118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://xs.zhonguo2118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://xi.zhonguo1118.cn

================================================================================
来源：https://ov.zhonguo1118.cn

M. 命令行 / 进程 / 环境
来源：https://bo.zhonguo8118.cn

================================================================================
来源：https://zi.zhonguo8118.cn

[M01] 读取命令行参数
来源：https://xk.zhonguo6118.cn

Py:   sys.argv[1:]
来源：https://mj.zhonguo1118.cn

PHP:  $argv;  $argc;
来源：https://qn.zhonguo6118.cn

JS:   process.argv.slice(2)
来源：https://cl.zhonguo6118.cn

TS:   process.argv.slice(2)
来源：https://jq.zhonguo5118.cn

Java: args 数组（main 方法参数）
来源：https://vm.zhonguo4118.cn

Go:   os.Args[1:]
来源：https://dh.zhonguo7118.cn

Ruby: ARGV
来源：https://vn.zhonguo8118.cn

C#:   args 数组（Main 方法参数）
来源：https://nx.zhonguo7118.cn

[M02] 读取环境变量
来源：https://kc.zhonguo2118.cn

Py:   os.environ.get("HOME")
来源：https://ff.zhonguo3118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://ra.zhonguo8118.cn

JS:   process.env.HOME
来源：https://ig.zhonguo6118.cn

TS:   process.env.HOME
来源：https://bw.zhonguo4118.cn

Java: System.getenv("HOME")
来源：https://ka.zhonguo2118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://ga.zhonguo1118.cn

Ruby: ENV["HOME"]
来源：https://te.zhonguo8118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://vb.zhonguo1118.cn

[M03] 执行外部命令
来源：https://yk.zhonguo2118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://sh.zhonguo2118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://tk.zhonguo1118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://bi.zhonguo8118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://px.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://yz.zhonguo2118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://aj.zhonguo1118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://dg.zhonguo8118.cn

C#:   Process.Start("ls", "-l");
来源：https://cn.zhonguo2118.cn

[M04] 获取当前工作目录
来源：https://aw.zhonguo8118.cn

Py:   os.getcwd()
来源：https://rc.zhonguo1118.cn

PHP:  getcwd();
来源：https://vo.zhonguo5118.cn

JS:   process.cwd()
来源：https://oo.zhonguo5118.cn

TS:   process.cwd()
来源：https://an.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://iq.zhonguo7118.cn

Go:   os.Getwd()
来源：https://ys.zhonguo6118.cn

Ruby: Dir.pwd
来源：https://fc.zhonguo4118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ah.zhonguo2118.cn

[M05] 设置退出码
来源：https://mu.zhonguo2118.cn

Py:   sys.exit(1)
来源：https://sq.zhonguo4118.cn

PHP:  exit(1);
来源：https://sm.zhonguo8118.cn

JS:   process.exit(1)
来源：https://lj.zhonguo8118.cn

TS:   process.exit(1)
来源：https://by.zhonguo8118.cn

Java: System.exit(1)
来源：https://db.zhonguo4118.cn

Go:   os.Exit(1)
来源：https://dq.zhonguo1118.cn

Ruby: exit 1
来源：https://zr.zhonguo3118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://qw.zhonguo7118.cn

[M06] 向标准错误输出
来源：https://eg.zhonguo8118.cn

Py:   print("err", file=sys.stderr)
来源：https://jh.zhonguo4118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://xo.zhonguo3118.cn

JS:   console.error("err")
来源：https://zf.zhonguo8118.cn

TS:   console.error("err")
来源：https://fu.zhonguo8118.cn

Java: System.err.println("err")
来源：https://lr.zhonguo1118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://dg.zhonguo2118.cn

Ruby: warn "err"
来源：https://up.zhonguo3118.cn

C#:   Console.Error.WriteLine("err")
来源：https://ok.zhonguo4118.cn

[M07] 判断是否为主入口
来源：https://sl.zhonguo6118.cn

Py:   if __name__ == "__main__":
来源：https://vu.zhonguo3118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://kb.zhonguo1118.cn

JS:   require.main === module
来源：https://dy.zhonguo8118.cn

TS:   require.main === module
来源：https://xv.zhonguo6118.cn

Java: public static void main(String[] args)
来源：https://lr.zhonguo7118.cn

Go:   func main()
来源：https://tt.zhonguo2118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://vz.zhonguo5118.cn

C#:   static void Main(string[] args)
来源：https://hi.zhonguo7118.cn

[M08] 获取系统与运行时信息
来源：https://zr.zhonguo4118.cn

Py:   platform.system();  platform.python_version()
来源：https://bq.zhonguo1118.cn

PHP:  PHP_OS;  phpversion();
来源：https://dm.zhonguo2118.cn

JS:   process.platform;  process.version
来源：https://cg.zhonguo6118.cn

TS:   process.platform;  process.version
来源：https://qp.zhonguo6118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://rh.zhonguo7118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://ch.zhonguo1118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://js.zhonguo3118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://tg.zhonguo7118.cn

================================================================================
来源：https://fr.zhonguo3118.cn

N. 数据结构与算法
来源：https://qk.zhonguo6118.cn

================================================================================
来源：https://ja.zhonguo2118.cn

[N01] 二分查找（有序数组）
来源：https://mv.zhonguo5118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://bh.zhonguo7118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://xh.zhonguo2118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://rd.zhonguo8118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://ma.zhonguo4118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://cs.zhonguo4118.cn

Go:   sort.SearchInts(arr, x)
来源：https://hf.zhonguo5118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://yd.zhonguo6118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://vs.zhonguo7118.cn

[N02] 排序（工程实践用内置实现）
来源：https://wr.zhonguo2118.cn

Py:   sorted(arr);  arr.sort()
来源：https://mv.zhonguo4118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://zo.zhonguo1118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://rm.zhonguo5118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://wy.zhonguo6118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://ty.zhonguo7118.cn

Go:   slices.Sort(arr)
来源：https://bv.zhonguo6118.cn

Ruby: arr.sort
来源：https://sk.zhonguo1118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://wg.zhonguo6118.cn

[N03] 快速排序（分治示例）
来源：https://yj.zhonguo8118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://tz.zhonguo6118.cn

PHP:  // 递归实现，或用 usort
来源：https://yi.zhonguo8118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://ig.zhonguo3118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://wj.zhonguo1118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://lz.zhonguo8118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://ji.zhonguo4118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://ih.zhonguo7118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://ha.zhonguo3118.cn

[N04] 斐波那契数列
来源：https://tx.zhonguo4118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://vj.zhonguo5118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://zm.zhonguo1118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://ga.zhonguo5118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://qm.zhonguo2118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://ck.zhonguo5118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://gp.zhonguo8118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://nw.zhonguo1118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://wk.zhonguo1118.cn

[N05] 最大公约数
来源：https://im.zhonguo4118.cn

Py:   math.gcd(a, b)
来源：https://ap.zhonguo4118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://zf.zhonguo1118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://by.zhonguo5118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://nb.zhonguo8118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://zo.zhonguo1118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://pt.zhonguo6118.cn

Ruby: a.gcd(b)
来源：https://zk.zhonguo2118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://yv.zhonguo3118.cn

[N06] 判断回文字符串
来源：https://bg.zhonguo6118.cn

Py:   s == s[::-1]
来源：https://zc.zhonguo7118.cn

PHP:  $s === strrev($s);
来源：https://od.zhonguo1118.cn

JS:   s === [...s].reverse().join("")
来源：https://ja.zhonguo4118.cn

TS:   s === [...s].reverse().join("")
来源：https://tg.zhonguo7118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://ad.zhonguo4118.cn

Go:   // 双指针从两端比较
来源：https://mg.zhonguo3118.cn

Ruby: s == s.reverse
来源：https://oc.zhonguo5118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://ay.zhonguo7118.cn

[N07] 两数之和（返回下标）
来源：https://mv.zhonguo2118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://pj.zhonguo2118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://qw.zhonguo2118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://be.zhonguo1118.cn

TS:   // 手写 Map<string, number>
来源：https://yq.zhonguo7118.cn

Java: // 手写 HashMap
来源：https://ba.zhonguo7118.cn

Go:   // 手写 map[int]int
来源：https://fl.zhonguo5118.cn

Ruby: // 手写 Hash
来源：https://kn.zhonguo8118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://iz.zhonguo7118.cn

[N08] 生成全排列
来源：https://yx.zhonguo4118.cn

Py:   itertools.permutations(arr)
来源：https://qd.zhonguo4118.cn

PHP:  // 手写递归交换
来源：https://ip.zhonguo4118.cn

JS:   // 手写回溯递归
来源：https://za.zhonguo3118.cn

TS:   // 手写回溯递归
来源：https://cm.zhonguo2118.cn

Java: // 手写回溯递归
来源：https://qm.zhonguo8118.cn

Go:   // 手写回溯递归
来源：https://gu.zhonguo3118.cn

Ruby: arr.permutation.to_a
来源：https://bz.zhonguo6118.cn

C#:   // 手写回溯递归
来源：https://re.zhonguo4118.cn

[N09] 栈与队列
来源：https://sd.zhonguo1118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://nq.zhonguo7118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://qe.zhonguo4118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://su.zhonguo4118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://pk.zhonguo4118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://dh.zhonguo6118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://wl.zhonguo8118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://mv.zhonguo6118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://sp.zhonguo1118.cn

[N10] 链表节点定义
来源：https://yu.zhonguo5118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://og.zhonguo3118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://du.zhonguo4118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://vu.zhonguo3118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://fo.zhonguo7118.cn

Java: class Node { int v; Node next; }
来源：https://za.zhonguo1118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://wo.zhonguo6118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://fy.zhonguo7118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://fl.zhonguo2118.cn

[N11] 二叉树中序遍历
来源：https://pm.zhonguo2118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://zv.zhonguo4118.cn

PHP:  // 手写递归函数
来源：https://qm.zhonguo7118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://cl.zhonguo2118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://cm.zhonguo1118.cn

Java: // 手写递归
来源：https://uw.zhonguo6118.cn

Go:   // 手写递归
来源：https://pa.zhonguo8118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://lu.zhonguo2118.cn

C#:   // 手写递归
来源：https://dj.zhonguo6118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://iw.zhonguo1118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://qw.zhonguo5118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://kl.zhonguo1118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://tk.zhonguo4118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://nj.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://bj.zhonguo2118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://ym.zhonguo5118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://uu.zhonguo8118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://qp.zhonguo2118.cn

================================================================================
来源：https://ys.zhonguo6118.cn

O. 并发与异步
来源：https://pf.zhonguo2118.cn

================================================================================
来源：https://tz.zhonguo1118.cn

[O01] 启动一个线程
来源：https://zc.zhonguo7118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://oc.zhonguo4118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://bu.zhonguo5118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://qt.zhonguo1118.cn

TS:   // 同 JS
来源：https://po.zhonguo5118.cn

Java: new Thread(() -> f()).start()
来源：https://ck.zhonguo8118.cn

Go:   go f()
来源：https://lz.zhonguo7118.cn

Ruby: Thread.new { f }
来源：https://ed.zhonguo1118.cn

C#:   Task.Run(() => F());
来源：https://vs.zhonguo6118.cn

[O02] 使用线程池
来源：https://ai.zhonguo2118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://jw.zhonguo6118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://xs.zhonguo4118.cn

JS:   // worker_threads 线程池
来源：https://kx.zhonguo3118.cn

TS:   // worker_threads 线程池
来源：https://dz.zhonguo6118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://cs.zhonguo2118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://ss.zhonguo8118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://tb.zhonguo2118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://wy.zhonguo3118.cn

[O03] 加锁保护共享数据
来源：https://jc.zhonguo5118.cn

Py:   with lock: shared += 1
来源：https://nd.zhonguo2118.cn

PHP:  // 用 flock() 做文件锁
来源：https://lo.zhonguo1118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://cy.zhonguo2118.cn

TS:   // 同 JS
来源：https://nf.zhonguo7118.cn

Java: synchronized (this) { shared++; }
来源：https://ma.zhonguo1118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://ld.zhonguo2118.cn


<!-- 参考信息 -->