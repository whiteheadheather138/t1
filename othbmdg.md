代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://aj.zhonguo6118.cn

[L04] 设置超时
来源：https://uh.zhonguo4118.cn

Py:   requests.get(url, timeout=5)
来源：https://qe.zhonguo6118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://lv.zhonguo5118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://lr.zhonguo7118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://em.zhonguo3118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://uh.zhonguo7118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://nc.zhonguo2118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://qe.zhonguo8118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://ky.zhonguo6118.cn

[L05] 上传文件（multipart）
来源：https://qa.zhonguo5118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://ys.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://jt.zhonguo3118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://wp.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://uj.zhonguo1118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://wf.zhonguo7118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://jx.zhonguo5118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://te.zhonguo4118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://pp.zhonguo1118.cn

[L06] 解析响应为 JSON
来源：https://rs.zhonguo2118.cn

Py:   resp.json()
来源：https://pz.zhonguo5118.cn

PHP:  json_decode($body, true);
来源：https://mn.zhonguo3118.cn

JS:   await resp.json()
来源：https://ut.zhonguo5118.cn

TS:   await resp.json()
来源：https://vd.zhonguo2118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://av.zhonguo1118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://yk.zhonguo6118.cn

Ruby: JSON.parse(resp.body)
来源：https://vv.zhonguo7118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://rh.zhonguo4118.cn

[L07] 处理 HTTP 状态码
来源：https://eu.zhonguo8118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://ru.zhonguo8118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://bx.zhonguo8118.cn

JS:   resp.ok;  resp.status
来源：https://bf.zhonguo1118.cn

TS:   resp.ok;  resp.status
来源：https://xk.zhonguo3118.cn

Java: resp.statusCode()
来源：https://ps.zhonguo2118.cn

Go:   resp.StatusCode
来源：https://bl.zhonguo1118.cn

Ruby: resp.code.to_i
来源：https://ph.zhonguo8118.cn

C#:   (int)resp.StatusCode
来源：https://mi.zhonguo7118.cn

[L08] 并发请求多个地址
来源：https://nt.zhonguo3118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://kd.zhonguo2118.cn

PHP:  curl_multi_init() 系列
来源：https://qa.zhonguo4118.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://rj.zhonguo4118.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：https://yt.zhonguo3118.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：https://hc.zhonguo6118.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：https://zg.zhonguo2118.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：https://cd.zhonguo4118.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：https://xg.zhonguo7118.cn

================================================================================
来源：https://ra.zhonguo1118.cn

M. 命令行 / 进程 / 环境
来源：https://sw.zhonguo4118.cn

================================================================================
来源：https://da.zhonguo7118.cn

[M01] 读取命令行参数
来源：https://gf.zhonguo5118.cn

Py:   sys.argv[1:]
来源：https://uh.zhonguo2118.cn

PHP:  $argv;  $argc;
来源：https://qn.zhonguo7118.cn

JS:   process.argv.slice(2)
来源：https://fg.zhonguo2118.cn

TS:   process.argv.slice(2)
来源：https://ky.zhonguo1118.cn

Java: args 数组（main 方法参数）
来源：https://tn.zhonguo1118.cn

Go:   os.Args[1:]
来源：https://nn.zhonguo3118.cn

Ruby: ARGV
来源：https://fu.zhonguo8118.cn

C#:   args 数组（Main 方法参数）
来源：https://ag.zhonguo2118.cn

[M02] 读取环境变量
来源：https://pz.zhonguo7118.cn

Py:   os.environ.get("HOME")
来源：https://cf.zhonguo3118.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：https://mx.zhonguo6118.cn

JS:   process.env.HOME
来源：https://ss.zhonguo4118.cn

TS:   process.env.HOME
来源：https://gg.zhonguo3118.cn

Java: System.getenv("HOME")
来源：https://ee.zhonguo4118.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：https://ke.zhonguo1118.cn

Ruby: ENV["HOME"]
来源：https://er.zhonguo5118.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：https://lz.zhonguo3118.cn

[M03] 执行外部命令
来源：https://ft.zhonguo3118.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：https://sf.zhonguo4118.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：https://kd.zhonguo6118.cn

JS:   child_process.execSync("ls -l").toString()
来源：https://lg.zhonguo7118.cn

TS:   child_process.execSync("ls -l").toString()
来源：https://nk.zhonguo3118.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：https://fj.zhonguo4118.cn

Go:   exec.Command("ls", "-l").Output()
来源：https://xo.zhonguo3118.cn

Ruby: system("ls -l");  `ls -l`
来源：https://yo.zhonguo4118.cn

C#:   Process.Start("ls", "-l");
来源：https://iy.zhonguo5118.cn

[M04] 获取当前工作目录
来源：https://rr.zhonguo3118.cn

Py:   os.getcwd()
来源：https://tc.zhonguo6118.cn

PHP:  getcwd();
来源：https://ds.zhonguo2118.cn

JS:   process.cwd()
来源：https://nr.zhonguo4118.cn

TS:   process.cwd()
来源：https://hn.zhonguo5118.cn

Java: Path.of("").toAbsolutePath()
来源：https://on.zhonguo8118.cn

Go:   os.Getwd()
来源：https://tj.zhonguo7118.cn

Ruby: Dir.pwd
来源：https://re.zhonguo2118.cn

C#:   Directory.GetCurrentDirectory()
来源：https://tr.zhonguo1118.cn

[M05] 设置退出码
来源：https://xp.zhonguo6118.cn

Py:   sys.exit(1)
来源：https://nl.zhonguo3118.cn

PHP:  exit(1);
来源：https://ec.zhonguo2118.cn

JS:   process.exit(1)
来源：https://wy.zhonguo1118.cn

TS:   process.exit(1)
来源：https://qa.zhonguo7118.cn

Java: System.exit(1)
来源：https://au.zhonguo3118.cn

Go:   os.Exit(1)
来源：https://bo.zhonguo8118.cn

Ruby: exit 1
来源：https://yj.zhonguo2118.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：https://gg.zhonguo5118.cn

[M06] 向标准错误输出
来源：https://wk.zhonguo5118.cn

Py:   print("err", file=sys.stderr)
来源：https://wa.zhonguo7118.cn

PHP:  fwrite(STDERR, "err\n");
来源：https://kf.zhonguo2118.cn

JS:   console.error("err")
来源：https://yz.zhonguo8118.cn

TS:   console.error("err")
来源：https://na.zhonguo4118.cn

Java: System.err.println("err")
来源：https://hp.zhonguo3118.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：https://ue.zhonguo1118.cn

Ruby: warn "err"
来源：https://tw.zhonguo8118.cn

C#:   Console.Error.WriteLine("err")
来源：https://my.zhonguo6118.cn

[M07] 判断是否为主入口
来源：https://yb.zhonguo7118.cn

Py:   if __name__ == "__main__":
来源：https://qt.zhonguo3118.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：https://fe.zhonguo4118.cn

JS:   require.main === module
来源：https://gv.zhonguo5118.cn

TS:   require.main === module
来源：https://cx.zhonguo7118.cn

Java: public static void main(String[] args)
来源：https://ib.zhonguo3118.cn

Go:   func main()
来源：https://qc.zhonguo3118.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：https://qp.zhonguo5118.cn

C#:   static void Main(string[] args)
来源：https://pb.zhonguo6118.cn

[M08] 获取系统与运行时信息
来源：https://fc.zhonguo5118.cn

Py:   platform.system();  platform.python_version()
来源：https://ah.zhonguo4118.cn

PHP:  PHP_OS;  phpversion();
来源：https://fz.zhonguo7118.cn

JS:   process.platform;  process.version
来源：https://wr.zhonguo4118.cn

TS:   process.platform;  process.version
来源：https://gg.zhonguo7118.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：https://fz.zhonguo5118.cn

Go:   runtime.GOOS;  runtime.Version()
来源：https://yj.zhonguo5118.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：https://km.zhonguo3118.cn

C#:   Environment.OSVersion;  Environment.Version
来源：https://ku.zhonguo8118.cn

================================================================================
来源：https://ls.zhonguo2118.cn

N. 数据结构与算法
来源：https://el.zhonguo1118.cn

================================================================================
来源：https://is.zhonguo3118.cn

[N01] 二分查找（有序数组）
来源：https://ct.zhonguo2118.cn

Py:   bisect.bisect_left(arr, x)
来源：https://pe.zhonguo4118.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：https://mt.zhonguo4118.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://zm.zhonguo7118.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：https://by.zhonguo5118.cn

Java: Arrays.binarySearch(arr, x)
来源：https://wi.zhonguo5118.cn

Go:   sort.SearchInts(arr, x)
来源：https://dj.zhonguo6118.cn

Ruby: arr.bsearch { |e| e >= x }
来源：https://rw.zhonguo8118.cn

C#:   Array.BinarySearch(arr, x)
来源：https://rs.zhonguo4118.cn

[N02] 排序（工程实践用内置实现）
来源：https://xg.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://aa.zhonguo3118.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：https://ex.zhonguo4118.cn

JS:   [...arr].sort((a, b) => a - b)
来源：https://gw.zhonguo4118.cn

TS:   [...arr].sort((a, b) => a - b)
来源：https://nr.zhonguo8118.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：https://il.zhonguo6118.cn

Go:   slices.Sort(arr)
来源：https://ye.zhonguo1118.cn

Ruby: arr.sort
来源：https://vm.zhonguo3118.cn

C#:   Array.Sort(arr);  list.Sort()
来源：https://gx.zhonguo4118.cn

[N03] 快速排序（分治示例）
来源：https://zq.zhonguo8118.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：https://ao.zhonguo7118.cn

PHP:  // 递归实现，或用 usort
来源：https://or.zhonguo2118.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://wu.zhonguo1118.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：https://le.zhonguo4118.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：https://ze.zhonguo2118.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：https://jq.zhonguo4118.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：https://ye.zhonguo7118.cn

C#:   // 手写递归，或 Array.Sort
来源：https://tb.zhonguo7118.cn

[N04] 斐波那契数列
来源：https://vr.zhonguo3118.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：https://nv.zhonguo2118.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：https://pf.zhonguo6118.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://cu.zhonguo6118.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：https://yy.zhonguo4118.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：https://sh.zhonguo2118.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：https://wm.zhonguo4118.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：https://at.zhonguo6118.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：https://df.zhonguo2118.cn

[N05] 最大公约数
来源：https://sp.zhonguo7118.cn

Py:   math.gcd(a, b)
来源：https://wf.zhonguo3118.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：https://ym.zhonguo8118.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://os.zhonguo5118.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：https://zu.zhonguo8118.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：https://yj.zhonguo1118.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：https://ss.zhonguo5118.cn

Ruby: a.gcd(b)
来源：https://ui.zhonguo8118.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：https://yg.zhonguo5118.cn

[N06] 判断回文字符串
来源：https://ma.zhonguo2118.cn

Py:   s == s[::-1]
来源：https://px.zhonguo1118.cn

PHP:  $s === strrev($s);
来源：https://se.zhonguo8118.cn

JS:   s === [...s].reverse().join("")
来源：https://iz.zhonguo8118.cn

TS:   s === [...s].reverse().join("")
来源：https://ao.zhonguo3118.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：https://od.zhonguo5118.cn

Go:   // 双指针从两端比较
来源：https://og.zhonguo8118.cn

Ruby: s == s.reverse
来源：https://xv.zhonguo2118.cn

C#:   s == new string(s.Reverse().ToArray())
来源：https://bu.zhonguo5118.cn

[N07] 两数之和（返回下标）
来源：https://wh.zhonguo1118.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：https://vp.zhonguo8118.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：https://lb.zhonguo1118.cn

JS:   // 手写 Map：map.set(v, i)
来源：https://pz.zhonguo8118.cn

TS:   // 手写 Map<string, number>
来源：https://kq.zhonguo7118.cn

Java: // 手写 HashMap
来源：https://mt.zhonguo3118.cn

Go:   // 手写 map[int]int
来源：https://dy.zhonguo6118.cn

Ruby: // 手写 Hash
来源：https://jf.zhonguo3118.cn

C#:   // 手写 Dictionary<int, int>
来源：https://kh.zhonguo5118.cn

[N08] 生成全排列
来源：https://xr.zhonguo8118.cn

Py:   itertools.permutations(arr)
来源：https://xm.zhonguo1118.cn

PHP:  // 手写递归交换
来源：https://eq.zhonguo6118.cn

JS:   // 手写回溯递归
来源：https://gp.zhonguo4118.cn

TS:   // 手写回溯递归
来源：https://vf.zhonguo8118.cn

Java: // 手写回溯递归
来源：https://pj.zhonguo8118.cn

Go:   // 手写回溯递归
来源：https://im.zhonguo4118.cn

Ruby: arr.permutation.to_a
来源：https://jg.zhonguo3118.cn

C#:   // 手写回溯递归
来源：https://vk.zhonguo8118.cn

[N09] 栈与队列
来源：https://vt.zhonguo2118.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：https://rw.zhonguo7118.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：https://ib.zhonguo7118.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：https://vk.zhonguo4118.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：https://hx.zhonguo8118.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：https://ba.zhonguo4118.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：https://wl.zhonguo7118.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：https://jp.zhonguo5118.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：https://ek.zhonguo1118.cn

[N10] 链表节点定义
来源：https://ew.zhonguo8118.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：https://hl.zhonguo6118.cn

PHP:  class Node { public $v; public $next = null; }
来源：https://ho.zhonguo2118.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：https://ef.zhonguo2118.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：https://zy.zhonguo7118.cn

Java: class Node { int v; Node next; }
来源：https://ro.zhonguo5118.cn

Go:   type Node struct { V int; Next *Node }
来源：https://cu.zhonguo5118.cn

Ruby: Node = Struct.new(:v, :next)
来源：https://sr.zhonguo6118.cn

C#:   class Node { public int V; public Node? Next; }
来源：https://ui.zhonguo7118.cn

[N11] 二叉树中序遍历
来源：https://br.zhonguo5118.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：https://tl.zhonguo1118.cn

PHP:  // 手写递归函数
来源：https://vs.zhonguo4118.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://js.zhonguo6118.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：https://qa.zhonguo5118.cn

Java: // 手写递归
来源：https://fv.zhonguo6118.cn

Go:   // 手写递归
来源：https://st.zhonguo8118.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：https://qv.zhonguo2118.cn

C#:   // 手写递归
来源：https://cy.zhonguo7118.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：https://dh.zhonguo6118.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：https://xt.zhonguo6118.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：https://nj.zhonguo8118.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://xe.zhonguo4118.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：https://vs.zhonguo1118.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：https://yk.zhonguo5118.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：https://vg.zhonguo4118.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：https://nw.zhonguo6118.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：https://hf.zhonguo2118.cn

================================================================================
来源：https://ip.zhonguo7118.cn

O. 并发与异步
来源：https://oq.zhonguo2118.cn

================================================================================
来源：https://ub.zhonguo2118.cn

[O01] 启动一个线程
来源：https://qb.zhonguo5118.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：https://xl.zhonguo6118.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：https://ng.zhonguo8118.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：https://tz.zhonguo4118.cn

TS:   // 同 JS
来源：https://uj.zhonguo4118.cn

Java: new Thread(() -> f()).start()
来源：https://gr.zhonguo7118.cn

Go:   go f()
来源：https://gg.zhonguo2118.cn

Ruby: Thread.new { f }
来源：https://cx.zhonguo1118.cn

C#:   Task.Run(() => F());
来源：https://zw.zhonguo3118.cn

[O02] 使用线程池
来源：https://hh.zhonguo1118.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：https://vn.zhonguo1118.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：https://xa.zhonguo7118.cn

JS:   // worker_threads 线程池
来源：https://kj.zhonguo5118.cn

TS:   // worker_threads 线程池
来源：https://at.zhonguo3118.cn

Java: Executors.newFixedThreadPool(4)
来源：https://wd.zhonguo3118.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：https://rg.zhonguo4118.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：https://yy.zhonguo3118.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：https://gc.zhonguo6118.cn

[O03] 加锁保护共享数据
来源：https://cq.zhonguo4118.cn

Py:   with lock: shared += 1
来源：https://iz.zhonguo7118.cn

PHP:  // 用 flock() 做文件锁
来源：https://vh.zhonguo3118.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：https://fu.zhonguo5118.cn

TS:   // 同 JS
来源：https://of.zhonguo7118.cn

Java: synchronized (this) { shared++; }
来源：https://tx.zhonguo3118.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：https://bi.zhonguo6118.cn

Ruby: mutex.synchronize { shared += 1 }
来源：https://xr.zhonguo2118.cn

C#:   lock (gate) { shared++; }
来源：https://fo.zhonguo8118.cn

[O04] 定义异步函数并等待
来源：https://rs.zhonguo2118.cn

Py:   async def f():⏎    await g()
来源：https://jo.zhonguo2118.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：https://ym.zhonguo2118.cn

JS:   async function f() { await g(); }
来源：https://mr.zhonguo6118.cn

TS:   async function f(): Promise<void> { await g(); }
来源：https://vj.zhonguo4118.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：https://zz.zhonguo2118.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：https://px.zhonguo8118.cn

Ruby: # 用 Fiber 或 async gem
来源：https://zt.zhonguo1118.cn

C#:   async Task F() { await G(); }
来源：https://pr.zhonguo4118.cn

[O05] 并发执行并等待全部完成
来源：https://no.zhonguo5118.cn

Py:   asyncio.gather(*tasks)
来源：https://te.zhonguo8118.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：https://wh.zhonguo6118.cn

JS:   await Promise.all(tasks)
来源：https://li.zhonguo7118.cn

TS:   await Promise.all(tasks)
来源：https://tv.zhonguo5118.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：https://sm.zhonguo4118.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：https://po.zhonguo7118.cn

Ruby: threads.map(&:join)
来源：https://hs.zhonguo2118.cn

C#:   await Task.WhenAll(t1, t2)
来源：https://wm.zhonguo6118.cn

[O06] 使用进程池
来源：https://ig.zhonguo4118.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：https://ko.zhonguo8118.cn

PHP:  // pcntl_fork 或多进程队列
来源：https://ik.zhonguo3118.cn

JS:   // child_process / cluster 模块
来源：https://qx.zhonguo1118.cn

TS:   // child_process / cluster 模块
来源：https://xm.zhonguo8118.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：https://wy.zhonguo7118.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：https://eu.zhonguo2118.cn

Ruby: // fork 块
来源：https://du.zhonguo3118.cn

C#:   Parallel.For
来源：https://go.zhonguo3118.cn

================================================================================
来源：https://cm.zhonguo6118.cn

P. 常用工具函数
来源：https://kt.zhonguo1118.cn

================================================================================
来源：https://pr.zhonguo6118.cn

[P01] 生成 UUID
来源：https://it.zhonguo8118.cn

Py:   str(uuid.uuid4())
来源：https://mi.zhonguo4118.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：https://qr.zhonguo1118.cn

JS:   crypto.randomUUID()
来源：https://hs.zhonguo8118.cn

TS:   crypto.randomUUID()
来源：https://cn.zhonguo3118.cn

Java: UUID.randomUUID().toString()
来源：https://ig.zhonguo4118.cn

Go:   // 用 github.com/google/uuid
来源：https://hs.zhonguo2118.cn

Ruby: SecureRandom.uuid
来源：https://lg.zhonguo4118.cn


<!-- 参考信息 -->