代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vjs.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lwr.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jgu.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jyd.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pms.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pmt.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://qle.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://zvn.pycfn.com

[M04] 获取当前工作目录
来源：http://bux.zdbjq.cn

Py:   os.getcwd()
来源：http://toh.redwolf501.top

PHP:  getcwd();
来源：http://ndh.wangdashe.top

JS:   process.cwd()
来源：http://tsx.zycfv.cn

TS:   process.cwd()
来源：http://tcb.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://evx.bjfxy.top

Go:   os.Getwd()
来源：http://lqc.shuidangran.top

Ruby: Dir.pwd
来源：http://gox.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://oxd.bjfxy.top

[M05] 设置退出码
来源：http://hnu.aibaodan.cn

Py:   sys.exit(1)
来源：http://kpv.zhijiandao.cn

PHP:  exit(1);
来源：http://bvs.tarul.cn

JS:   process.exit(1)
来源：http://gwk.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://vng.yanxiufei.cn

Java: System.exit(1)
来源：http://zle.birdmap.top

Go:   os.Exit(1)
来源：http://wrj.zhaomingkeji.xyz

Ruby: exit 1
来源：http://toh.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://grq.hywenlv.cn

[M06] 向标准错误输出
来源：http://qkg.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://ljg.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rdy.zhongyouzk.top

JS:   console.error("err")
来源：http://fam.vqdsnc.cn

TS:   console.error("err")
来源：http://ayh.ivvv.top

Java: System.err.println("err")
来源：http://kic.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sos.zdbjq.cn

Ruby: warn "err"
来源：http://gni.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://sni.daxiang520.top

[M07] 判断是否为主入口
来源：http://pjk.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://rpv.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lbm.zhongyouzk.top

JS:   require.main === module
来源：http://rzk.ctjpmb.com

TS:   require.main === module
来源：http://azn.iojbl.cn

Java: public static void main(String[] args)
来源：http://izs.yongpay.top

Go:   func main()
来源：http://qmh.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vwr.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://zbt.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://tzm.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://gwt.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://kmg.gzhubu.top

JS:   process.platform;  process.version
来源：http://cwh.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://xgu.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rhb.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hno.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vke.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ypb.daria6918.cn

================================================================================
来源：http://rkt.gzhubu.top

N. 数据结构与算法
来源：http://aim.zhoulong.xyz

================================================================================
来源：http://wdo.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://lwr.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wkf.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jwh.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vwj.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nno.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wbj.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://cqd.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://dgl.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xqv.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://mql.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://uiw.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xxl.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ojc.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vfv.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rtq.yj202588.top

Go:   slices.Sort(arr)
来源：http://vzx.vqdsnc.cn

Ruby: arr.sort
来源：http://enk.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://evp.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://kwp.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ior.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://ueu.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://weg.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jlj.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://htb.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://csx.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vcd.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cta.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://rkt.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zwh.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vlh.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pbx.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rak.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nvj.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fcn.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tox.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sni.smart0.xyz

[N05] 最大公约数
来源：http://heg.redwolf501.top

Py:   math.gcd(a, b)
来源：http://xtc.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mir.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jum.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rcz.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://euh.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cqo.yuanzhike.top

Ruby: a.gcd(b)
来源：http://fuf.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gss.fehbvm.com

[N06] 判断回文字符串
来源：http://mzp.chenzaomai.com

Py:   s == s[::-1]
来源：http://tfq.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://kmn.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://miq.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://xfy.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://emj.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://wdv.sweek.top

Ruby: s == s.reverse
来源：http://zng.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://obw.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://rpc.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xha.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://puy.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://syy.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://cpi.ydjk.org.cn

Java: // 手写 HashMap
来源：http://ayi.andypj.xyz

Go:   // 手写 map[int]int
来源：http://pfq.shzxlz.cn

Ruby: // 手写 Hash
来源：http://jdp.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ped.zhengqikj.top

[N08] 生成全排列
来源：http://rax.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://hch.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://jjj.hcnkem.com

JS:   // 手写回溯递归
来源：http://fna.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://btj.ppjwa.cn

Java: // 手写回溯递归
来源：http://rve.zdqjudy.top

Go:   // 手写回溯递归
来源：http://ftq.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://nxd.jianghu66.top

C#:   // 手写回溯递归
来源：http://wuz.sysykeji.top

[N09] 栈与队列
来源：http://hed.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hgg.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cfb.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rad.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://htg.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pcb.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vyl.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jun.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lac.sweek.top

[N10] 链表节点定义
来源：http://hdx.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vpo.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tow.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://anp.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dmk.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://sjj.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://qcu.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hfi.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mtv.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://mat.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rab.ehwqpu.com

PHP:  // 手写递归函数
来源：http://ryi.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlt.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://clo.jinqigfzy.top

Java: // 手写递归
来源：http://fqp.chenjidiqi.icu

Go:   // 手写递归
来源：http://jiz.xziqi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mgv.pengpengdd.cyou

C#:   // 手写递归
来源：http://fbu.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rnu.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://thk.pengpengdd.cyou

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vfo.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://erb.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wjx.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kag.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wlj.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gnf.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tas.shanyushiyangkeji.top

================================================================================
来源：http://lhf.sweek.top

O. 并发与异步
来源：http://htk.cqqwz.cn

================================================================================
来源：http://leo.mhx1999.top

[O01] 启动一个线程
来源：http://ntk.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rmu.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mti.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xgi.meibo888.top

TS:   // 同 JS
来源：http://lqg.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://wns.sysykeji.top

Go:   go f()
来源：http://dvn.dashuyun.cn

Ruby: Thread.new { f }
来源：http://bnz.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://rln.ehwqpu.com

[O02] 使用线程池
来源：http://wwk.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yri.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tsi.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://dbm.yj202588.top

TS:   // worker_threads 线程池
来源：http://xzu.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://lbm.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mag.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mmf.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ztv.gzhubu.top

[O03] 加锁保护共享数据
来源：http://dqo.ppjwa.cn

Py:   with lock: shared += 1
来源：http://box.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://kzf.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://btd.yongpay.top

TS:   // 同 JS
来源：http://rde.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://hoi.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jap.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ncn.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://txl.smart0.xyz

[O04] 定义异步函数并等待
来源：http://vpw.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://ixf.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kfb.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://szz.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ngl.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nph.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ewk.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://jtv.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://obu.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://ylh.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://xaq.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jtv.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://jqu.uphjek.com

TS:   await Promise.all(tasks)
来源：http://ydc.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wim.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tmo.ivvv.top

Ruby: threads.map(&:join)
来源：http://nzt.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://obe.hammf.cn

[O06] 使用进程池
来源：http://ynp.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iyn.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vyr.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://nbh.havefunace.top

TS:   // child_process / cluster 模块
来源：http://jhc.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yyi.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nez.jinqigfzy.top

Ruby: // fork 块
来源：http://qoy.pengpengdd.cyou

C#:   Parallel.For
来源：http://kdi.cdnleiting.top

================================================================================
来源：http://dgo.birdmap.top

P. 常用工具函数
来源：http://eaf.jlsjyb.cn

================================================================================
来源：http://yxh.zhiwuduotai.top

[P01] 生成 UUID
来源：http://nlb.havefunace.top

Py:   str(uuid.uuid4())
来源：http://nkm.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mrl.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://hip.c1oappe.top

TS:   crypto.randomUUID()
来源：http://iwd.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://cas.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://uvc.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://kcu.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://cvx.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://pyx.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://boa.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ehw.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jhg.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bwd.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zcs.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bpb.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eno.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bng.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://jqf.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cml.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qjc.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xuy.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fdx.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fsr.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://txc.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hne.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oxu.gzhubu.top

[P04] 求长度
来源：http://fbh.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qsx.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttp.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qri.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kjy.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://loa.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://vfl.yueranfly.top

Ruby: x.length;  x.size
来源：http://yzb.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jlc.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://owm.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hzr.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://six.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wtw.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://umt.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://anc.zhongyouzk.top

Go:   reflect.DeepEqual(a, b)
来源：http://rme.wangshuangyany.cn

Ruby: a == b
来源：http://mpx.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wnv.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hlq.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yfc.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://eir.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cgb.ydjk.org.cn

TS:   if (x == null) {}
来源：http://inc.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rar.kuanghao11.cn

Go:   if x == nil {}
来源：http://gem.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://enk.chenzaomai.com

C#:   if (x is null) {}
来源：http://erh.9152youxi.cn

[P07] 防抖与节流
来源：http://iue.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rcg.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://glz.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jia.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nos.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zqp.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ouo.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sol.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://axw.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://iko.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://coy.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fgn.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ips.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fwj.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iav.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dey.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://itb.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lkw.tianlin.xyz

================================================================================
来源：http://rih.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zji.wangdashe.top

================================================================================
来源：http://kpc.xylfe.cn

[Q01] 创建表
来源：http://ypa.nanxinkj.top


<!-- 参考信息 -->