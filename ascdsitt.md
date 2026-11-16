代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ase.sjlbkw.cn

JS:   process.env.HOME
来源：http://qcw.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://oqf.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://wxq.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mxb.shuidangran.top

Ruby: ENV["HOME"]
来源：http://bbe.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tii.pycfn.com

[M03] 执行外部命令
来源：http://jyy.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zgk.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fcp.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zvv.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iga.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pve.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ngy.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://cjg.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://jjp.xuanzx.com

[M04] 获取当前工作目录
来源：http://tpd.9152youxi.cn

Py:   os.getcwd()
来源：http://ieb.daria6918.cn

PHP:  getcwd();
来源：http://oiz.vqdsnc.cn

JS:   process.cwd()
来源：http://kbw.tianlin.xyz

TS:   process.cwd()
来源：http://uos.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://rfp.sjlbkw.cn

Go:   os.Getwd()
来源：http://dmf.jqgufenzy.top

Ruby: Dir.pwd
来源：http://rcq.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vsn.nwbrower.top

[M05] 设置退出码
来源：http://cct.vqdsnc.cn

Py:   sys.exit(1)
来源：http://rza.zhixingplan.top

PHP:  exit(1);
来源：http://psh.aibaodan.cn

JS:   process.exit(1)
来源：http://oua.cucudq.cn

TS:   process.exit(1)
来源：http://ctp.hnxiangtu.top

Java: System.exit(1)
来源：http://lyg.nanxuanxn.top

Go:   os.Exit(1)
来源：http://wtn.bbcook.cn

Ruby: exit 1
来源：http://lga.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gps.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://flg.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://igl.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://zfq.xziqi.cn

JS:   console.error("err")
来源：http://ugp.redwolf501.top

TS:   console.error("err")
来源：http://jme.uphjek.com

Java: System.err.println("err")
来源：http://ozv.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mqk.fengsongda.top

Ruby: warn "err"
来源：http://mjw.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://eoi.shuidangran.top

[M07] 判断是否为主入口
来源：http://qwo.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://tfz.vqdsnc.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nzs.sxryk.cn

JS:   require.main === module
来源：http://bxw.jqgfzy.top

TS:   require.main === module
来源：http://pof.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://gcu.yanxiufei.cn

Go:   func main()
来源：http://eqg.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xfo.mhx1999.top

C#:   static void Main(string[] args)
来源：http://rkz.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://ctj.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://sru.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://bne.sysykeji.top

JS:   process.platform;  process.version
来源：http://uql.tanke756.top

TS:   process.platform;  process.version
来源：http://fue.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iai.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aez.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cev.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ldg.tarul.cn

================================================================================
来源：http://kjo.wangshuangyany.cn

N. 数据结构与算法
来源：http://pze.fktsv.cn

================================================================================
来源：http://nry.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://cdq.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://fyg.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kez.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jov.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uaf.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://fae.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://mrc.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rsx.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vxa.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://zvs.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://tfs.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hlw.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wrx.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://upw.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uiv.daria6918.cn

Go:   slices.Sort(arr)
来源：http://bsw.xuanzx.com

Ruby: arr.sort
来源：http://xim.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wxn.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://ojg.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://itw.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://qsc.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plw.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ltv.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zsf.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ebf.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nmz.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://yrn.ehwqpu.com

[N04] 斐波那契数列
来源：http://pue.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gfr.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iuu.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yce.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vtk.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qdw.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fyo.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://inx.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hsz.hnxiangtu.top

[N05] 最大公约数
来源：http://eji.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://xjh.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uji.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrb.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://krw.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jfx.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://unp.bjfxy.top

Ruby: a.gcd(b)
来源：http://pyw.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxr.quarkkingdee.top

[N06] 判断回文字符串
来源：http://oxh.jianghu66.top

Py:   s == s[::-1]
来源：http://ysy.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://cny.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://kwm.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://ycm.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tmu.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://agw.tianlin.xyz

Ruby: s == s.reverse
来源：http://nrn.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://him.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://oio.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://axq.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sgf.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rvj.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://ram.meibo888.top

Java: // 手写 HashMap
来源：http://ztl.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://xra.dianchejie.cn

Ruby: // 手写 Hash
来源：http://ggo.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://nuw.aibaodan.cn

[N08] 生成全排列
来源：http://fwk.pycfn.com

Py:   itertools.permutations(arr)
来源：http://axl.xylfe.cn

PHP:  // 手写递归交换
来源：http://qkm.shzxlz.cn

JS:   // 手写回溯递归
来源：http://pgr.ydzc1.top

TS:   // 手写回溯递归
来源：http://hfu.epnwcf.com

Java: // 手写回溯递归
来源：http://vkd.mhx1999.top

Go:   // 手写回溯递归
来源：http://jfm.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://ecr.fktsv.cn

C#:   // 手写回溯递归
来源：http://wry.yj20258.top

[N09] 栈与队列
来源：http://thf.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ieh.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jft.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tqd.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jmp.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mtz.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eqw.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://knu.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xyg.nanxinkj.top

[N10] 链表节点定义
来源：http://uve.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ita.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sku.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uij.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yur.cheryme.top

Java: class Node { int v; Node next; }
来源：http://upf.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://zql.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bpz.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kvx.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://rra.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vqp.chenzaomai.com

PHP:  // 手写递归函数
来源：http://nqf.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ucx.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cev.epnwcf.com

Java: // 手写递归
来源：http://vmz.zhiwuduotai.top

Go:   // 手写递归
来源：http://cpy.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://but.shzxlz.cn

C#:   // 手写递归
来源：http://xvh.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vvw.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://idu.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ckv.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://twh.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnk.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qna.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vse.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eim.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ocx.dashuyun.cn

================================================================================
来源：http://kvd.yj20258888.top

O. 并发与异步
来源：http://toc.fehbvm.com

================================================================================
来源：http://xvb.c1oappe.top

[O01] 启动一个线程
来源：http://tqc.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iuf.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mmq.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://czl.jqgufenzy.top

TS:   // 同 JS
来源：http://zmj.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://yzn.yongpay.top

Go:   go f()
来源：http://kxq.hammf.cn

Ruby: Thread.new { f }
来源：http://jol.hesvh.cn

C#:   Task.Run(() => F());
来源：http://fjl.sxryk.cn

[O02] 使用线程池
来源：http://kax.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hih.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zza.yvedp.cn

JS:   // worker_threads 线程池
来源：http://pkt.pycfn.com

TS:   // worker_threads 线程池
来源：http://kpz.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://wxb.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hvg.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uow.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://age.yuxming.cn

[O03] 加锁保护共享数据
来源：http://ajy.tanke756.top

Py:   with lock: shared += 1
来源：http://cok.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://gcv.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pod.tianlin.xyz

TS:   // 同 JS
来源：http://psc.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://sit.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gva.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gju.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://iid.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://bae.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://qpx.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jqt.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://hdh.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ccq.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kvy.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kxe.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://pyd.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://fgb.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://pkj.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://ddt.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zwz.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://jmt.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://lcq.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wwf.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sin.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://owv.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qjz.jyoumei.cn

[O06] 使用进程池
来源：http://yfs.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xby.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://djz.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://cyl.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://cyy.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fnb.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ies.meibo888.top

Ruby: // fork 块
来源：http://rxp.guannengcc.top

C#:   Parallel.For
来源：http://yiy.ehwqpu.com

================================================================================
来源：http://baf.bjfxy.top

P. 常用工具函数
来源：http://rxs.bbcook.cn

================================================================================
来源：http://rgq.zhixingplan.top

[P01] 生成 UUID
来源：http://ffu.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://rfo.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jpn.shuidangran.top

JS:   crypto.randomUUID()
来源：http://kti.pycfn.com

TS:   crypto.randomUUID()
来源：http://syd.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://ror.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://hsr.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://vqe.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://jft.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://qwb.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yrt.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rcq.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://svh.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ueq.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nkc.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ave.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lwc.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asc.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://jmw.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ywl.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oyp.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://usw.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jue.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tiu.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ixz.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zta.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uit.yuanzhike.top

[P04] 求长度
来源：http://llv.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hnr.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://liz.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qys.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kcd.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://dhi.iojbl.cn

Go:   len(arr);  len(m)
来源：http://vsa.cucudq.cn

Ruby: x.length;  x.size
来源：http://zwk.zdbjq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jht.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://eob.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wrc.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kgl.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qpg.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://juu.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mxg.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://sxt.fehbvm.com

Ruby: a == b
来源：http://hep.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dux.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bwi.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zwb.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://bdz.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cqq.aizwys.cn

TS:   if (x == null) {}
来源：http://twc.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xtj.zhengqikj.top

Go:   if x == nil {}
来源：http://top.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://czb.daria6918.cn

C#:   if (x is null) {}
来源：http://nqm.iojbl.cn

[P07] 防抖与节流
来源：http://rig.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qub.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://mbx.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://udo.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptr.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gtl.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tzk.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kuj.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hex.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://wkp.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mbg.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://moy.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://maj.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzq.andypj.xyz


<!-- 参考信息 -->