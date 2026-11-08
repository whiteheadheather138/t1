代发 wailian999

Go:   encoding/gob
来源：https://xv.zhonguo5118.cn

Ruby: Marshal.dump(obj)
来源：https://si.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://iy.zhonguo7118.cn

================================================================================
来源：https://jh.zhonguo6118.cn

L. 网络请求
来源：https://zw.zhonguo7118.cn

================================================================================
来源：https://es.zhonguo1118.cn

[L01] 发送 GET 请求
来源：https://wu.zhonguo4118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://vs.zhonguo4118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://vx.zhonguo2118.cn

JS:   await fetch(url)
来源：https://eg.zhonguo7118.cn

TS:   await fetch(url)
来源：https://jg.zhonguo7118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://um.zhonguo3118.cn

Go:   resp, err := http.Get(url)
来源：https://wa.zhonguo8118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://ow.zhonguo4118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://ei.zhonguo6118.cn

[L02] 发送 POST JSON
来源：https://od.zhonguo2118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://rg.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://om.zhonguo7118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://tb.zhonguo5118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://uo.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://oa.zhonguo1118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://ay.zhonguo6118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://kx.zhonguo7118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://gh.zhonguo1118.cn

[L03] 设置自定义请求头
来源：https://zs.zhonguo1118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://ok.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://kd.zhonguo6118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://po.zhonguo3118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://dg.zhonguo8118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://hd.zhonguo8118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://xx.zhonguo5118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://yc.zhonguo8118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://xf.zhonguo1118.cn

[L04] 设置超时
来源：https://wy.zhonguo2118.cn

Py:   requests.get(url, timeout=5)
来源：https://ph.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://lj.zhonguo7118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://cq.zhonguo4118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://yb.zhonguo6118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://kr.zhonguo2118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://cz.zhonguo2118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://hm.zhonguo5118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://un.zhonguo1118.cn

[L05] 上传文件（multipart）
来源：https://oc.zhonguo2118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://yz.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://df.zhonguo7118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://gl.zhonguo3118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://lq.zhonguo4118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://qj.zhonguo5118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://he.zhonguo4118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ut.zhonguo4118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://in.zhonguo5118.cn

[L06] 解析响应为 JSON
来源：https://ho.zhonguo2118.cn

Py:   resp.json()
来源：https://iy.zhonguo3118.cn

PHP:  json_decode($body, true);
来源：https://lo.zhonguo7118.cn

JS:   await resp.json()
来源：https://wv.zhonguo3118.cn

TS:   await resp.json()
来源：https://ub.zhonguo7118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://vn.zhonguo6118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://ry.zhonguo8118.cn

Ruby: JSON.parse(resp.body)
来源：https://bq.zhonguo1118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://he.zhonguo2118.cn

[L07] 处理 HTTP 状态码
来源：https://vp.zhonguo3118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://qt.zhonguo8118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://jw.zhonguo7118.cn

JS:   resp.ok;  resp.status
来源：https://zh.zhonguo1118.cn

TS:   resp.ok;  resp.status
来源：https://be.zhonguo2118.cn

Java: resp.statusCode()
来源：https://wz.zhonguo4118.cn

Go:   resp.StatusCode
来源：https://lz.zhonguo4118.cn

Ruby: resp.code.to_i
来源：https://rt.zhonguo5118.cn

C#:   (int)resp.StatusCode
来源：https://eo.zhonguo5118.cn

[L08] 并发请求多个地址
来源：https://kt.zhonguo5118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://mx.zhonguo5118.cn

PHP:  curl_multi_init() 系列
来源：https://wl.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ey.zhonguo3118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://zo.zhonguo8118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://iw.zhonguo3118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://sn.zhonguo3118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://gk.zhonguo5118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://bt.zhonguo5118.cn

================================================================================
来源：https://au.zhonguo5118.cn

M. 命令行 / 进程 / 环境
来源：https://zo.zhonguo4118.cn

================================================================================
来源：https://jy.zhonguo7118.cn

[M01] 读取命令行参数
来源：https://gj.zhonguo2118.cn

Py:   sys.argv[1:]
来源：https://lw.zhonguo3118.cn

PHP:  $argv;  $argc;
来源：https://un.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://dz.zhonguo4118.cn

TS:   process.argv.slice(2)
来源：https://mc.zhonguo7118.cn

Java: args 数组（main 方法参数）
来源：https://kc.zhonguo6118.cn

Go:   os.Args[1:]
来源：https://tq.zhonguo6118.cn

Ruby: ARGV
来源：https://pr.zhonguo4118.cn

C#:   args 数组（Main 方法参数）
来源：https://sm.zhonguo5118.cn

[M02] 读取环境变量
来源：https://sm.zhonguo6118.cn

Py:   os.environ.get("HOME")
来源：https://zk.zhonguo7118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://dw.zhonguo4118.cn

JS:   process.env.HOME
来源：https://mw.zhonguo4118.cn

TS:   process.env.HOME
来源：https://ez.zhonguo1118.cn

Java: System.getenv("HOME")
来源：https://lm.zhonguo2118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://wi.zhonguo4118.cn

Ruby: ENV["HOME"]
来源：https://jc.zhonguo8118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://oz.zhonguo2118.cn

[M03] 执行外部命令
来源：https://tj.zhonguo5118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://nt.zhonguo8118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://tf.zhonguo3118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://im.zhonguo1118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://jd.zhonguo4118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://aa.zhonguo2118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://nc.zhonguo6118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://iq.zhonguo1118.cn

C#:   Process.Start("ls", "-l");
来源：https://sn.zhonguo5118.cn

[M04] 获取当前工作目录
来源：https://my.zhonguo2118.cn

Py:   os.getcwd()
来源：https://fe.zhonguo2118.cn

PHP:  getcwd();
来源：https://fa.zhonguo4118.cn

JS:   process.cwd()
来源：https://lr.zhonguo2118.cn

TS:   process.cwd()
来源：https://ke.zhonguo6118.cn

Java: Path.of("").toAbsolutePath()
来源：https://kh.zhonguo8118.cn

Go:   os.Getwd()
来源：https://xh.zhonguo5118.cn

Ruby: Dir.pwd
来源：https://cu.zhonguo4118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://yj.zhonguo7118.cn

[M05] 设置退出码
来源：https://fo.zhonguo2118.cn

Py:   sys.exit(1)
来源：https://cj.zhonguo2118.cn

PHP:  exit(1);
来源：https://dh.zhonguo7118.cn

JS:   process.exit(1)
来源：https://vx.zhonguo7118.cn

TS:   process.exit(1)
来源：https://jb.zhonguo5118.cn

Java: System.exit(1)
来源：https://bk.zhonguo5118.cn

Go:   os.Exit(1)
来源：https://pt.zhonguo2118.cn

Ruby: exit 1
来源：https://dj.zhonguo5118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://kf.zhonguo7118.cn

[M06] 向标准错误输出
来源：https://yh.zhonguo5118.cn

Py:   print("err", file=sys.stderr)
来源：https://nf.zhonguo8118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://wa.zhonguo7118.cn

JS:   console.error("err")
来源：https://wa.zhonguo2118.cn

TS:   console.error("err")
来源：https://fc.zhonguo1118.cn

Java: System.err.println("err")
来源：https://zn.zhonguo3118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://wf.zhonguo3118.cn

Ruby: warn "err"
来源：https://mf.zhonguo5118.cn

C#:   Console.Error.WriteLine("err")
来源：https://xl.zhonguo2118.cn

[M07] 判断是否为主入口
来源：https://vu.zhonguo8118.cn

Py:   if __name__ == "__main__":
来源：https://ob.zhonguo7118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://in.zhonguo1118.cn

JS:   require.main === module
来源：https://zz.zhonguo8118.cn

TS:   require.main === module
来源：https://ms.zhonguo5118.cn

Java: public static void main(String[] args)
来源：https://ih.zhonguo6118.cn

Go:   func main()
来源：https://nd.zhonguo6118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://nc.zhonguo5118.cn

C#:   static void Main(string[] args)
来源：https://wf.zhonguo6118.cn

[M08] 获取系统与运行时信息
来源：https://ws.zhonguo5118.cn

Py:   platform.system();  platform.python_version()
来源：https://mj.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://ce.zhonguo6118.cn

JS:   process.platform;  process.version
来源：https://ql.zhonguo4118.cn

TS:   process.platform;  process.version
来源：https://ed.zhonguo4118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://mj.zhonguo3118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://qd.zhonguo6118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://hj.zhonguo4118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://oy.zhonguo4118.cn

================================================================================
来源：https://ch.zhonguo2118.cn

N. 数据结构与算法
来源：https://gy.zhonguo2118.cn

================================================================================
来源：https://qt.zhonguo3118.cn

[N01] 二分查找（有序数组）
来源：https://qt.zhonguo8118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://mf.zhonguo7118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://eo.zhonguo1118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://jp.zhonguo8118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://yn.zhonguo1118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://br.zhonguo6118.cn

Go:   sort.SearchInts(arr, x)
来源：https://gu.zhonguo6118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://iw.zhonguo2118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://uc.zhonguo8118.cn

[N02] 排序（工程实践用内置实现）
来源：https://xj.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://sr.zhonguo3118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://zj.zhonguo3118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://ue.zhonguo5118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://fr.zhonguo3118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://ir.zhonguo7118.cn

Go:   slices.Sort(arr)
来源：https://yy.zhonguo5118.cn

Ruby: arr.sort
来源：https://bs.zhonguo5118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://uy.zhonguo5118.cn

[N03] 快速排序（分治示例）
来源：https://jg.zhonguo5118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://ih.zhonguo5118.cn

PHP:  // 递归实现，或用 usort
来源：https://gq.zhonguo8118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://hr.zhonguo2118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://rq.zhonguo7118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://ds.zhonguo2118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://pd.zhonguo5118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://hy.zhonguo7118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://tc.zhonguo6118.cn

[N04] 斐波那契数列
来源：https://do.zhonguo4118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://fk.zhonguo5118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://dz.zhonguo2118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://bk.zhonguo3118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://wp.zhonguo4118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://ah.zhonguo2118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://bl.zhonguo8118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://ba.zhonguo5118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://fq.zhonguo7118.cn

[N05] 最大公约数
来源：https://mx.zhonguo2118.cn

Py:   math.gcd(a, b)
来源：https://yd.zhonguo2118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://ei.zhonguo7118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://tq.zhonguo3118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://fx.zhonguo7118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://yp.zhonguo4118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://um.zhonguo4118.cn

Ruby: a.gcd(b)
来源：https://fx.zhonguo7118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://co.zhonguo1118.cn

[N06] 判断回文字符串
来源：https://mf.zhonguo8118.cn

Py:   s == s[::-1]
来源：https://uk.zhonguo4118.cn

PHP:  $s === strrev($s);
来源：https://lr.zhonguo3118.cn

JS:   s === [...s].reverse().join("")
来源：https://gq.zhonguo3118.cn

TS:   s === [...s].reverse().join("")
来源：https://ro.zhonguo5118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://fo.zhonguo3118.cn

Go:   // 双指针从两端比较
来源：https://zd.zhonguo8118.cn

Ruby: s == s.reverse
来源：https://hg.zhonguo5118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://ot.zhonguo4118.cn

[N07] 两数之和（返回下标）
来源：https://ml.zhonguo4118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://hs.zhonguo4118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://gc.zhonguo3118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://bx.zhonguo8118.cn

TS:   // 手写 Map<string, number>
来源：https://wj.zhonguo7118.cn

Java: // 手写 HashMap
来源：https://aa.zhonguo5118.cn

Go:   // 手写 map[int]int
来源：https://re.zhonguo5118.cn

Ruby: // 手写 Hash
来源：https://nj.zhonguo4118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://iw.zhonguo7118.cn

[N08] 生成全排列
来源：https://ax.zhonguo1118.cn

Py:   itertools.permutations(arr)
来源：https://pk.zhonguo6118.cn

PHP:  // 手写递归交换
来源：https://fp.zhonguo4118.cn

JS:   // 手写回溯递归
来源：https://ix.zhonguo1118.cn

TS:   // 手写回溯递归
来源：https://xp.zhonguo1118.cn

Java: // 手写回溯递归
来源：https://qt.zhonguo1118.cn

Go:   // 手写回溯递归
来源：https://fw.zhonguo5118.cn

Ruby: arr.permutation.to_a
来源：https://ad.zhonguo4118.cn

C#:   // 手写回溯递归
来源：https://kd.zhonguo6118.cn

[N09] 栈与队列
来源：https://zc.zhonguo4118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://ct.zhonguo6118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://cd.zhonguo3118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://mo.zhonguo5118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://rt.zhonguo2118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://ui.zhonguo2118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://tn.zhonguo2118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://mb.zhonguo5118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://xz.zhonguo5118.cn

[N10] 链表节点定义
来源：https://lr.zhonguo5118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://bx.zhonguo7118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://rl.zhonguo6118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://uc.zhonguo2118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://rp.zhonguo2118.cn

Java: class Node { int v; Node next; }
来源：https://sc.zhonguo5118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://vo.zhonguo3118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://wt.zhonguo8118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://fn.zhonguo8118.cn

[N11] 二叉树中序遍历
来源：https://lq.zhonguo2118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://hz.zhonguo4118.cn

PHP:  // 手写递归函数
来源：https://bv.zhonguo8118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://fl.zhonguo4118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://wd.zhonguo7118.cn

Java: // 手写递归
来源：https://nc.zhonguo8118.cn

Go:   // 手写递归
来源：https://er.zhonguo6118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://vx.zhonguo1118.cn

C#:   // 手写递归
来源：https://nh.zhonguo2118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://fw.zhonguo2118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://qg.zhonguo7118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://rx.zhonguo3118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://rf.zhonguo4118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://rc.zhonguo3118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://xr.zhonguo3118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://iw.zhonguo8118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://xt.zhonguo7118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://aa.zhonguo7118.cn

================================================================================
来源：https://bv.zhonguo1118.cn

O. 并发与异步
来源：https://lq.zhonguo6118.cn

================================================================================
来源：https://vj.zhonguo2118.cn

[O01] 启动一个线程
来源：https://ze.zhonguo3118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://di.zhonguo6118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://gd.zhonguo5118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://fr.zhonguo7118.cn

TS:   // 同 JS
来源：https://mu.zhonguo2118.cn

Java: new Thread(() -> f()).start()
来源：https://uz.zhonguo3118.cn

Go:   go f()
来源：https://bn.zhonguo6118.cn

Ruby: Thread.new { f }
来源：https://jy.zhonguo2118.cn

C#:   Task.Run(() => F());
来源：https://au.zhonguo3118.cn

[O02] 使用线程池
来源：https://dq.zhonguo4118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://ga.zhonguo3118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://wu.zhonguo3118.cn

JS:   // worker_threads 线程池
来源：https://bm.zhonguo7118.cn

TS:   // worker_threads 线程池
来源：https://fo.zhonguo4118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://ya.zhonguo7118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://hl.zhonguo4118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://ht.zhonguo7118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://zn.zhonguo6118.cn

[O03] 加锁保护共享数据
来源：https://hq.zhonguo6118.cn

Py:   with lock: shared += 1
来源：https://kl.zhonguo2118.cn

PHP:  // 用 flock() 做文件锁
来源：https://jl.zhonguo2118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://ck.zhonguo5118.cn

TS:   // 同 JS
来源：https://xe.zhonguo7118.cn

Java: synchronized (this) { shared++; }
来源：https://hk.zhonguo7118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://cz.zhonguo8118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://bx.zhonguo3118.cn

C#:   lock (gate) { shared++; }
来源：https://ce.zhonguo5118.cn

[O04] 定义异步函数并等待
来源：https://uv.zhonguo5118.cn

Py:   async def f():⏎    await g()
来源：https://wv.zhonguo4118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://wc.zhonguo6118.cn

JS:   async function f() { await g(); }
来源：https://yz.zhonguo8118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://nv.zhonguo3118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://gk.zhonguo8118.cn


<!-- 参考信息 -->