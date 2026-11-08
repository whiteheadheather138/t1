代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://lz.zhonguo1118.cn

[L04] 设置超时
来源：https://vq.zhonguo1118.cn

Py:   requests.get(url, timeout=5)
来源：https://rl.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://aj.zhonguo1118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://eb.zhonguo6118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://qu.zhonguo4118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://gn.zhonguo7118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://aw.zhonguo5118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://rj.zhonguo1118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://kv.zhonguo3118.cn

[L05] 上传文件（multipart）
来源：https://zp.zhonguo5118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://oz.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://el.zhonguo1118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://nm.zhonguo7118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://cn.zhonguo7118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://ln.zhonguo7118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://re.zhonguo6118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://my.zhonguo3118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://vr.zhonguo5118.cn

[L06] 解析响应为 JSON
来源：https://yk.zhonguo6118.cn

Py:   resp.json()
来源：https://ru.zhonguo1118.cn

PHP:  json_decode($body, true);
来源：https://jl.zhonguo7118.cn

JS:   await resp.json()
来源：https://ws.zhonguo4118.cn

TS:   await resp.json()
来源：https://km.zhonguo5118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://or.zhonguo5118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://zi.zhonguo8118.cn

Ruby: JSON.parse(resp.body)
来源：https://ff.zhonguo8118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://vo.zhonguo4118.cn

[L07] 处理 HTTP 状态码
来源：https://uf.zhonguo2118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://gz.zhonguo3118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://zs.zhonguo4118.cn

JS:   resp.ok;  resp.status
来源：https://wb.zhonguo3118.cn

TS:   resp.ok;  resp.status
来源：https://kq.zhonguo3118.cn

Java: resp.statusCode()
来源：https://pz.zhonguo7118.cn

Go:   resp.StatusCode
来源：https://yv.zhonguo7118.cn

Ruby: resp.code.to_i
来源：https://tz.zhonguo8118.cn

C#:   (int)resp.StatusCode
来源：https://yo.zhonguo7118.cn

[L08] 并发请求多个地址
来源：https://bp.zhonguo2118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://gc.zhonguo6118.cn

PHP:  curl_multi_init() 系列
来源：https://vi.zhonguo1118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://uu.zhonguo2118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://ct.zhonguo6118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://ex.zhonguo3118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://yk.zhonguo3118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://sk.zhonguo6118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://al.zhonguo1118.cn

================================================================================
来源：https://sj.zhonguo3118.cn

M. 命令行 / 进程 / 环境
来源：https://tg.zhonguo8118.cn

================================================================================
来源：https://hr.zhonguo6118.cn

[M01] 读取命令行参数
来源：https://sa.zhonguo1118.cn

Py:   sys.argv[1:]
来源：https://vv.zhonguo1118.cn

PHP:  $argv;  $argc;
来源：https://og.zhonguo2118.cn

JS:   process.argv.slice(2)
来源：https://de.zhonguo6118.cn

TS:   process.argv.slice(2)
来源：https://mc.zhonguo2118.cn

Java: args 数组（main 方法参数）
来源：https://ly.zhonguo8118.cn

Go:   os.Args[1:]
来源：https://sq.zhonguo7118.cn

Ruby: ARGV
来源：https://vg.zhonguo6118.cn

C#:   args 数组（Main 方法参数）
来源：https://hx.zhonguo3118.cn

[M02] 读取环境变量
来源：https://hp.zhonguo4118.cn

Py:   os.environ.get("HOME")
来源：https://ab.zhonguo2118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://nq.zhonguo2118.cn

JS:   process.env.HOME
来源：https://dq.zhonguo1118.cn

TS:   process.env.HOME
来源：https://jw.zhonguo1118.cn

Java: System.getenv("HOME")
来源：https://ky.zhonguo4118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://bd.zhonguo7118.cn

Ruby: ENV["HOME"]
来源：https://ik.zhonguo5118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://ol.zhonguo2118.cn

[M03] 执行外部命令
来源：https://zc.zhonguo5118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://rh.zhonguo3118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://am.zhonguo3118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://cf.zhonguo2118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://yc.zhonguo3118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://rg.zhonguo1118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://oo.zhonguo6118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://yy.zhonguo7118.cn

C#:   Process.Start("ls", "-l");
来源：https://bp.zhonguo6118.cn

[M04] 获取当前工作目录
来源：https://sw.zhonguo3118.cn

Py:   os.getcwd()
来源：https://zw.zhonguo2118.cn

PHP:  getcwd();
来源：https://hb.zhonguo7118.cn

JS:   process.cwd()
来源：https://ap.zhonguo5118.cn

TS:   process.cwd()
来源：https://pc.zhonguo8118.cn

Java: Path.of("").toAbsolutePath()
来源：https://nx.zhonguo1118.cn

Go:   os.Getwd()
来源：https://cu.zhonguo1118.cn

Ruby: Dir.pwd
来源：https://ht.zhonguo6118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://gt.zhonguo5118.cn

[M05] 设置退出码
来源：https://pz.zhonguo6118.cn

Py:   sys.exit(1)
来源：https://st.zhonguo1118.cn

PHP:  exit(1);
来源：https://zo.zhonguo3118.cn

JS:   process.exit(1)
来源：https://xy.zhonguo6118.cn

TS:   process.exit(1)
来源：https://mt.zhonguo1118.cn

Java: System.exit(1)
来源：https://un.zhonguo2118.cn

Go:   os.Exit(1)
来源：https://ez.zhonguo7118.cn

Ruby: exit 1
来源：https://yg.zhonguo2118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://zs.zhonguo1118.cn

[M06] 向标准错误输出
来源：https://ib.zhonguo1118.cn

Py:   print("err", file=sys.stderr)
来源：https://sy.zhonguo5118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://uj.zhonguo1118.cn

JS:   console.error("err")
来源：https://fj.zhonguo6118.cn

TS:   console.error("err")
来源：https://cu.zhonguo5118.cn

Java: System.err.println("err")
来源：https://ou.zhonguo4118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://au.zhonguo4118.cn

Ruby: warn "err"
来源：https://jg.zhonguo3118.cn

C#:   Console.Error.WriteLine("err")
来源：https://fb.zhonguo3118.cn

[M07] 判断是否为主入口
来源：https://qe.zhonguo7118.cn

Py:   if __name__ == "__main__":
来源：https://xp.zhonguo3118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://ql.zhonguo7118.cn

JS:   require.main === module
来源：https://gv.zhonguo4118.cn

TS:   require.main === module
来源：https://fb.zhonguo8118.cn

Java: public static void main(String[] args)
来源：https://mk.zhonguo6118.cn

Go:   func main()
来源：https://ss.zhonguo6118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://it.zhonguo2118.cn

C#:   static void Main(string[] args)
来源：https://bb.zhonguo8118.cn

[M08] 获取系统与运行时信息
来源：https://rw.zhonguo2118.cn

Py:   platform.system();  platform.python_version()
来源：https://kc.zhonguo5118.cn

PHP:  PHP_OS;  phpversion();
来源：https://bs.zhonguo4118.cn

JS:   process.platform;  process.version
来源：https://na.zhonguo1118.cn

TS:   process.platform;  process.version
来源：https://nt.zhonguo2118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://il.zhonguo5118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://tl.zhonguo7118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://ew.zhonguo1118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://xv.zhonguo8118.cn

================================================================================
来源：https://vv.zhonguo4118.cn

N. 数据结构与算法
来源：https://zk.zhonguo6118.cn

================================================================================
来源：https://cm.zhonguo5118.cn

[N01] 二分查找（有序数组）
来源：https://eo.zhonguo1118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://kg.zhonguo1118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://if.zhonguo2118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://lb.zhonguo8118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://ro.zhonguo1118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://bx.zhonguo1118.cn

Go:   sort.SearchInts(arr, x)
来源：https://pa.zhonguo3118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://tj.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://pt.zhonguo5118.cn

[N02] 排序（工程实践用内置实现）
来源：https://ap.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://pj.zhonguo3118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://xo.zhonguo8118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://ab.zhonguo4118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://oz.zhonguo8118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://by.zhonguo4118.cn

Go:   slices.Sort(arr)
来源：https://bu.zhonguo5118.cn

Ruby: arr.sort
来源：https://pw.zhonguo6118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://lj.zhonguo4118.cn

[N03] 快速排序（分治示例）
来源：https://ec.zhonguo8118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://rx.zhonguo8118.cn

PHP:  // 递归实现，或用 usort
来源：https://cw.zhonguo8118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://fb.zhonguo5118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://rt.zhonguo1118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://fm.zhonguo7118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://el.zhonguo2118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://yh.zhonguo6118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://hl.zhonguo6118.cn

[N04] 斐波那契数列
来源：https://ig.zhonguo1118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://mu.zhonguo5118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://sv.zhonguo5118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://pa.zhonguo1118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://jj.zhonguo6118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://zn.zhonguo1118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://fh.zhonguo8118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://ky.zhonguo7118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://oy.zhonguo6118.cn

[N05] 最大公约数
来源：https://mj.zhonguo2118.cn

Py:   math.gcd(a, b)
来源：https://xb.zhonguo1118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://ds.zhonguo7118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://ox.zhonguo3118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://hm.zhonguo1118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://wj.zhonguo7118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://vz.zhonguo7118.cn

Ruby: a.gcd(b)
来源：https://xf.zhonguo2118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://ec.zhonguo6118.cn

[N06] 判断回文字符串
来源：https://fp.zhonguo3118.cn

Py:   s == s[::-1]
来源：https://bv.zhonguo6118.cn

PHP:  $s === strrev($s);
来源：https://yz.zhonguo3118.cn

JS:   s === [...s].reverse().join("")
来源：https://nl.zhonguo6118.cn

TS:   s === [...s].reverse().join("")
来源：https://do.zhonguo7118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://rr.zhonguo3118.cn

Go:   // 双指针从两端比较
来源：https://hd.zhonguo1118.cn

Ruby: s == s.reverse
来源：https://ju.zhonguo3118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://fl.zhonguo2118.cn

[N07] 两数之和（返回下标）
来源：https://ld.zhonguo6118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://do.zhonguo5118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://jk.zhonguo1118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://qn.zhonguo8118.cn

TS:   // 手写 Map<string, number>
来源：https://vo.zhonguo4118.cn

Java: // 手写 HashMap
来源：https://ha.zhonguo5118.cn

Go:   // 手写 map[int]int
来源：https://ki.zhonguo6118.cn

Ruby: // 手写 Hash
来源：https://dt.zhonguo4118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://ev.zhonguo2118.cn

[N08] 生成全排列
来源：https://qy.zhonguo1118.cn

Py:   itertools.permutations(arr)
来源：https://eq.zhonguo2118.cn

PHP:  // 手写递归交换
来源：https://nf.zhonguo6118.cn

JS:   // 手写回溯递归
来源：https://gr.zhonguo5118.cn

TS:   // 手写回溯递归
来源：https://go.zhonguo8118.cn

Java: // 手写回溯递归
来源：https://fv.zhonguo3118.cn

Go:   // 手写回溯递归
来源：https://rq.zhonguo8118.cn

Ruby: arr.permutation.to_a
来源：https://hj.zhonguo2118.cn

C#:   // 手写回溯递归
来源：https://qk.zhonguo1118.cn

[N09] 栈与队列
来源：https://uw.zhonguo1118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://hr.zhonguo2118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://sw.zhonguo4118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://kd.zhonguo4118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://qo.zhonguo2118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://kx.zhonguo3118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://kq.zhonguo7118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://xn.zhonguo6118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://qr.zhonguo1118.cn

[N10] 链表节点定义
来源：https://nu.zhonguo1118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://qf.zhonguo7118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://jh.zhonguo5118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://tk.zhonguo6118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://xl.zhonguo8118.cn

Java: class Node { int v; Node next; }
来源：https://iq.zhonguo1118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://fd.zhonguo3118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://nt.zhonguo4118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://xa.zhonguo8118.cn

[N11] 二叉树中序遍历
来源：https://tt.zhonguo2118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://mq.zhonguo3118.cn

PHP:  // 手写递归函数
来源：https://lb.zhonguo8118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://jo.zhonguo8118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://vo.zhonguo7118.cn

Java: // 手写递归
来源：https://xx.zhonguo7118.cn

Go:   // 手写递归
来源：https://wt.zhonguo1118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://ar.zhonguo3118.cn

C#:   // 手写递归
来源：https://lg.zhonguo1118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://ad.zhonguo3118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://cv.zhonguo6118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://gn.zhonguo1118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://zc.zhonguo4118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://wd.zhonguo5118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://po.zhonguo3118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://ev.zhonguo1118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://up.zhonguo2118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://kz.zhonguo2118.cn

================================================================================
来源：https://gu.zhonguo3118.cn

O. 并发与异步
来源：https://oe.zhonguo8118.cn

================================================================================
来源：https://ca.zhonguo6118.cn

[O01] 启动一个线程
来源：https://gu.zhonguo8118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://za.zhonguo2118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://fl.zhonguo6118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://td.zhonguo4118.cn

TS:   // 同 JS
来源：https://ol.zhonguo6118.cn

Java: new Thread(() -> f()).start()
来源：https://tq.zhonguo7118.cn

Go:   go f()
来源：https://dw.zhonguo6118.cn

Ruby: Thread.new { f }
来源：https://cq.zhonguo8118.cn

C#:   Task.Run(() => F());
来源：https://tv.zhonguo4118.cn

[O02] 使用线程池
来源：https://bz.zhonguo1118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://bg.zhonguo3118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://hp.zhonguo4118.cn

JS:   // worker_threads 线程池
来源：https://vf.zhonguo6118.cn

TS:   // worker_threads 线程池
来源：https://rz.zhonguo2118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://mn.zhonguo5118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://nr.zhonguo3118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://eg.zhonguo3118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://ut.zhonguo6118.cn

[O03] 加锁保护共享数据
来源：https://wu.zhonguo7118.cn

Py:   with lock: shared += 1
来源：https://aj.zhonguo1118.cn

PHP:  // 用 flock() 做文件锁
来源：https://ld.zhonguo7118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://hw.zhonguo8118.cn

TS:   // 同 JS
来源：https://yy.zhonguo2118.cn

Java: synchronized (this) { shared++; }
来源：https://sf.zhonguo1118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://ok.zhonguo7118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://dt.zhonguo4118.cn

C#:   lock (gate) { shared++; }
来源：https://ao.zhonguo1118.cn

[O04] 定义异步函数并等待
来源：https://cv.zhonguo2118.cn

Py:   async def f():⏎    await g()
来源：https://np.zhonguo3118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://yl.zhonguo1118.cn

JS:   async function f() { await g(); }
来源：https://ea.zhonguo5118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://so.zhonguo5118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://yx.zhonguo4118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://bk.zhonguo7118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://tx.zhonguo2118.cn

C#:   async Task F() { await G(); }
来源：https://ks.zhonguo8118.cn

[O05] 并发执行并等待全部完成
来源：https://gj.zhonguo6118.cn

Py:   asyncio.gather(*tasks)
来源：https://bq.zhonguo3118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://nz.zhonguo6118.cn

JS:   await Promise.all(tasks)
来源：https://wy.zhonguo8118.cn

TS:   await Promise.all(tasks)
来源：https://eh.zhonguo7118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://cy.zhonguo5118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://np.zhonguo4118.cn

Ruby: threads.map(&:join)
来源：https://mk.zhonguo8118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://bc.zhonguo1118.cn

[O06] 使用进程池
来源：https://xw.zhonguo8118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://ie.zhonguo3118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://aa.zhonguo4118.cn

JS:   // child_process / cluster 模块
来源：https://ww.zhonguo6118.cn

TS:   // child_process / cluster 模块
来源：https://ni.zhonguo3118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://xc.zhonguo5118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://hv.zhonguo3118.cn

Ruby: // fork 块
来源：https://ra.zhonguo8118.cn

C#:   Parallel.For
来源：https://ag.zhonguo7118.cn

================================================================================
来源：https://bo.zhonguo4118.cn

P. 常用工具函数
来源：https://jg.zhonguo5118.cn

================================================================================
来源：https://ti.zhonguo4118.cn

[P01] 生成 UUID
来源：https://rh.zhonguo6118.cn

Py:   str(uuid.uuid4())
来源：https://hf.zhonguo2118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://vv.zhonguo5118.cn

JS:   crypto.randomUUID()
来源：https://ly.zhonguo7118.cn

TS:   crypto.randomUUID()
来源：https://jw.zhonguo5118.cn

Java: UUID.randomUUID().toString()
来源：https://vx.zhonguo7118.cn

Go:   // 用 github.com/google/uuid
来源：https://yk.zhonguo3118.cn

Ruby: SecureRandom.uuid
来源：https://jd.zhonguo8118.cn


<!-- 参考信息 -->