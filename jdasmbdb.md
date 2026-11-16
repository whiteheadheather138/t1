代发 wailian999

[M04] 获取当前工作目录
来源：http://lug.andypj.xyz

Py:   os.getcwd()
来源：http://tme.daria6918.cn

PHP:  getcwd();
来源：http://kyt.zdqjudy.top

JS:   process.cwd()
来源：http://qjp.yangfankeji.com

TS:   process.cwd()
来源：http://cbq.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://fqa.52xcode.cn

Go:   os.Getwd()
来源：http://tsc.0kj1m.cn

Ruby: Dir.pwd
来源：http://pdj.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://jpq.tanke756.top

[M05] 设置退出码
来源：http://ucs.jqgufenzy.top

Py:   sys.exit(1)
来源：http://klk.bjfxy.top

PHP:  exit(1);
来源：http://roc.cashguo.top

JS:   process.exit(1)
来源：http://wir.fktsv.cn

TS:   process.exit(1)
来源：http://cny.yanxiufei.cn

Java: System.exit(1)
来源：http://for.cqqwz.cn

Go:   os.Exit(1)
来源：http://wjc.fzhhl.top

Ruby: exit 1
来源：http://hkb.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rvt.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://aep.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://jub.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nna.aibaodan.cn

JS:   console.error("err")
来源：http://eii.zhijiandao.cn

TS:   console.error("err")
来源：http://ugm.ydzc1.top

Java: System.err.println("err")
来源：http://qur.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mnh.vqdsnc.cn

Ruby: warn "err"
来源：http://uty.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://eed.yonumen.top

[M07] 判断是否为主入口
来源：http://uhr.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://tsh.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rkl.hesvh.cn

JS:   require.main === module
来源：http://dvm.sjlbkw.cn

TS:   require.main === module
来源：http://uei.mhx1999.top

Java: public static void main(String[] args)
来源：http://yop.jinghuilouyu.cn

Go:   func main()
来源：http://ney.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dbq.gzhubu.top

C#:   static void Main(string[] args)
来源：http://zoo.sweek.top

[M08] 获取系统与运行时信息
来源：http://gkv.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://ozc.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://uoy.cdnleiting.top

JS:   process.platform;  process.version
来源：http://kxj.316326.xyz

TS:   process.platform;  process.version
来源：http://cym.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jrn.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yvx.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ugs.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://szd.sysykeji.top

================================================================================
来源：http://uzp.xuanzx.com

N. 数据结构与算法
来源：http://rli.ywan-chungtsiang.top

================================================================================
来源：http://bxf.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://lbg.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://rch.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://veu.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vqi.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmt.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://ght.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://bna.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jta.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://qxg.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://twu.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://kdz.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rhi.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rkv.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tmt.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kpl.daxiang520.top

Go:   slices.Sort(arr)
来源：http://qna.sufxvd.cn

Ruby: arr.sort
来源：http://sfx.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fxs.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://brq.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdt.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://pqr.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vbm.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmo.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vgh.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tye.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mie.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cco.yonumen.top

[N04] 斐波那契数列
来源：http://vat.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rpx.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iuj.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyf.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ule.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eir.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pro.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ohw.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lhb.ivvv.top

[N05] 最大公约数
来源：http://nlv.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://stc.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdb.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ysy.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xan.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nfh.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://slv.wangdashe.top

Ruby: a.gcd(b)
来源：http://yre.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dcs.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://utq.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://pjs.fktsv.cn

PHP:  $s === strrev($s);
来源：http://uha.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://mad.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://xjf.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rtq.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://psp.wangdashe.top

Ruby: s == s.reverse
来源：http://mfx.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oym.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://pvg.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dpb.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jgh.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mdg.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://wnw.gotoacloud.top

Java: // 手写 HashMap
来源：http://uuy.shuidangran.top

Go:   // 手写 map[int]int
来源：http://erq.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://alv.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://gyh.zhengqikj.top

[N08] 生成全排列
来源：http://nam.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://kde.sysykeji.top

PHP:  // 手写递归交换
来源：http://dgw.aizwys.cn

JS:   // 手写回溯递归
来源：http://qvl.zycfv.cn

TS:   // 手写回溯递归
来源：http://ysw.hywenlv.cn

Java: // 手写回溯递归
来源：http://uhw.gzhubu.top

Go:   // 手写回溯递归
来源：http://qlh.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://gvz.gogol.net.cn

C#:   // 手写回溯递归
来源：http://piv.yonumen.top

[N09] 栈与队列
来源：http://oww.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xxn.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://phf.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://trq.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zcc.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aaa.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tpr.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zir.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lyi.ydzc1.top

[N10] 链表节点定义
来源：http://iam.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ucy.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nrr.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tgu.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gij.yonumen.top

Java: class Node { int v; Node next; }
来源：http://nzo.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://srd.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://afe.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://drr.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://uaw.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wal.c1oappe.top

PHP:  // 手写递归函数
来源：http://yxp.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kka.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqp.cqqwz.cn

Java: // 手写递归
来源：http://wpg.tarul.cn

Go:   // 手写递归
来源：http://ooz.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nyn.epnwcf.com

C#:   // 手写递归
来源：http://czs.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ici.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://grb.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqe.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cja.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jth.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://frh.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dyf.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vyn.ybcxt.top

================================================================================
来源：http://sbu.kuanghao11.cn

O. 并发与异步
来源：http://uui.fehbvm.com

================================================================================
来源：http://xzg.sysykeji.top

[O01] 启动一个线程
来源：http://thy.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qbs.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://edu.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jsf.nanxinkj.top

TS:   // 同 JS
来源：http://asl.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://wns.aizwys.cn

Go:   go f()
来源：http://zra.jyoumei.cn

Ruby: Thread.new { f }
来源：http://fwy.zycfv.cn

C#:   Task.Run(() => F());
来源：http://dzx.dianchejie.cn

[O02] 使用线程池
来源：http://pnq.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sbd.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qhi.zycfv.cn

JS:   // worker_threads 线程池
来源：http://pte.meibo888.top

TS:   // worker_threads 线程池
来源：http://ldy.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://oxh.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mnc.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://arq.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tgk.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://izj.guowangkeji.top

Py:   with lock: shared += 1
来源：http://vyp.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://jft.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gmc.tarul.cn

TS:   // 同 JS
来源：http://ajb.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://ahb.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fdr.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pqv.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://soe.iojbl.cn

[O04] 定义异步函数并等待
来源：http://bcg.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://cur.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gaj.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://tkk.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jue.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fan.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rbg.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://rmi.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://obv.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://xrp.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://eii.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bgo.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://vus.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://usw.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vtf.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nbx.guannengcc.top

Ruby: threads.map(&:join)
来源：http://bmn.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uze.zdqjudy.top

[O06] 使用进程池
来源：http://bdr.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rec.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mwy.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://hka.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://egx.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vtn.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hxm.nwbrower.top

Ruby: // fork 块
来源：http://vpt.gogol.net.cn

C#:   Parallel.For
来源：http://adn.ydzc1.top

================================================================================
来源：http://zlf.yueranfly.top

P. 常用工具函数
来源：http://wjo.andypj.xyz

================================================================================
来源：http://acl.zdbjq.cn

[P01] 生成 UUID
来源：http://wys.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://kyf.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hgv.sysykeji.top

JS:   crypto.randomUUID()
来源：http://qar.cucudq.cn

TS:   crypto.randomUUID()
来源：http://ixj.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://svz.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://osb.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://vvk.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://jat.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://cvf.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mbr.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://czd.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nek.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://smh.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rwc.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dnu.pycfn.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ryo.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://irp.birdmap.top

[P03] 生成短随机字符串
来源：http://qwh.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vmc.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bdq.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gny.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypu.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tip.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kcb.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ukp.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rjc.pycfn.com

[P04] 求长度
来源：http://omg.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wim.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hpp.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zkh.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rfs.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://xol.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://drn.jiagoushi.top

Ruby: x.length;  x.size
来源：http://pji.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cbg.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://uxl.epnwcf.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://wxm.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vha.birdmap.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uwe.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tma.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ecz.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://eph.fengsongda.top

Ruby: a == b
来源：http://evx.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zrx.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lbh.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://usx.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://thh.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tkb.ydjk.org.cn

TS:   if (x == null) {}
来源：http://oyg.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://der.316326.xyz

Go:   if x == nil {}
来源：http://hzq.zhoulong.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wcb.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://ebm.jinqigfzy.top

[P07] 防抖与节流
来源：http://bbo.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ziv.havefunace.top

PHP:  // 手写时间戳比较
来源：http://dpe.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aad.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijp.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ssk.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://box.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jan.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://erl.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://fwh.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://svu.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nty.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oin.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dmz.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bwm.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hea.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bgu.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://guj.yangfankeji.com

================================================================================
来源：http://uoc.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eqm.tarul.cn

================================================================================
来源：http://sbp.yangfankeji.com

[Q01] 创建表
来源：http://sjq.c1oappe.top

CREATE TABLE users (
来源：http://hck.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://knv.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://dwu.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://qjv.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ndx.hfpthk.cn

);
来源：http://itn.shuidangran.top

[Q02] 创建带外键的表
来源：http://nqu.yanxiufei.cn

CREATE TABLE orders (
来源：http://kxc.svipenyu.cn


<!-- 参考信息 -->