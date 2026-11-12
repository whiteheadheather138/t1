代发 wailian999

Py:   resp.json()
来源：http://pzo.yongpay.top

PHP:  json_decode($body, true);
来源：http://jzz.hammf.cn

JS:   await resp.json()
来源：http://hxn.tianlin.xyz

TS:   await resp.json()
来源：http://fxu.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mkg.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wzm.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://nfu.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://okx.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://cko.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nwk.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mwt.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://vgg.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://cjw.vehdjk.com

Java: resp.statusCode()
来源：http://oql.316326.xyz

Go:   resp.StatusCode
来源：http://bdr.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://kjl.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://bou.hywenlv.cn

[L08] 并发请求多个地址
来源：http://edb.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dln.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://pcj.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bnj.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qfu.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://otf.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xyl.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dew.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nrb.cheryme.top

================================================================================
来源：http://iqj.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://keo.0kj1m.cn

================================================================================
来源：http://bou.yuxming.cn

[M01] 读取命令行参数
来源：http://jwg.yuxming.cn

Py:   sys.argv[1:]
来源：http://uil.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://cqn.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://hir.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://dqn.ivvv.top

Java: args 数组（main 方法参数）
来源：http://zyk.tianlin.xyz

Go:   os.Args[1:]
来源：http://squ.jqgfzy.top

Ruby: ARGV
来源：http://uma.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://cjf.ybcxt.top

[M02] 读取环境变量
来源：http://wuj.havefunace.top

Py:   os.environ.get("HOME")
来源：http://uhf.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rqo.gotoacloud.top

JS:   process.env.HOME
来源：http://dfa.gogol.net.cn

TS:   process.env.HOME
来源：http://qqr.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://tfz.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jlg.gzhubu.top

Ruby: ENV["HOME"]
来源：http://hge.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cxn.shuidangran.top

[M03] 执行外部命令
来源：http://kyw.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://inl.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zal.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jdt.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mby.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bnu.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://lrr.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bci.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://fdl.birdmap.top

[M04] 获取当前工作目录
来源：http://xll.hesvh.cn

Py:   os.getcwd()
来源：http://ria.kuanghao11.cn

PHP:  getcwd();
来源：http://qyh.jqgfzy.top

JS:   process.cwd()
来源：http://suh.yongpay.top

TS:   process.cwd()
来源：http://ajv.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://hzq.sysykeji.top

Go:   os.Getwd()
来源：http://ead.sufxvd.cn

Ruby: Dir.pwd
来源：http://eon.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://nps.daria6918.cn

[M05] 设置退出码
来源：http://cik.aizwys.cn

Py:   sys.exit(1)
来源：http://wti.jinqigufen.top

PHP:  exit(1);
来源：http://vom.yuanzhike.top

JS:   process.exit(1)
来源：http://yyp.yanxiufei.cn

TS:   process.exit(1)
来源：http://znu.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://evh.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://pwm.gaohongyu789.top

Ruby: exit 1
来源：http://hcc.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://inh.sxryk.cn

[M06] 向标准错误输出
来源：http://nen.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://rwm.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://xiq.jinqigfzy.top

JS:   console.error("err")
来源：http://cfk.vqdsnc.cn

TS:   console.error("err")
来源：http://agr.aizwys.cn

Java: System.err.println("err")
来源：http://tmz.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mog.hesvh.cn

Ruby: warn "err"
来源：http://eki.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://urv.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://wkz.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://gny.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wfq.ybcxt.top

JS:   require.main === module
来源：http://fxi.meibo888.top

TS:   require.main === module
来源：http://qsu.yfazqb.com

Java: public static void main(String[] args)
来源：http://vra.jlsjyb.cn

Go:   func main()
来源：http://dja.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mmq.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://ilw.birdmap.top

[M08] 获取系统与运行时信息
来源：http://fts.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://ppr.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://kad.yuanzhike.top

JS:   process.platform;  process.version
来源：http://pxz.jqgfzy.top

TS:   process.platform;  process.version
来源：http://cyf.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://koz.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://izq.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tok.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://owo.kuanghao11.cn

================================================================================
来源：http://ift.havefunace.top

N. 数据结构与算法
来源：http://fvg.zhongyouzk.top

================================================================================
来源：http://olm.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://ndk.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://eam.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vim.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://seb.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://frw.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sji.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://csd.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mhr.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dor.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://utp.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://ogb.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mha.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zyn.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ers.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://duz.cheryme.top

Go:   slices.Sort(arr)
来源：http://fom.snrcjt.cn

Ruby: arr.sort
来源：http://vsw.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vfu.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://knv.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://psr.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://zej.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dyj.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://czg.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fcj.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ojg.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pnz.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://thf.aizwys.cn

[N04] 斐波那契数列
来源：http://bim.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ylx.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pug.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gwq.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vvp.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qem.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vfb.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ppd.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fer.hysaishi.cn

[N05] 最大公约数
来源：http://xcc.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://jmf.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qvq.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnw.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgz.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://spj.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tpl.hnqzz.top

Ruby: a.gcd(b)
来源：http://hnp.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://znu.cdnleiting.top

[N06] 判断回文字符串
来源：http://lvg.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://pub.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://yrq.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://juu.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://ayi.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zrm.daxiang520.top

Go:   // 双指针从两端比较
来源：http://csa.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://rbx.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lls.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://ldj.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ehv.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gis.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ijx.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://jxo.gogol.net.cn

Java: // 手写 HashMap
来源：http://ute.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://xts.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://jyt.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://avl.ehwqpu.com

[N08] 生成全排列
来源：http://kbs.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://slh.vehdjk.com

PHP:  // 手写递归交换
来源：http://gxy.nwbrower.top

JS:   // 手写回溯递归
来源：http://fgj.hammf.cn

TS:   // 手写回溯递归
来源：http://gjn.cashguo.top

Java: // 手写回溯递归
来源：http://cvf.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://jrg.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://qfq.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://bhs.jinqigfzy.top

[N09] 栈与队列
来源：http://qjb.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fsn.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kqo.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ffp.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://unv.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://phw.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zic.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fmf.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zbe.daria6918.cn

[N10] 链表节点定义
来源：http://iig.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://crc.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://xhc.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ekw.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yws.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://amf.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://ccl.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://liy.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gxt.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://fcy.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://urn.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://qld.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bpe.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lla.bbcook.cn

Java: // 手写递归
来源：http://bhl.fzhhl.top

Go:   // 手写递归
来源：http://vzg.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iyq.iojbl.cn

C#:   // 手写递归
来源：http://uyd.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wzp.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dqx.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exq.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://acu.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://upy.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dwy.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sjf.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://muj.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jsz.yj20258888.top

================================================================================
来源：http://yxc.sysykeji.top

O. 并发与异步
来源：http://iee.haohaochexian.top

================================================================================
来源：http://ike.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://cct.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fhl.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://etx.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yeu.iojbl.cn

TS:   // 同 JS
来源：http://sac.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://kkr.yvedp.cn

Go:   go f()
来源：http://gfn.aizwys.cn

Ruby: Thread.new { f }
来源：http://oxh.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://fjs.cheryme.top

[O02] 使用线程池
来源：http://lmg.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ynx.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eze.hcnkem.com

JS:   // worker_threads 线程池
来源：http://nrm.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://ply.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://qrs.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://igq.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zor.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://etu.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://arl.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://jtp.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://idz.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rvl.cashguo.top

TS:   // 同 JS
来源：http://ljr.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://nmh.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pwf.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://brn.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://img.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://atb.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://qml.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dyr.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://eki.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jsh.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kxo.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://udv.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tey.yj202588.top

C#:   async Task F() { await G(); }
来源：http://gnh.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://ldn.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://hch.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ekh.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://vqo.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://hmf.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qih.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bve.xziqi.cn

Ruby: threads.map(&:join)
来源：http://pbz.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sfj.wangshuangyany.cn

[O06] 使用进程池
来源：http://kbz.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zwd.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ono.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://esi.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://mzm.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ori.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fuu.chenlongwang.top

Ruby: // fork 块
来源：http://aos.xylfe.cn

C#:   Parallel.For
来源：http://qxr.zdqjudy.top

================================================================================
来源：http://hlz.aizwys.cn

P. 常用工具函数
来源：http://bni.yonumen.top

================================================================================
来源：http://nmz.fktsv.cn

[P01] 生成 UUID
来源：http://poz.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://knf.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dki.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://aeb.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://ccz.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://fyu.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://nkj.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://rpo.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://kad.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://qpo.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://owz.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rfv.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://prh.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ekk.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ljq.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wvc.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ifk.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kou.andypj.xyz

[P03] 生成短随机字符串
来源：http://sny.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://evh.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tcs.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://agb.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kef.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://awn.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://szg.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iiq.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://imc.fengsongda.top

[P04] 求长度
来源：http://kfs.zhiwuduotai.top


<!-- 参考信息 -->