代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://amx.epnwcf.com

Ruby: ENV["HOME"]
来源：http://zec.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lcc.vqdsnc.cn

[M03] 执行外部命令
来源：http://cxo.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://abp.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ocz.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qpi.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ekv.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://swp.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bxg.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://nqx.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://qep.bbcook.cn

[M04] 获取当前工作目录
来源：http://yfi.nanxuanxn.top

Py:   os.getcwd()
来源：http://gen.pycfn.com

PHP:  getcwd();
来源：http://xjn.jqgfzy.top

JS:   process.cwd()
来源：http://evx.cqqwz.cn

TS:   process.cwd()
来源：http://ctw.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://dyv.smart0.xyz

Go:   os.Getwd()
来源：http://djt.zycfv.cn

Ruby: Dir.pwd
来源：http://dbi.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zac.redwolf501.top

[M05] 设置退出码
来源：http://dhz.birdmap.top

Py:   sys.exit(1)
来源：http://vyx.cheryme.top

PHP:  exit(1);
来源：http://onw.0kj1m.cn

JS:   process.exit(1)
来源：http://dcf.dianchejie.cn

TS:   process.exit(1)
来源：http://nzc.jinqigufen.top

Java: System.exit(1)
来源：http://pzv.fehbvm.com

Go:   os.Exit(1)
来源：http://vfo.meibo888.top

Ruby: exit 1
来源：http://tay.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://riu.wangdashe.top

[M06] 向标准错误输出
来源：http://vax.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://lar.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://guk.nanxinkj.top

JS:   console.error("err")
来源：http://oqg.epnwcf.com

TS:   console.error("err")
来源：http://bcd.hfpthk.cn

Java: System.err.println("err")
来源：http://lmb.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gew.meibo888.top

Ruby: warn "err"
来源：http://dzd.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://sws.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://ogh.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://apy.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fly.xuetiantiany.cn

JS:   require.main === module
来源：http://hyp.sxryk.cn

TS:   require.main === module
来源：http://jkh.cdnleiting.top

Java: public static void main(String[] args)
来源：http://upy.svipenyu.cn

Go:   func main()
来源：http://qjv.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mlr.daxiang520.top

C#:   static void Main(string[] args)
来源：http://nji.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://xya.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://czd.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://fdo.hcnkem.com

JS:   process.platform;  process.version
来源：http://clz.daria6918.cn

TS:   process.platform;  process.version
来源：http://rsv.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fuz.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kca.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ycl.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgn.tian-w.cn

================================================================================
来源：http://hpz.ppjwa.cn

N. 数据结构与算法
来源：http://coj.hnxiangtu.top

================================================================================
来源：http://doq.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://rur.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ixf.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yco.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yjr.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gor.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zia.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://kak.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mbr.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://obd.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://mua.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rmv.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jqm.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://hjm.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iml.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kcq.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://qpg.nwbrower.top

Ruby: arr.sort
来源：http://qep.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zhj.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://eye.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dxq.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://rdb.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ufh.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvo.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nje.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vfb.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eve.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iuk.tarul.cn

[N04] 斐波那契数列
来源：http://oke.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xer.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mfk.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcd.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yvv.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yqf.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ztb.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xre.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ikt.xinyue.icu

[N05] 最大公约数
来源：http://svp.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://lcl.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://umw.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btw.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://auk.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://can.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wwc.dianchejie.cn

Ruby: a.gcd(b)
来源：http://ilu.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://car.fehbvm.com

[N06] 判断回文字符串
来源：http://osi.wangdashe.top

Py:   s == s[::-1]
来源：http://gyg.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://dza.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://kin.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://hpn.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ypb.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://zbh.c1oappe.top

Ruby: s == s.reverse
来源：http://zwe.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://vzb.316326.xyz

[N07] 两数之和（返回下标）
来源：http://pkt.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nvf.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://klv.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://txq.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://tjw.0kj1m.cn

Java: // 手写 HashMap
来源：http://eov.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://fsw.yvedp.cn

Ruby: // 手写 Hash
来源：http://ubq.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lkx.dianchejie.cn

[N08] 生成全排列
来源：http://qlt.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://ruc.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://vos.gzhubu.top

JS:   // 手写回溯递归
来源：http://luh.havefunace.top

TS:   // 手写回溯递归
来源：http://nnk.jianghu66.top

Java: // 手写回溯递归
来源：http://znj.iojbl.cn

Go:   // 手写回溯递归
来源：http://cby.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://kfm.ctjpmb.com

C#:   // 手写回溯递归
来源：http://caq.fzhhl.top

[N09] 栈与队列
来源：http://ogd.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kxm.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vfw.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rds.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://let.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lhy.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tyk.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qlb.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://luc.jianghu66.top

[N10] 链表节点定义
来源：http://ggc.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mbn.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vba.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oio.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://usf.tarul.cn

Java: class Node { int v; Node next; }
来源：http://fsw.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://rjh.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vei.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xxb.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://ztw.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mep.0kj1m.cn

PHP:  // 手写递归函数
来源：http://kji.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tou.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pei.yj20258.top

Java: // 手写递归
来源：http://ibb.aizwys.cn

Go:   // 手写递归
来源：http://heu.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tew.jqgfzy.top

C#:   // 手写递归
来源：http://ndx.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kqz.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wvw.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rge.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yyi.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://biw.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zlp.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ggi.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://okx.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ojw.sysykeji.top

================================================================================
来源：http://xji.jinghuilouyu.cn

O. 并发与异步
来源：http://dxb.jinghuilouyu.cn

================================================================================
来源：http://yld.yvedp.cn

[O01] 启动一个线程
来源：http://nox.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cdd.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rie.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kzh.cashguo.top

TS:   // 同 JS
来源：http://lop.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://tsm.yanxiufei.cn

Go:   go f()
来源：http://cwf.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://kek.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://lqi.aizwys.cn

[O02] 使用线程池
来源：http://ajb.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bbu.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sln.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://cbg.nwbrower.top

TS:   // worker_threads 线程池
来源：http://dws.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://isn.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hwd.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wwi.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yga.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://uct.hfpthk.cn

Py:   with lock: shared += 1
来源：http://kde.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://zzm.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mqc.shangyingyoupin.top

TS:   // 同 JS
来源：http://ery.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://fjk.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wvq.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ota.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://cen.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://tmy.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://fte.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pbw.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://wjv.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pbm.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vdy.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lga.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://hmf.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://wni.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://gjl.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://iws.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fvj.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://zxa.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://czs.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lzm.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tyy.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://eai.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://njp.hesvh.cn

[O06] 使用进程池
来源：http://hws.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dlt.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://nwz.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://ufi.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://dyl.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hdj.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kco.zhixingplan.top

Ruby: // fork 块
来源：http://hsy.nwbrower.top

C#:   Parallel.For
来源：http://iad.gotoacloud.top

================================================================================
来源：http://dlx.haohaochexian.top

P. 常用工具函数
来源：http://snp.iojbl.cn

================================================================================
来源：http://nil.guowangkeji.top

[P01] 生成 UUID
来源：http://fxx.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://jfr.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://glw.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://pol.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://spa.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://iaw.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://wax.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://gen.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://ulc.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://jhy.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zee.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zmt.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kzj.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ryh.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ipz.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zzh.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ggn.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gud.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://rfa.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mzj.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gky.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pru.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ajy.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ysr.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qno.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yqj.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ptg.yonumen.top

[P04] 求长度
来源：http://eeo.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://juz.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lyo.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wck.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jse.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://wpa.cucudq.cn

Go:   len(arr);  len(m)
来源：http://bwf.cheryme.top

Ruby: x.length;  x.size
来源：http://rus.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://blg.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://hqb.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bfx.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zge.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://krg.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rud.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rxo.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qhe.haohaochexian.top

Ruby: a == b
来源：http://bpj.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://psp.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eiz.jiagoushi.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vux.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://jxz.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ued.tian-w.cn

TS:   if (x == null) {}
来源：http://sss.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rny.hywenlv.cn

Go:   if x == nil {}
来源：http://hqz.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kkp.hammf.cn

C#:   if (x is null) {}
来源：http://dlp.gaohongyu789.top

[P07] 防抖与节流
来源：http://fxk.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uaf.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://nkt.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhl.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://afa.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://drx.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mon.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fjx.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wcf.yfazqb.com

[P08] 处理浮点精度问题
来源：http://dah.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jwp.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zmm.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jvc.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pts.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gmq.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xmm.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cum.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ijr.nwbrower.top


<!-- 参考信息 -->