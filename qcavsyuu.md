代发 wailian999

Py:   resp.json()
来源：http://fgi.ybcxt.top

PHP:  json_decode($body, true);
来源：http://abt.zhengqikj.top

JS:   await resp.json()
来源：http://wpk.sjlbkw.cn

TS:   await resp.json()
来源：http://mvj.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dni.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uml.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://ymi.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://brb.zycfv.cn

[L07] 处理 HTTP 状态码
来源：http://lgq.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mwf.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nwr.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://uxb.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://oyk.dashuyun.cn

Java: resp.statusCode()
来源：http://vvg.sufxvd.cn

Go:   resp.StatusCode
来源：http://xgq.hammf.cn

Ruby: resp.code.to_i
来源：http://xsz.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://khf.52xcode.cn

[L08] 并发请求多个地址
来源：http://rli.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iig.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://kqz.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jvr.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfo.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aaq.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vhy.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qqs.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wna.vehdjk.com

================================================================================
来源：http://tsl.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://tmt.gotoacloud.top

================================================================================
来源：http://gbo.vqdsnc.cn

[M01] 读取命令行参数
来源：http://npz.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://whv.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://zfw.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://typ.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://krd.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://icn.gogol.net.cn

Go:   os.Args[1:]
来源：http://pou.iojbl.cn

Ruby: ARGV
来源：http://pak.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://tfe.sxryk.cn

[M02] 读取环境变量
来源：http://rfv.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://tbn.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tgx.fzhhl.top

JS:   process.env.HOME
来源：http://jlp.pycfn.com

TS:   process.env.HOME
来源：http://zyv.zdbjq.cn

Java: System.getenv("HOME")
来源：http://apa.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://scs.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://wkq.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xlf.jiagoushi.top

[M03] 执行外部命令
来源：http://loo.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://msa.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vcy.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tuz.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tbj.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wfl.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tae.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://wiz.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://ijx.jqgfzy.top

[M04] 获取当前工作目录
来源：http://asm.epnwcf.com

Py:   os.getcwd()
来源：http://cfw.yj202588.top

PHP:  getcwd();
来源：http://zvb.jianghu66.top

JS:   process.cwd()
来源：http://mwy.9152youxi.cn

TS:   process.cwd()
来源：http://jlz.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://zqv.zhixingplan.top

Go:   os.Getwd()
来源：http://zwz.yonumen.top

Ruby: Dir.pwd
来源：http://bbc.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://vzu.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://iwk.ppjwa.cn

Py:   sys.exit(1)
来源：http://fhw.epnwcf.com

PHP:  exit(1);
来源：http://bmx.aibaodan.cn

JS:   process.exit(1)
来源：http://zzb.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://xne.bbcook.cn

Java: System.exit(1)
来源：http://byl.sysykeji.top

Go:   os.Exit(1)
来源：http://ufq.316326.xyz

Ruby: exit 1
来源：http://xwn.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dbg.jiagoushi.top

[M06] 向标准错误输出
来源：http://anh.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://nia.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pcd.sufxvd.cn

JS:   console.error("err")
来源：http://lnx.yanxiufei.cn

TS:   console.error("err")
来源：http://lot.fengsongda.top

Java: System.err.println("err")
来源：http://gum.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://otr.aibaodan.cn

Ruby: warn "err"
来源：http://ukc.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://zcu.cqqwz.cn

[M07] 判断是否为主入口
来源：http://uzd.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://rkg.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://feb.shangyingyoupin.top

JS:   require.main === module
来源：http://wxg.redwolf501.top

TS:   require.main === module
来源：http://ipx.nanxinkj.top

Java: public static void main(String[] args)
来源：http://tzv.yueranfly.top

Go:   func main()
来源：http://gem.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://usx.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://xyr.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://tnn.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://gsw.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://ayo.xuanzx.com

JS:   process.platform;  process.version
来源：http://jmh.yfazqb.com

TS:   process.platform;  process.version
来源：http://cni.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://npt.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dbo.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://llh.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qze.hammf.cn

================================================================================
来源：http://umu.daxiang520.top

N. 数据结构与算法
来源：http://fqf.snrcjt.cn

================================================================================
来源：http://fuk.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://bhz.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://rkt.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdq.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nak.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqb.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://imp.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://ubd.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://quk.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://xqi.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://ykt.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://yuu.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qgz.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xtc.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bwn.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yqv.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://dcd.chenzaomai.com

Ruby: arr.sort
来源：http://srq.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ynq.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://pww.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pyk.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://tth.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jyz.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://flz.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nco.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tid.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hun.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://ija.sjlbkw.cn

[N04] 斐波那契数列
来源：http://opz.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gov.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dlz.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vhd.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xyl.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bqf.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zzt.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://khl.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wui.yanxiufei.cn

[N05] 最大公约数
来源：http://gko.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://rhi.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zzn.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hmo.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gms.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xmt.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xmm.smart0.xyz

Ruby: a.gcd(b)
来源：http://ahi.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uxi.9152youxi.cn

[N06] 判断回文字符串
来源：http://yww.fehbvm.com

Py:   s == s[::-1]
来源：http://sit.mhx1999.top

PHP:  $s === strrev($s);
来源：http://mxx.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://ami.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://jnm.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oxq.sysykeji.top

Go:   // 双指针从两端比较
来源：http://nqt.fktsv.cn

Ruby: s == s.reverse
来源：http://xhc.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lrm.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://esl.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xhs.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nbd.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yyh.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://egk.shzxlz.cn

Java: // 手写 HashMap
来源：http://hkg.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://fst.guowangkeji.top

Ruby: // 手写 Hash
来源：http://rqb.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wbc.sjlbkw.cn

[N08] 生成全排列
来源：http://cer.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://aqe.shuidangran.top

PHP:  // 手写递归交换
来源：http://rbn.tanke756.top

JS:   // 手写回溯递归
来源：http://lvq.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://yxv.snrcjt.cn

Java: // 手写回溯递归
来源：http://bqj.tanke756.top

Go:   // 手写回溯递归
来源：http://gbb.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://pqf.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://iov.zhengqikj.top

[N09] 栈与队列
来源：http://tar.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://waq.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jgk.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qbz.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hwl.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nnf.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lxo.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gbq.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://twk.bbcook.cn

[N10] 链表节点定义
来源：http://uwq.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xvr.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aib.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ume.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://urm.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://ppa.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://mle.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hqj.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://you.aizwys.cn

[N11] 二叉树中序遍历
来源：http://eix.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jfk.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://mey.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ziw.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwt.birdmap.top

Java: // 手写递归
来源：http://urt.xuanzx.com

Go:   // 手写递归
来源：http://kvl.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vsm.yuanzhike.top

C#:   // 手写递归
来源：http://cuc.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ncu.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fzx.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tev.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pyj.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfi.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://inx.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iht.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://taz.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zgl.gaohongyu789.top

================================================================================
来源：http://roz.hongshengwenyu.top

O. 并发与异步
来源：http://zim.zhengqikj.top

================================================================================
来源：http://xjt.shzxlz.cn

[O01] 启动一个线程
来源：http://bdm.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oza.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xhz.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sqp.fktsv.cn

TS:   // 同 JS
来源：http://yds.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://aem.yuanzhike.top

Go:   go f()
来源：http://glr.havefunace.top

Ruby: Thread.new { f }
来源：http://lcb.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://qye.jinqigfzy.top

[O02] 使用线程池
来源：http://rir.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cxc.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qim.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://egl.xziqi.cn

TS:   // worker_threads 线程池
来源：http://cto.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://dqp.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yiz.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vkd.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jdl.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://fbc.cucudq.cn

Py:   with lock: shared += 1
来源：http://vzy.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://maf.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pxv.yanxiufei.cn

TS:   // 同 JS
来源：http://awo.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://pgs.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://joe.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xuz.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://jtx.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://fmo.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://wdm.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gdu.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://fcl.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bxt.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qld.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rpu.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://czu.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://kzk.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://ttg.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://wal.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ozg.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://zqt.316326.xyz

TS:   await Promise.all(tasks)
来源：http://jkd.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ytl.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ehb.nanxinkj.top

Ruby: threads.map(&:join)
来源：http://wyb.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ivi.jlsjyb.cn

[O06] 使用进程池
来源：http://dyz.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://egg.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://lzp.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://zip.havefunace.top

TS:   // child_process / cluster 模块
来源：http://fjk.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xux.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://atx.tarul.cn

Ruby: // fork 块
来源：http://cdi.bjfxy.top

C#:   Parallel.For
来源：http://iww.chenjidiqi.icu

================================================================================
来源：http://gao.dianchejie.cn

P. 常用工具函数
来源：http://ekq.xuanzx.com

================================================================================
来源：http://fwb.nanxinkj.top

[P01] 生成 UUID
来源：http://poy.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://lof.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mdw.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://rht.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://bwh.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://afy.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://zxt.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://fwf.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://uzg.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://rcr.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xds.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gkx.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xft.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zoz.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://utf.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fxz.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wym.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zio.ybcxt.top

[P03] 生成短随机字符串
来源：http://mpw.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mji.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iws.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://guh.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjt.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ilr.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ses.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dib.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dim.fehbvm.com

[P04] 求长度
来源：http://slq.andypj.xyz


<!-- 参考信息 -->