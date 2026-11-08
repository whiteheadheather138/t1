代发 wailian999

[L03] 设置自定义请求头
来源：https://sy.zhonguo2118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://xp.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://am.zhonguo1118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://qv.zhonguo3118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ap.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://ya.zhonguo7118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://rf.zhonguo6118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://po.zhonguo7118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://sh.zhonguo2118.cn

[L04] 设置超时
来源：https://zx.zhonguo5118.cn

Py:   requests.get(url, timeout=5)
来源：https://lv.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://ul.zhonguo6118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://xy.zhonguo3118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://co.zhonguo1118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://fc.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://wf.zhonguo7118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://nu.zhonguo8118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://do.zhonguo1118.cn

[L05] 上传文件（multipart）
来源：https://wo.zhonguo8118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://lt.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://mk.zhonguo8118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://zd.zhonguo8118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://qu.zhonguo4118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://gj.zhonguo8118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://we.zhonguo7118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ip.zhonguo1118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://im.zhonguo5118.cn

[L06] 解析响应为 JSON
来源：https://ry.zhonguo4118.cn

Py:   resp.json()
来源：https://gv.zhonguo1118.cn

PHP:  json_decode($body, true);
来源：https://yr.zhonguo4118.cn

JS:   await resp.json()
来源：https://ls.zhonguo3118.cn

TS:   await resp.json()
来源：https://yy.zhonguo1118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://zl.zhonguo2118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://px.zhonguo8118.cn

Ruby: JSON.parse(resp.body)
来源：https://si.zhonguo6118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://rd.zhonguo8118.cn

[L07] 处理 HTTP 状态码
来源：https://vj.zhonguo8118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://dw.zhonguo8118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://fl.zhonguo3118.cn

JS:   resp.ok;  resp.status
来源：https://ey.zhonguo3118.cn

TS:   resp.ok;  resp.status
来源：https://cy.zhonguo1118.cn

Java: resp.statusCode()
来源：https://gt.zhonguo5118.cn

Go:   resp.StatusCode
来源：https://jc.zhonguo8118.cn

Ruby: resp.code.to_i
来源：https://tp.zhonguo5118.cn

C#:   (int)resp.StatusCode
来源：https://vl.zhonguo8118.cn

[L08] 并发请求多个地址
来源：https://fn.zhonguo6118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://mi.zhonguo7118.cn

PHP:  curl_multi_init() 系列
来源：https://wq.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://zt.zhonguo7118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://og.zhonguo6118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://cx.zhonguo1118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://xa.zhonguo7118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://oz.zhonguo1118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://ak.zhonguo8118.cn

================================================================================
来源：https://fh.zhonguo1118.cn

M. 命令行 / 进程 / 环境
来源：https://go.zhonguo3118.cn

================================================================================
来源：https://jc.zhonguo6118.cn

[M01] 读取命令行参数
来源：https://to.zhonguo4118.cn

Py:   sys.argv[1:]
来源：https://we.zhonguo2118.cn

PHP:  $argv;  $argc;
来源：https://kn.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://nq.zhonguo1118.cn

TS:   process.argv.slice(2)
来源：https://bj.zhonguo4118.cn

Java: args 数组（main 方法参数）
来源：https://yf.zhonguo8118.cn

Go:   os.Args[1:]
来源：https://mp.zhonguo2118.cn

Ruby: ARGV
来源：https://fh.zhonguo3118.cn

C#:   args 数组（Main 方法参数）
来源：https://vw.zhonguo7118.cn

[M02] 读取环境变量
来源：https://yi.zhonguo5118.cn

Py:   os.environ.get("HOME")
来源：https://if.zhonguo5118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://dn.zhonguo8118.cn

JS:   process.env.HOME
来源：https://dq.zhonguo5118.cn

TS:   process.env.HOME
来源：https://xd.zhonguo7118.cn

Java: System.getenv("HOME")
来源：https://xm.zhonguo1118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://ht.zhonguo1118.cn

Ruby: ENV["HOME"]
来源：https://tw.zhonguo6118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://xa.zhonguo6118.cn

[M03] 执行外部命令
来源：https://bh.zhonguo2118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://wk.zhonguo6118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://ru.zhonguo6118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://rw.zhonguo3118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://ba.zhonguo8118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://dk.zhonguo3118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://vs.zhonguo5118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://zd.zhonguo7118.cn

C#:   Process.Start("ls", "-l");
来源：https://dn.zhonguo7118.cn

[M04] 获取当前工作目录
来源：https://oj.zhonguo6118.cn

Py:   os.getcwd()
来源：https://ka.zhonguo8118.cn

PHP:  getcwd();
来源：https://qv.zhonguo4118.cn

JS:   process.cwd()
来源：https://qt.zhonguo3118.cn

TS:   process.cwd()
来源：https://kz.zhonguo1118.cn

Java: Path.of("").toAbsolutePath()
来源：https://vy.zhonguo2118.cn

Go:   os.Getwd()
来源：https://nr.zhonguo8118.cn

Ruby: Dir.pwd
来源：https://ns.zhonguo5118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://ou.zhonguo8118.cn

[M05] 设置退出码
来源：https://mv.zhonguo5118.cn

Py:   sys.exit(1)
来源：https://gc.zhonguo8118.cn

PHP:  exit(1);
来源：https://vq.zhonguo4118.cn

JS:   process.exit(1)
来源：https://lw.zhonguo5118.cn

TS:   process.exit(1)
来源：https://xb.zhonguo7118.cn

Java: System.exit(1)
来源：https://tp.zhonguo4118.cn

Go:   os.Exit(1)
来源：https://mc.zhonguo7118.cn

Ruby: exit 1
来源：https://mi.zhonguo6118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://sk.zhonguo6118.cn

[M06] 向标准错误输出
来源：https://oq.zhonguo3118.cn

Py:   print("err", file=sys.stderr)
来源：https://ni.zhonguo4118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://gx.zhonguo7118.cn

JS:   console.error("err")
来源：https://jg.zhonguo4118.cn

TS:   console.error("err")
来源：https://vx.zhonguo7118.cn

Java: System.err.println("err")
来源：https://wk.zhonguo4118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://gh.zhonguo6118.cn

Ruby: warn "err"
来源：https://bi.zhonguo1118.cn

C#:   Console.Error.WriteLine("err")
来源：https://bn.zhonguo7118.cn

[M07] 判断是否为主入口
来源：https://lj.zhonguo8118.cn

Py:   if __name__ == "__main__":
来源：https://kk.zhonguo1118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://xk.zhonguo4118.cn

JS:   require.main === module
来源：https://sj.zhonguo3118.cn

TS:   require.main === module
来源：https://mp.zhonguo5118.cn

Java: public static void main(String[] args)
来源：https://js.zhonguo5118.cn

Go:   func main()
来源：https://ni.zhonguo3118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://yz.zhonguo1118.cn

C#:   static void Main(string[] args)
来源：https://rd.zhonguo2118.cn

[M08] 获取系统与运行时信息
来源：https://ls.zhonguo4118.cn

Py:   platform.system();  platform.python_version()
来源：https://ie.zhonguo7118.cn

PHP:  PHP_OS;  phpversion();
来源：https://dr.zhonguo8118.cn

JS:   process.platform;  process.version
来源：https://mu.zhonguo4118.cn

TS:   process.platform;  process.version
来源：https://wn.zhonguo7118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://um.zhonguo1118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://gb.zhonguo1118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://ui.zhonguo1118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://ck.zhonguo7118.cn

================================================================================
来源：https://tl.zhonguo1118.cn

N. 数据结构与算法
来源：https://ut.zhonguo1118.cn

================================================================================
来源：https://bb.zhonguo4118.cn

[N01] 二分查找（有序数组）
来源：https://zq.zhonguo5118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://or.zhonguo3118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://qt.zhonguo2118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://jz.zhonguo3118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://hs.zhonguo1118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://dx.zhonguo2118.cn

Go:   sort.SearchInts(arr, x)
来源：https://sc.zhonguo7118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://mo.zhonguo5118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://gw.zhonguo5118.cn

[N02] 排序（工程实践用内置实现）
来源：https://du.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://ta.zhonguo3118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://hd.zhonguo6118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://eg.zhonguo2118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://kf.zhonguo2118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://bu.zhonguo3118.cn

Go:   slices.Sort(arr)
来源：https://ze.zhonguo6118.cn

Ruby: arr.sort
来源：https://nt.zhonguo2118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://oa.zhonguo7118.cn

[N03] 快速排序（分治示例）
来源：https://tv.zhonguo4118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://fk.zhonguo7118.cn

PHP:  // 递归实现，或用 usort
来源：https://bc.zhonguo2118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://jb.zhonguo4118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://ds.zhonguo8118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://iv.zhonguo6118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://ws.zhonguo7118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://nx.zhonguo1118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://hb.zhonguo8118.cn

[N04] 斐波那契数列
来源：https://ma.zhonguo4118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://tu.zhonguo4118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://nj.zhonguo2118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://pt.zhonguo3118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://xj.zhonguo2118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://tk.zhonguo2118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://jz.zhonguo6118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://ft.zhonguo3118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://vz.zhonguo5118.cn

[N05] 最大公约数
来源：https://ks.zhonguo1118.cn

Py:   math.gcd(a, b)
来源：https://tt.zhonguo3118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://ax.zhonguo2118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://rq.zhonguo1118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://lt.zhonguo8118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://wr.zhonguo3118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://id.zhonguo1118.cn

Ruby: a.gcd(b)
来源：https://wf.zhonguo8118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://hs.zhonguo5118.cn

[N06] 判断回文字符串
来源：https://hu.zhonguo6118.cn

Py:   s == s[::-1]
来源：https://gl.zhonguo6118.cn

PHP:  $s === strrev($s);
来源：https://im.zhonguo3118.cn

JS:   s === [...s].reverse().join("")
来源：https://rz.zhonguo2118.cn

TS:   s === [...s].reverse().join("")
来源：https://mv.zhonguo1118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://ln.zhonguo7118.cn

Go:   // 双指针从两端比较
来源：https://co.zhonguo6118.cn

Ruby: s == s.reverse
来源：https://fb.zhonguo1118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://pb.zhonguo8118.cn

[N07] 两数之和（返回下标）
来源：https://qp.zhonguo1118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://au.zhonguo7118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://ju.zhonguo6118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://rh.zhonguo3118.cn

TS:   // 手写 Map<string, number>
来源：https://li.zhonguo8118.cn

Java: // 手写 HashMap
来源：https://ru.zhonguo7118.cn

Go:   // 手写 map[int]int
来源：https://rx.zhonguo5118.cn

Ruby: // 手写 Hash
来源：https://jq.zhonguo5118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://ym.zhonguo4118.cn

[N08] 生成全排列
来源：https://jt.zhonguo3118.cn

Py:   itertools.permutations(arr)
来源：https://er.zhonguo6118.cn

PHP:  // 手写递归交换
来源：https://fc.zhonguo5118.cn

JS:   // 手写回溯递归
来源：https://zq.zhonguo4118.cn

TS:   // 手写回溯递归
来源：https://zo.zhonguo8118.cn

Java: // 手写回溯递归
来源：https://yj.zhonguo1118.cn

Go:   // 手写回溯递归
来源：https://ls.zhonguo3118.cn

Ruby: arr.permutation.to_a
来源：https://ki.zhonguo6118.cn

C#:   // 手写回溯递归
来源：https://ij.zhonguo7118.cn

[N09] 栈与队列
来源：https://bo.zhonguo7118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://fl.zhonguo8118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://yh.zhonguo6118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://tt.zhonguo3118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://ju.zhonguo6118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://wb.zhonguo1118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://lp.zhonguo3118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://os.zhonguo7118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://ma.zhonguo7118.cn

[N10] 链表节点定义
来源：https://yq.zhonguo3118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://an.zhonguo2118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://ve.zhonguo2118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://tw.zhonguo1118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://dc.zhonguo4118.cn

Java: class Node { int v; Node next; }
来源：https://ss.zhonguo1118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://rw.zhonguo6118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://cl.zhonguo6118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://ow.zhonguo7118.cn

[N11] 二叉树中序遍历
来源：https://st.zhonguo4118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://nm.zhonguo3118.cn

PHP:  // 手写递归函数
来源：https://gw.zhonguo8118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://dm.zhonguo1118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://ci.zhonguo2118.cn

Java: // 手写递归
来源：https://gj.zhonguo3118.cn

Go:   // 手写递归
来源：https://wq.zhonguo1118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://cz.zhonguo2118.cn

C#:   // 手写递归
来源：https://bo.zhonguo7118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://nb.zhonguo8118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://gi.zhonguo6118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://tq.zhonguo3118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://ks.zhonguo3118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://dc.zhonguo6118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://iu.zhonguo7118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://od.zhonguo4118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://mm.zhonguo1118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://qg.zhonguo5118.cn

================================================================================
来源：https://pb.zhonguo3118.cn

O. 并发与异步
来源：https://pc.zhonguo3118.cn

================================================================================
来源：https://zx.zhonguo4118.cn

[O01] 启动一个线程
来源：https://cv.zhonguo6118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://nc.zhonguo7118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://ya.zhonguo4118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://go.zhonguo4118.cn

TS:   // 同 JS
来源：https://jn.zhonguo6118.cn

Java: new Thread(() -> f()).start()
来源：https://iu.zhonguo4118.cn

Go:   go f()
来源：https://ne.zhonguo2118.cn

Ruby: Thread.new { f }
来源：https://nz.zhonguo6118.cn

C#:   Task.Run(() => F());
来源：https://gw.zhonguo2118.cn

[O02] 使用线程池
来源：https://li.zhonguo2118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://qc.zhonguo6118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://hl.zhonguo7118.cn

JS:   // worker_threads 线程池
来源：https://ma.zhonguo4118.cn

TS:   // worker_threads 线程池
来源：https://oz.zhonguo7118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://vp.zhonguo6118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://mt.zhonguo3118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://ef.zhonguo2118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://mw.zhonguo5118.cn

[O03] 加锁保护共享数据
来源：https://ww.zhonguo8118.cn

Py:   with lock: shared += 1
来源：https://na.zhonguo5118.cn

PHP:  // 用 flock() 做文件锁
来源：https://pd.zhonguo6118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://vl.zhonguo2118.cn

TS:   // 同 JS
来源：https://ar.zhonguo6118.cn

Java: synchronized (this) { shared++; }
来源：https://fp.zhonguo1118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://zk.zhonguo4118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://nm.zhonguo6118.cn

C#:   lock (gate) { shared++; }
来源：https://no.zhonguo7118.cn

[O04] 定义异步函数并等待
来源：https://dd.zhonguo8118.cn

Py:   async def f():⏎    await g()
来源：https://lr.zhonguo6118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://nv.zhonguo2118.cn

JS:   async function f() { await g(); }
来源：https://le.zhonguo5118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://zh.zhonguo3118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://bw.zhonguo3118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://ym.zhonguo6118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://ic.zhonguo3118.cn

C#:   async Task F() { await G(); }
来源：https://so.zhonguo2118.cn

[O05] 并发执行并等待全部完成
来源：https://yi.zhonguo4118.cn

Py:   asyncio.gather(*tasks)
来源：https://dw.zhonguo3118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://wl.zhonguo4118.cn

JS:   await Promise.all(tasks)
来源：https://vt.zhonguo8118.cn

TS:   await Promise.all(tasks)
来源：https://va.zhonguo1118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://cy.zhonguo4118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://vq.zhonguo6118.cn

Ruby: threads.map(&:join)
来源：https://mr.zhonguo3118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://wv.zhonguo5118.cn

[O06] 使用进程池
来源：https://bd.zhonguo6118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://hx.zhonguo2118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://ku.zhonguo7118.cn

JS:   // child_process / cluster 模块
来源：https://zo.zhonguo3118.cn

TS:   // child_process / cluster 模块
来源：https://gy.zhonguo2118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://go.zhonguo6118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://qv.zhonguo3118.cn

Ruby: // fork 块
来源：https://po.zhonguo2118.cn

C#:   Parallel.For
来源：https://iq.zhonguo1118.cn

================================================================================
来源：https://sy.zhonguo4118.cn

P. 常用工具函数
来源：https://ht.zhonguo1118.cn

================================================================================
来源：https://ax.zhonguo1118.cn


<!-- 参考信息 -->