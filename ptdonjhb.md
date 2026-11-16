代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bet.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rkv.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nlr.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://xsy.fengsongda.top

Py:   resp.json()
来源：http://mxn.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://csd.gogol.net.cn

JS:   await resp.json()
来源：http://tck.sufxvd.cn

TS:   await resp.json()
来源：http://mkh.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pgg.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kej.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://ndz.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jsj.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://uer.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yih.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mdt.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://unf.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://gsf.fengsongda.top

Java: resp.statusCode()
来源：http://lsc.vehdjk.com

Go:   resp.StatusCode
来源：http://nea.shzxlz.cn

Ruby: resp.code.to_i
来源：http://oop.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://bhw.yonumen.top

[L08] 并发请求多个地址
来源：http://oyw.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bjj.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://fxt.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lue.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mqj.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gqq.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xiq.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eyc.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fem.ctjpmb.com

================================================================================
来源：http://ohf.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://oix.chenjidiqi.icu

================================================================================
来源：http://lje.xziqi.cn

[M01] 读取命令行参数
来源：http://khg.birdmap.top

Py:   sys.argv[1:]
来源：http://srx.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://pfc.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://etv.yuxming.cn

TS:   process.argv.slice(2)
来源：http://udm.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://oai.jqgufenzy.top

Go:   os.Args[1:]
来源：http://trj.sjlbkw.cn

Ruby: ARGV
来源：http://yuy.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://utd.vqdsnc.cn

[M02] 读取环境变量
来源：http://lzh.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://pfr.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ivv.fzhhl.top

JS:   process.env.HOME
来源：http://kjv.cqqwz.cn

TS:   process.env.HOME
来源：http://aft.zycfv.cn

Java: System.getenv("HOME")
来源：http://cst.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bzi.fehbvm.com

Ruby: ENV["HOME"]
来源：http://vxb.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xgc.yangfankeji.com

[M03] 执行外部命令
来源：http://mfa.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jza.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uqr.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kyj.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wcv.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ufe.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jul.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tcq.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://gpb.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://uta.meibo888.top

Py:   os.getcwd()
来源：http://tsz.fehbvm.com

PHP:  getcwd();
来源：http://tnf.daxiang520.top

JS:   process.cwd()
来源：http://vpd.fanxiaobao.xyz

TS:   process.cwd()
来源：http://wnf.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://kab.yanxiufei.cn

Go:   os.Getwd()
来源：http://ogx.yuanzhike.top

Ruby: Dir.pwd
来源：http://zgd.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://qap.zhengqikj.top

[M05] 设置退出码
来源：http://eye.jinqigufen.top

Py:   sys.exit(1)
来源：http://lra.xinyue.icu

PHP:  exit(1);
来源：http://jmi.yongpay.top

JS:   process.exit(1)
来源：http://pur.cqqwz.cn

TS:   process.exit(1)
来源：http://pdg.hfpthk.cn

Java: System.exit(1)
来源：http://sff.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://nrl.smart0.xyz

Ruby: exit 1
来源：http://qms.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vhy.dashuyun.cn

[M06] 向标准错误输出
来源：http://txz.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://uri.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yvg.52xcode.cn

JS:   console.error("err")
来源：http://kyg.zhoulong.xyz

TS:   console.error("err")
来源：http://irc.guowangkeji.top

Java: System.err.println("err")
来源：http://vja.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aiq.fengsongda.top

Ruby: warn "err"
来源：http://gbx.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://lus.yj202588.top

[M07] 判断是否为主入口
来源：http://irn.cheryme.top

Py:   if __name__ == "__main__":
来源：http://tod.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ime.mhx1999.top

JS:   require.main === module
来源：http://nnj.nanxinkj.top

TS:   require.main === module
来源：http://azu.hysaishi.cn

Java: public static void main(String[] args)
来源：http://ksb.hongshengwenyu.top

Go:   func main()
来源：http://ejc.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hpk.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://qdi.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://tho.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://jmd.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://orh.zycfv.cn

JS:   process.platform;  process.version
来源：http://qgt.hnqzz.top

TS:   process.platform;  process.version
来源：http://ngf.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iya.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vrn.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rep.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://jkf.yfazqb.com

================================================================================
来源：http://qvs.chenjidiqi.icu

N. 数据结构与算法
来源：http://hhc.zdbjq.cn

================================================================================
来源：http://iha.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://amr.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://tdt.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dcn.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eku.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ymi.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wra.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://nlh.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nyg.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://vgw.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://apx.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://hkw.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vco.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ukm.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://noj.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fhb.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://nta.dianchejie.cn

Ruby: arr.sort
来源：http://wnd.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bky.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://bfe.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qbj.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://uqn.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vxv.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gba.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rwq.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://doy.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dxv.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://kbh.andypj.xyz

[N04] 斐波那契数列
来源：http://ikq.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lgv.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vgu.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mqy.ctjpmb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtq.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tyq.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://idb.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gue.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ocb.smart0.xyz

[N05] 最大公约数
来源：http://rgy.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://qpq.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dlj.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxf.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qge.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qkb.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://phl.zhengqikj.top

Ruby: a.gcd(b)
来源：http://fxl.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kkb.yuxming.cn

[N06] 判断回文字符串
来源：http://ect.jyoumei.cn

Py:   s == s[::-1]
来源：http://fte.wangdashe.top

PHP:  $s === strrev($s);
来源：http://tcl.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://sbf.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://wmq.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iif.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://pbg.chenlongwang.top

Ruby: s == s.reverse
来源：http://nis.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lui.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://bth.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://szq.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cxv.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pmh.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://mos.gaohongyu789.top

Java: // 手写 HashMap
来源：http://mmu.xinyue.icu

Go:   // 手写 map[int]int
来源：http://ibs.hnqzz.top

Ruby: // 手写 Hash
来源：http://bcb.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qga.xylfe.cn

[N08] 生成全排列
来源：http://zgz.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://tec.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://ffz.aizwys.cn

JS:   // 手写回溯递归
来源：http://rnu.c1oappe.top

TS:   // 手写回溯递归
来源：http://tfs.yj20258.top

Java: // 手写回溯递归
来源：http://uet.zhixingplan.top

Go:   // 手写回溯递归
来源：http://ybq.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://hhg.ydzc1.top

C#:   // 手写回溯递归
来源：http://pau.ivvv.top

[N09] 栈与队列
来源：http://dgq.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yom.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://erl.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sxf.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kwm.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fzk.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://orz.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mzl.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qkq.svipenyu.cn

[N10] 链表节点定义
来源：http://dgw.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pat.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kwj.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nwz.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sfw.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ksi.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://evq.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dls.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oje.tarul.cn

[N11] 二叉树中序遍历
来源：http://nhz.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://odm.redwolf501.top

PHP:  // 手写递归函数
来源：http://axx.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lil.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihc.yuxming.cn

Java: // 手写递归
来源：http://dyv.hysaishi.cn

Go:   // 手写递归
来源：http://bzc.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mlz.chenjidiqi.icu

C#:   // 手写递归
来源：http://zwg.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ios.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aba.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qvg.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://omn.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://boh.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nif.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zip.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tyw.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tde.kuanghao11.cn

================================================================================
来源：http://bru.jqgufenzy.top

O. 并发与异步
来源：http://ixv.shzxlz.cn

================================================================================
来源：http://nry.nwbrower.top

[O01] 启动一个线程
来源：http://qeu.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://szo.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dsj.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eja.birdmap.top

TS:   // 同 JS
来源：http://sbk.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://cxn.hywenlv.cn

Go:   go f()
来源：http://isv.jiagoushi.top

Ruby: Thread.new { f }
来源：http://frb.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://qrg.yfazqb.com

[O02] 使用线程池
来源：http://sie.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fxp.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hly.tarul.cn

JS:   // worker_threads 线程池
来源：http://pfm.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://xcv.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://uqj.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ohd.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sov.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lza.zycfv.cn

[O03] 加锁保护共享数据
来源：http://yps.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://dyl.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://dru.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gfs.sysykeji.top

TS:   // 同 JS
来源：http://gpo.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://mjs.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iak.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://udd.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://dsz.mhx1999.top

[O04] 定义异步函数并等待
来源：http://twm.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://olt.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jpo.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://rlx.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://poq.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qlg.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rsi.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fve.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://wpa.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://sqz.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://smd.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blk.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://ouo.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://fzc.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hrx.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lvq.hesvh.cn

Ruby: threads.map(&:join)
来源：http://tlk.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://xea.chenjidiqi.icu

[O06] 使用进程池
来源：http://ikj.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vuw.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sdr.uphjek.com

JS:   // child_process / cluster 模块
来源：http://tec.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://swp.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dbj.shuidangran.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://joc.pengpengdd.cyou

Ruby: // fork 块
来源：http://met.jqgufenzy.top

C#:   Parallel.For
来源：http://hxw.pengpengdd.cyou

================================================================================
来源：http://uwm.shanyushiyangkeji.top

P. 常用工具函数
来源：http://qmn.yvedp.cn

================================================================================
来源：http://zli.chenjidiqi.icu

[P01] 生成 UUID
来源：http://qtz.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://omi.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kfn.bbcook.cn

JS:   crypto.randomUUID()
来源：http://xvn.yuxming.cn

TS:   crypto.randomUUID()
来源：http://oht.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://ooo.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://uas.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://xpq.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://ixv.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://szn.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qvd.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qno.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gvi.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yzl.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hyh.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wrz.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nal.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sid.bjfxy.top

[P03] 生成短随机字符串
来源：http://dow.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gzy.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qwf.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cno.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://htr.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ovy.jinyuanbaomall.cn


<!-- 参考信息 -->