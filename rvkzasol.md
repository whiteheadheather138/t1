代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://elg.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vxq.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lvo.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://njf.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yxz.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zkf.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://rwn.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://mws.0kj1m.cn

[M04] 获取当前工作目录
来源：http://iai.52xcode.cn

Py:   os.getcwd()
来源：http://doo.tanke756.top

PHP:  getcwd();
来源：http://jsu.sjlbkw.cn

JS:   process.cwd()
来源：http://uoc.havefunace.top

TS:   process.cwd()
来源：http://qwc.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://lmp.jqgufenzy.top

Go:   os.Getwd()
来源：http://ypb.zdqjudy.top

Ruby: Dir.pwd
来源：http://ntm.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://oun.jlsjyb.cn

[M05] 设置退出码
来源：http://uzk.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://zfn.ybcxt.top

PHP:  exit(1);
来源：http://tan.quarkkingdee.top

JS:   process.exit(1)
来源：http://jbk.chenjidiqi.icu

TS:   process.exit(1)
来源：http://sfb.mhx1999.top

Java: System.exit(1)
来源：http://vft.vehdjk.com

Go:   os.Exit(1)
来源：http://jpn.pengpengdd.cyou

Ruby: exit 1
来源：http://cap.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fap.cheryme.top

[M06] 向标准错误输出
来源：http://jec.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://nqm.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ddy.daxiang520.top

JS:   console.error("err")
来源：http://ide.chenzaomai.com

TS:   console.error("err")
来源：http://tgn.wangdashe.top

Java: System.err.println("err")
来源：http://aiv.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jeu.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://xaa.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://jsa.zdbjq.cn

[M07] 判断是否为主入口
来源：http://bnl.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://eir.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jeo.hnqzz.top

JS:   require.main === module
来源：http://aqs.jqgufenzy.top

TS:   require.main === module
来源：http://upi.gogol.net.cn

Java: public static void main(String[] args)
来源：http://mxv.xinyue.icu

Go:   func main()
来源：http://eyz.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wnw.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://feu.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://rbn.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://iqg.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://lwt.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://cye.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://smh.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xxi.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sjd.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wjw.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zum.dashuyun.cn

================================================================================
来源：http://sea.zhiwuduotai.top

N. 数据结构与算法
来源：http://pbe.smart0.xyz

================================================================================
来源：http://hce.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://icr.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://gbi.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fcw.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://szd.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bwv.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://auf.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://zef.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://som.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xqm.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://ubr.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://blz.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sxr.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hmb.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jhb.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xim.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://hjs.gaohongyu789.top

Ruby: arr.sort
来源：http://jjj.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://osp.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://iua.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cqt.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://qmq.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qso.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vng.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ptp.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bwp.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rvw.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://nmg.chenzaomai.com

[N04] 斐波那契数列
来源：http://kiz.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jzj.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qkz.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozb.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewj.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vba.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qrw.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mns.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mbe.xziqi.cn

[N05] 最大公约数
来源：http://yie.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://ibe.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cbn.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sct.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvr.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymb.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xep.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://fad.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bre.cucudq.cn

[N06] 判断回文字符串
来源：http://pnh.havefunace.top

Py:   s == s[::-1]
来源：http://ykn.316326.xyz

PHP:  $s === strrev($s);
来源：http://jcn.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://hrx.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://hrg.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dto.tanke756.top

Go:   // 双指针从两端比较
来源：http://npn.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://qlc.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ett.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://hfk.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ecy.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vbm.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vpd.sweek.top

TS:   // 手写 Map<string, number>
来源：http://igr.hnqzz.top

Java: // 手写 HashMap
来源：http://cdg.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://hkf.havefunace.top

Ruby: // 手写 Hash
来源：http://onc.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://lzz.jinqigufen.top

[N08] 生成全排列
来源：http://ihw.birdmap.top

Py:   itertools.permutations(arr)
来源：http://oti.uphjek.com

PHP:  // 手写递归交换
来源：http://pgd.gogol.net.cn

JS:   // 手写回溯递归
来源：http://uwl.xylfe.cn

TS:   // 手写回溯递归
来源：http://tju.havefunace.top

Java: // 手写回溯递归
来源：http://jwl.316326.xyz

Go:   // 手写回溯递归
来源：http://ttm.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://kij.tian-w.cn

C#:   // 手写回溯递归
来源：http://geb.zhengqikj.top

[N09] 栈与队列
来源：http://xkt.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cnh.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lky.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hlp.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xlr.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xtf.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tbo.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xvo.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tnr.snrcjt.cn

[N10] 链表节点定义
来源：http://pln.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hal.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://djk.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ycq.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cfw.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://gwc.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://tmq.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bhs.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://exy.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://aex.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ytt.gotoacloud.top

PHP:  // 手写递归函数
来源：http://qzt.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhu.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wus.fanxiaobao.xyz

Java: // 手写递归
来源：http://qlt.yonumen.top

Go:   // 手写递归
来源：http://yha.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ego.ydjk.org.cn

C#:   // 手写递归
来源：http://bxe.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vlx.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pyc.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mep.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugj.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pex.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gzn.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vis.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qmj.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ypa.cqqwz.cn

================================================================================
来源：http://soa.kuanghao11.cn

O. 并发与异步
来源：http://nzw.chenjidiqi.icu

================================================================================
来源：http://yyi.yj20258888.top

[O01] 启动一个线程
来源：http://siu.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pru.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkj.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sby.yj202588.top

TS:   // 同 JS
来源：http://suh.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://wcd.shanyushiyangkeji.top

Go:   go f()
来源：http://gat.smart0.xyz

Ruby: Thread.new { f }
来源：http://bqu.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://qjg.jiagoushi.top

[O02] 使用线程池
来源：http://tte.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sap.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ays.tarul.cn

JS:   // worker_threads 线程池
来源：http://hpd.hammf.cn

TS:   // worker_threads 线程池
来源：http://kra.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://evl.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fip.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bws.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vnc.meibo888.top

[O03] 加锁保护共享数据
来源：http://giu.ybcxt.top

Py:   with lock: shared += 1
来源：http://xeo.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://ldn.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dxh.c1oappe.top

TS:   // 同 JS
来源：http://zfs.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://elf.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kcu.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wrx.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://tia.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://yqk.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://kca.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lsg.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://clv.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qgo.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xqo.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hik.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://stt.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://dyw.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://znr.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://byd.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ndh.yj202588.top

JS:   await Promise.all(tasks)
来源：http://rzg.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://pam.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ivf.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ola.ydzc1.top

Ruby: threads.map(&:join)
来源：http://pyh.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://uio.52xcode.cn

[O06] 使用进程池
来源：http://xoi.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zol.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sad.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://zqz.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://kxm.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pbo.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zje.hammf.cn

Ruby: // fork 块
来源：http://xon.yvedp.cn

C#:   Parallel.For
来源：http://aob.wangshuangyany.cn

================================================================================
来源：http://tcj.cashguo.top

P. 常用工具函数
来源：http://ugk.gotoacloud.top

================================================================================
来源：http://ijn.cucudq.cn

[P01] 生成 UUID
来源：http://ogx.yj20258.top

Py:   str(uuid.uuid4())
来源：http://ild.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ndq.c1oappe.top

JS:   crypto.randomUUID()
来源：http://aus.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://cos.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://fsq.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://zgw.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://zhm.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://wvh.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://hab.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bda.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xwe.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dnk.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qqg.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fxt.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xaq.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dwx.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yrc.sysykeji.top

[P03] 生成短随机字符串
来源：http://cpk.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pww.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lqb.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://npa.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtl.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cvw.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ccq.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://npk.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yfr.chenzaomai.com

[P04] 求长度
来源：http://opr.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xrn.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tcr.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aju.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yub.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://jeq.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://xkp.daria6918.cn

Ruby: x.length;  x.size
来源：http://dwp.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wdi.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://kca.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rba.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mwc.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bdl.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ppk.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://okq.bbcook.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fxs.xingfuxueyuan.xyz

Ruby: a == b
来源：http://cpz.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://otq.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ifs.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://igs.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://gjb.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nwz.ctjpmb.com

TS:   if (x == null) {}
来源：http://hpk.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jqu.hfpthk.cn

Go:   if x == nil {}
来源：http://kag.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pmf.daria6918.cn

C#:   if (x is null) {}
来源：http://fez.hfpthk.cn

[P07] 防抖与节流
来源：http://okk.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sux.316326.xyz

PHP:  // 手写时间戳比较
来源：http://njq.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yec.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hor.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uis.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://neb.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://aku.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gnv.redwolf501.top

[P08] 处理浮点精度问题
来源：http://ryl.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hgn.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qwk.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wva.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hhc.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mud.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wyo.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vyl.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jlh.xuetiantiany.cn

================================================================================
来源：http://wrc.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tpj.smart0.xyz

================================================================================
来源：http://dlx.feifeiyinyue.top

[Q01] 创建表
来源：http://pom.hfpthk.cn


<!-- 参考信息 -->