代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vqc.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blj.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lbv.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vkx.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qsn.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gey.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ajo.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://dtb.uphjek.com

[M04] 获取当前工作目录
来源：http://oux.jyoumei.cn

Py:   os.getcwd()
来源：http://ejn.zhiwuduotai.top

PHP:  getcwd();
来源：http://cby.yonumen.top

JS:   process.cwd()
来源：http://flj.316326.xyz

TS:   process.cwd()
来源：http://xsr.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://wvc.jianghu66.top

Go:   os.Getwd()
来源：http://uhj.yuanzhike.top

Ruby: Dir.pwd
来源：http://gpf.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://whf.yonumen.top

[M05] 设置退出码
来源：http://rcu.kuanghao11.cn

Py:   sys.exit(1)
来源：http://bni.svipenyu.cn

PHP:  exit(1);
来源：http://bhz.shzxlz.cn

JS:   process.exit(1)
来源：http://gsj.cucudq.cn

TS:   process.exit(1)
来源：http://hvg.nanxinkj.top

Java: System.exit(1)
来源：http://zbf.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://bcy.tarul.cn

Ruby: exit 1
来源：http://ove.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qti.ppjwa.cn

[M06] 向标准错误输出
来源：http://vmf.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://ujs.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zmq.ppjwa.cn

JS:   console.error("err")
来源：http://vzr.mhx1999.top

TS:   console.error("err")
来源：http://kjl.birdmap.top

Java: System.err.println("err")
来源：http://ljw.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nvt.fktsv.cn

Ruby: warn "err"
来源：http://iyv.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://sau.jianghu66.top

[M07] 判断是否为主入口
来源：http://sly.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://nzs.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pnh.yvedp.cn

JS:   require.main === module
来源：http://rzh.birdmap.top

TS:   require.main === module
来源：http://yqa.316326.xyz

Java: public static void main(String[] args)
来源：http://cwr.jianghu66.top

Go:   func main()
来源：http://ere.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qee.zycfv.cn

C#:   static void Main(string[] args)
来源：http://prh.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://psh.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://vgp.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://enr.sufxvd.cn

JS:   process.platform;  process.version
来源：http://lbs.hcnkem.com

TS:   process.platform;  process.version
来源：http://wam.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uzr.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://lzx.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mmz.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jsp.xuanzx.com

================================================================================
来源：http://syz.ydjk.org.cn

N. 数据结构与算法
来源：http://sqk.yj202588.top

================================================================================
来源：http://frv.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://qjz.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://swg.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gzc.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://foy.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yfz.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://tak.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://jem.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uud.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lzj.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://csq.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://wgw.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zzr.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yiu.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uhm.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zvk.316326.xyz

Go:   slices.Sort(arr)
来源：http://xvn.fktsv.cn

Ruby: arr.sort
来源：http://wxb.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mga.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://oao.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rjh.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://aih.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gzt.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mgt.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gsq.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lgf.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xab.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://nku.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://dbi.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bbz.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ysn.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhf.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eys.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://drb.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zsf.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://siy.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gnf.haohaochexian.top

[N05] 最大公约数
来源：http://krw.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://gva.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iye.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvl.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tzz.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kdc.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xhx.snrcjt.cn

Ruby: a.gcd(b)
来源：http://sey.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://caa.gotoacloud.top

[N06] 判断回文字符串
来源：http://jjp.hnxiangtu.top

Py:   s == s[::-1]
来源：http://frr.fktsv.cn

PHP:  $s === strrev($s);
来源：http://mnj.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://ztb.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://ndr.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xjl.ybcxt.top

Go:   // 双指针从两端比较
来源：http://ivi.9152youxi.cn

Ruby: s == s.reverse
来源：http://rly.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://xck.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://tyu.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mwz.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xkl.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qds.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://bek.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://akm.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://dwy.wangdashe.top

Ruby: // 手写 Hash
来源：http://ckg.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://weh.gogol.net.cn

[N08] 生成全排列
来源：http://xrk.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://zwt.nanxinkj.top

PHP:  // 手写递归交换
来源：http://fau.ppjwa.cn

JS:   // 手写回溯递归
来源：http://esm.xziqi.cn

TS:   // 手写回溯递归
来源：http://esp.yanxiufei.cn

Java: // 手写回溯递归
来源：http://axl.yvedp.cn

Go:   // 手写回溯递归
来源：http://sen.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://sil.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://cxs.gzhubu.top

[N09] 栈与队列
来源：http://ljp.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://amy.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://etd.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wlh.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://egr.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hyo.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jmz.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lmg.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://erd.jqgufenzy.top

[N10] 链表节点定义
来源：http://grf.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vnq.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fxn.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jmw.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://raf.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://mkv.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://dco.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dzr.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ldk.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://cjf.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gvu.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://hoy.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ehk.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qlr.xuanzx.com

Java: // 手写递归
来源：http://afp.gzhubu.top

Go:   // 手写递归
来源：http://mpe.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jry.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://otb.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kud.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hpp.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jmu.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qci.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://heq.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cry.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pgg.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zuf.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ngd.snrcjt.cn

================================================================================
来源：http://krc.smart0.xyz

O. 并发与异步
来源：http://ket.yj202588.top

================================================================================
来源：http://hvn.hcnkem.com

[O01] 启动一个线程
来源：http://apo.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xaq.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nvm.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tyl.cashguo.top

TS:   // 同 JS
来源：http://fnj.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://ntw.havefunace.top

Go:   go f()
来源：http://rel.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://iwu.xylfe.cn

C#:   Task.Run(() => F());
来源：http://avn.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://uhl.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dsr.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wyp.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://nmo.sysykeji.top

TS:   // worker_threads 线程池
来源：http://zqp.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://biz.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cft.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jlv.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://utz.jianghu66.top

[O03] 加锁保护共享数据
来源：http://ymo.nwbrower.top

Py:   with lock: shared += 1
来源：http://hit.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://csj.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://znb.jqgufenzy.top

TS:   // 同 JS
来源：http://meq.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://bsq.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ckp.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://cvc.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://wre.yj202588.top

[O04] 定义异步函数并等待
来源：http://kwm.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://akt.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ook.epnwcf.com

JS:   async function f() { await g(); }
来源：http://lak.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://anv.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nmb.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://prh.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://wqe.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://cuk.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://elu.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://yah.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tuc.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://gmz.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://izc.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpr.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rgx.andypj.xyz

Ruby: threads.map(&:join)
来源：http://ydn.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nfj.smart0.xyz

[O06] 使用进程池
来源：http://jsh.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vyf.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://uka.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://ntm.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://eco.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pxw.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mwu.jqgfzy.top

Ruby: // fork 块
来源：http://ytf.hfpthk.cn

C#:   Parallel.For
来源：http://lex.jlsjyb.cn

================================================================================
来源：http://hgk.zhengqikj.top

P. 常用工具函数
来源：http://oqd.52xcode.cn

================================================================================
来源：http://gob.shangyingyoupin.top

[P01] 生成 UUID
来源：http://lub.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://vxp.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ake.sysykeji.top

JS:   crypto.randomUUID()
来源：http://hgm.hcnkem.com

TS:   crypto.randomUUID()
来源：http://pht.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://paw.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://ohl.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://gmk.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://khj.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://sjq.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dly.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oqt.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ljq.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ayy.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pkc.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ajh.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lhq.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zcb.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://qak.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rfs.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://omi.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sme.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uma.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qol.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rgq.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nvx.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pvf.ywan-chungtsiang.top

[P04] 求长度
来源：http://uhk.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qjx.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rzu.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfs.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzh.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://plr.cucudq.cn

Go:   len(arr);  len(m)
来源：http://qxj.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://vwq.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jjd.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://hvd.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qzm.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://soz.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qok.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzm.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rmb.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://vsq.sjlbkw.cn

Ruby: a == b
来源：http://iil.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vtl.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jbz.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pbi.hammf.cn

PHP:  if (empty($x)) {}
来源：http://nxd.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://frn.zhijiandao.cn

TS:   if (x == null) {}
来源：http://qqy.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mym.quarkkingdee.top

Go:   if x == nil {}
来源：http://oep.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nzb.dianchejie.cn

C#:   if (x is null) {}
来源：http://zrd.wangdashe.top

[P07] 防抖与节流
来源：http://apc.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mge.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://pzq.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://all.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqb.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fgf.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qmn.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zdz.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tsd.tarul.cn

[P08] 处理浮点精度问题
来源：http://yjv.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eqq.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ebn.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://msb.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ksq.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cpx.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://odm.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jsq.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qer.hongshengwenyu.top

================================================================================
来源：http://xht.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dot.gogol.net.cn

================================================================================
来源：http://jga.aizwys.cn

[Q01] 创建表
来源：http://fzf.yongpay.top


<!-- 参考信息 -->