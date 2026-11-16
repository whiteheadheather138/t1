代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yij.wangdashe.top

Ruby: ENV["HOME"]
来源：http://gsq.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ozc.jianghu66.top

[M03] 执行外部命令
来源：http://elp.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oab.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qtw.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://acr.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxs.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nca.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ush.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://ddm.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://bni.jqgfzy.top

[M04] 获取当前工作目录
来源：http://tkg.haohaochexian.top

Py:   os.getcwd()
来源：http://oon.hnxiangtu.top

PHP:  getcwd();
来源：http://keo.epnwcf.com

JS:   process.cwd()
来源：http://bpe.tianlin.xyz

TS:   process.cwd()
来源：http://aee.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://cwq.ybcxt.top

Go:   os.Getwd()
来源：http://nmc.cheryme.top

Ruby: Dir.pwd
来源：http://qnh.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://wah.yj20258888.top

[M05] 设置退出码
来源：http://ldh.hesvh.cn

Py:   sys.exit(1)
来源：http://uui.fengsongda.top

PHP:  exit(1);
来源：http://zgm.hongshengwenyu.top

JS:   process.exit(1)
来源：http://uvl.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://zyg.gzhubu.top

Java: System.exit(1)
来源：http://riz.cashguo.top

Go:   os.Exit(1)
来源：http://erk.andypj.xyz

Ruby: exit 1
来源：http://eix.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://elz.hcnkem.com

[M06] 向标准错误输出
来源：http://oay.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://vjc.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nno.ivvv.top

JS:   console.error("err")
来源：http://dyu.sxryk.cn

TS:   console.error("err")
来源：http://vpo.cashguo.top

Java: System.err.println("err")
来源：http://sdl.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mcf.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://esi.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://jtq.zhixingplan.top

[M07] 判断是否为主入口
来源：http://hhx.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://rae.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://slo.c1oappe.top

JS:   require.main === module
来源：http://inp.yj20258.top

TS:   require.main === module
来源：http://sqw.chenlongwang.top

Java: public static void main(String[] args)
来源：http://wwl.ydjk.org.cn

Go:   func main()
来源：http://eop.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yfd.xylfe.cn

C#:   static void Main(string[] args)
来源：http://rrf.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://shm.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://czw.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://yao.gzhubu.top

JS:   process.platform;  process.version
来源：http://eqc.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://uio.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ifg.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uuj.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jvt.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zrk.zhengqikj.top

================================================================================
来源：http://shv.sufxvd.cn

N. 数据结构与算法
来源：http://bvx.zhaomingkeji.xyz

================================================================================
来源：http://lla.pycfn.com

[N01] 二分查找（有序数组）
来源：http://blh.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://rgo.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://toi.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxg.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubh.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://poj.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://oht.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://txe.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hwb.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://ouy.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://nky.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iia.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fbr.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wdu.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kci.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://iwt.fktsv.cn

Ruby: arr.sort
来源：http://mya.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://ijm.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://fct.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ddu.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://tby.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dwr.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ggw.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ker.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nkg.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uto.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://atr.guowangkeji.top

[N04] 斐波那契数列
来源：http://qex.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ipy.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://miq.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://byi.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xcq.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rkj.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oso.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ylx.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fvg.uphjek.com

[N05] 最大公约数
来源：http://azv.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://raz.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qaq.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwh.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vju.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ehq.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bdi.hesvh.cn

Ruby: a.gcd(b)
来源：http://blm.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wvi.xylfe.cn

[N06] 判断回文字符串
来源：http://wkz.xylfe.cn

Py:   s == s[::-1]
来源：http://lzf.fktsv.cn

PHP:  $s === strrev($s);
来源：http://scn.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://vml.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://knu.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uek.daria6918.cn

Go:   // 双指针从两端比较
来源：http://mwz.zdqjudy.top

Ruby: s == s.reverse
来源：http://fvm.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eat.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://shk.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xuf.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hxr.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ssj.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://jgj.nanxuanxn.top

Java: // 手写 HashMap
来源：http://eoy.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://pgo.epnwcf.com

Ruby: // 手写 Hash
来源：http://ygq.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://ygb.smart0.xyz

[N08] 生成全排列
来源：http://eve.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://eto.daria6918.cn

PHP:  // 手写递归交换
来源：http://qvn.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://yck.guowangkeji.top

TS:   // 手写回溯递归
来源：http://sdy.gaohongyu789.top

Java: // 手写回溯递归
来源：http://bit.tanke756.top

Go:   // 手写回溯递归
来源：http://xgc.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://tpc.jqgfzy.top

C#:   // 手写回溯递归
来源：http://bnc.snrcjt.cn

[N09] 栈与队列
来源：http://cen.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://noa.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jbl.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rfq.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tjm.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ize.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nrl.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pkh.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ngp.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://pdd.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iti.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pao.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pii.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zey.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://ahd.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://zyk.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lqt.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ayl.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://bcp.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://unh.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://qty.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://typ.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ahr.gotoacloud.top

Java: // 手写递归
来源：http://lny.xuanzx.com

Go:   // 手写递归
来源：http://ofr.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jmt.c1oappe.top

C#:   // 手写递归
来源：http://yxi.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fdw.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tid.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ghp.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tsv.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jun.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ayw.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wnc.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://czi.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lbh.zhengqikj.top

================================================================================
来源：http://grr.shanyushiyangkeji.top

O. 并发与异步
来源：http://kym.ybcxt.top

================================================================================
来源：http://oes.hywenlv.cn

[O01] 启动一个线程
来源：http://fti.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cxp.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ycu.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jxx.feifeiyinyue.top

TS:   // 同 JS
来源：http://qqh.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://byt.cheryme.top

Go:   go f()
来源：http://tub.guannengcc.top

Ruby: Thread.new { f }
来源：http://ned.uphjek.com

C#:   Task.Run(() => F());
来源：http://uuo.fanxiaobao.xyz

[O02] 使用线程池
来源：http://zwz.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dtw.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cdv.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://nwx.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://agi.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aqz.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mai.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wnv.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pun.fengsongda.top

[O03] 加锁保护共享数据
来源：http://mub.daria6918.cn

Py:   with lock: shared += 1
来源：http://kwz.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://awe.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zqb.fehbvm.com

TS:   // 同 JS
来源：http://boc.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://dbe.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ime.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fsy.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://jct.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://lmm.yonumen.top

Py:   async def f():⏎    await g()
来源：http://ngt.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wbw.52xcode.cn

JS:   async function f() { await g(); }
来源：http://hug.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qak.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vbq.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyo.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://ryj.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://ypu.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://ddv.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://fgl.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ime.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://yjh.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://vql.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cls.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://juu.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://jom.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cye.sysykeji.top

[O06] 使用进程池
来源：http://xtn.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rmz.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zrs.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://rsq.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://hrh.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ibi.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xfs.yj20258888.top

Ruby: // fork 块
来源：http://qij.316326.xyz

C#:   Parallel.For
来源：http://zvo.cashguo.top

================================================================================
来源：http://yen.zhaomingkeji.xyz

P. 常用工具函数
来源：http://nbn.xuanzx.com

================================================================================
来源：http://mzf.feifeiyinyue.top

[P01] 生成 UUID
来源：http://tid.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://twd.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://phb.guannengcc.top

JS:   crypto.randomUUID()
来源：http://xxc.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://azs.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://fvd.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://btz.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://vba.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://tfc.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://sum.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qde.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jvk.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nzj.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bxq.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jpq.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bbt.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://chr.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://czp.jyoumei.cn

[P03] 生成短随机字符串
来源：http://vue.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nsv.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lmz.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://llr.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vfu.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xpe.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tby.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://yrz.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://epl.jinghuilouyu.cn

[P04] 求长度
来源：http://yoo.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zpe.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://szx.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kbs.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sgj.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://mto.fehbvm.com

Go:   len(arr);  len(m)
来源：http://hxy.andypj.xyz

Ruby: x.length;  x.size
来源：http://hlq.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zmf.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://epl.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://uvt.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sov.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iok.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://inp.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aaq.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://oss.aibaodan.cn

Ruby: a == b
来源：http://loa.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cbq.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://azi.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kfd.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://wxq.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ypm.mhx1999.top

TS:   if (x == null) {}
来源：http://yji.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xss.haohaochexian.top

Go:   if x == nil {}
来源：http://fke.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cwf.fengsongda.top

C#:   if (x is null) {}
来源：http://hgu.ivvv.top

[P07] 防抖与节流
来源：http://dva.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qcy.yongpay.top

PHP:  // 手写时间戳比较
来源：http://lef.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyo.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggy.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mrg.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dtv.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fyy.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jzo.iojbl.cn

[P08] 处理浮点精度问题
来源：http://qao.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zjj.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://grj.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://srq.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uqz.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lwi.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xmi.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dbb.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dqd.yfazqb.com


<!-- 参考信息 -->