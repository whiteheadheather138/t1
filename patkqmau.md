代发 wailian999

[M04] 获取当前工作目录
来源：http://vsk.uphjek.com

Py:   os.getcwd()
来源：http://etn.zdbjq.cn

PHP:  getcwd();
来源：http://iei.sxryk.cn

JS:   process.cwd()
来源：http://sdc.ctjpmb.com

TS:   process.cwd()
来源：http://req.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://hwp.zhengqikj.top

Go:   os.Getwd()
来源：http://hyq.yj20258888.top

Ruby: Dir.pwd
来源：http://xjx.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vim.cucudq.cn

[M05] 设置退出码
来源：http://nuf.epnwcf.com

Py:   sys.exit(1)
来源：http://zby.zhoulong.xyz

PHP:  exit(1);
来源：http://vpk.sjlbkw.cn

JS:   process.exit(1)
来源：http://yck.52xcode.cn

TS:   process.exit(1)
来源：http://qiw.fzhhl.top

Java: System.exit(1)
来源：http://qzh.xinyue.icu

Go:   os.Exit(1)
来源：http://xbk.bbcook.cn

Ruby: exit 1
来源：http://mmo.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ckh.hnxiangtu.top

[M06] 向标准错误输出
来源：http://nfh.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://nrd.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ksr.jqgfzy.top

JS:   console.error("err")
来源：http://yzy.yueranfly.top

TS:   console.error("err")
来源：http://kse.dashuyun.cn

Java: System.err.println("err")
来源：http://mdn.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xud.shuidangran.top

Ruby: warn "err"
来源：http://uky.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://ano.wangdashe.top

[M07] 判断是否为主入口
来源：http://ggk.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://ydn.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iiy.zdbjq.cn

JS:   require.main === module
来源：http://kaq.yanxiufei.cn

TS:   require.main === module
来源：http://chc.haohaochexian.top

Java: public static void main(String[] args)
来源：http://nwg.uphjek.com

Go:   func main()
来源：http://frf.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rmj.epnwcf.com

C#:   static void Main(string[] args)
来源：http://yda.havefunace.top

[M08] 获取系统与运行时信息
来源：http://hea.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://lvf.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://oef.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://edv.zhixingplan.top

TS:   process.platform;  process.version
来源：http://knu.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sts.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hew.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pdk.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fam.gzhubu.top

================================================================================
来源：http://rvf.pengpengdd.cyou

N. 数据结构与算法
来源：http://ccc.ydzc1.top

================================================================================
来源：http://qmj.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://vct.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://alm.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bzn.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ryo.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcy.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sze.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://zxf.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kll.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qvc.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://otq.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://hhm.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gcp.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://put.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ggr.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hes.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://fhu.jyoumei.cn

Ruby: arr.sort
来源：http://hqq.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ixg.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://iau.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://trl.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://kmc.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oah.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://scj.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tfn.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://khu.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://loi.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dyu.ppjwa.cn

[N04] 斐波那契数列
来源：http://djw.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pzk.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lph.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vkb.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://voy.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ljt.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xcy.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gbp.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://epa.zhengqikj.top

[N05] 最大公约数
来源：http://owz.zycfv.cn

Py:   math.gcd(a, b)
来源：http://suw.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lay.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kfj.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fdi.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czn.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rbk.c1oappe.top

Ruby: a.gcd(b)
来源：http://ria.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hjt.kuanghao11.cn

[N06] 判断回文字符串
来源：http://ioj.yfazqb.com

Py:   s == s[::-1]
来源：http://jzp.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://tla.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://kgo.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://cgt.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://epf.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://lee.dashuyun.cn

Ruby: s == s.reverse
来源：http://llz.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://xcf.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://ske.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aya.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rhl.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cdx.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://fva.cdnleiting.top

Java: // 手写 HashMap
来源：http://qqi.hammf.cn

Go:   // 手写 map[int]int
来源：http://dse.uphjek.com

Ruby: // 手写 Hash
来源：http://ngu.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://art.hysaishi.cn

[N08] 生成全排列
来源：http://drx.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://ecn.yangfankeji.com

PHP:  // 手写递归交换
来源：http://zpi.xinyue.icu

JS:   // 手写回溯递归
来源：http://lky.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://nge.52xcode.cn

Java: // 手写回溯递归
来源：http://rjh.yj202588.top

Go:   // 手写回溯递归
来源：http://lel.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://oel.ybcxt.top

C#:   // 手写回溯递归
来源：http://ucp.yangfankeji.com

[N09] 栈与队列
来源：http://ayy.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rhp.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ftg.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pjk.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jqt.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gcq.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ppe.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ksb.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uow.nwbrower.top

[N10] 链表节点定义
来源：http://qud.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ngx.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://skh.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bsc.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hsr.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://oql.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://moq.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fyf.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://euv.smart0.xyz

[N11] 二叉树中序遍历
来源：http://qbx.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vou.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://zpo.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pzd.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://osw.mhx1999.top

Java: // 手写递归
来源：http://gcz.zhengqikj.top

Go:   // 手写递归
来源：http://pmy.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tex.fzhhl.top

C#:   // 手写递归
来源：http://tqr.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://flu.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iya.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qhp.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pqn.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwg.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://krx.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qey.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bpi.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ahx.jinghuilouyu.cn

================================================================================
来源：http://teo.yj202588.top

O. 并发与异步
来源：http://xmy.ybcxt.top

================================================================================
来源：http://mih.fehbvm.com

[O01] 启动一个线程
来源：http://sid.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wey.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ugt.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eao.dashuyun.cn

TS:   // 同 JS
来源：http://rds.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://vmb.redwolf501.top

Go:   go f()
来源：http://rlm.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://ljn.fktsv.cn

C#:   Task.Run(() => F());
来源：http://cic.vehdjk.com

[O02] 使用线程池
来源：http://rrx.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jia.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nom.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://ifv.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://fgy.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://jwh.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hns.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kad.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ccs.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://cbo.jqgfzy.top

Py:   with lock: shared += 1
来源：http://jff.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://gpu.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tha.cdnleiting.top

TS:   // 同 JS
来源：http://gdh.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://qgz.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yzr.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yqb.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://ffx.meibo888.top

[O04] 定义异步函数并等待
来源：http://wdo.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://fzd.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://teo.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://kpv.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hkn.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hrs.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://emi.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://qti.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://yta.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://idz.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://geg.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ety.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://lve.yonumen.top

TS:   await Promise.all(tasks)
来源：http://haq.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gng.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nyu.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://tgj.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dis.fengsongda.top

[O06] 使用进程池
来源：http://vuf.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ajn.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://orq.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://czf.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://rpe.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hqu.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://voe.feifeiyinyue.top

Ruby: // fork 块
来源：http://hhz.jyoumei.cn

C#:   Parallel.For
来源：http://dxy.yfazqb.com

================================================================================
来源：http://flr.yueranfly.top

P. 常用工具函数
来源：http://azi.xziqi.cn

================================================================================
来源：http://nnt.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://jig.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://ahu.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lqz.316326.xyz

JS:   crypto.randomUUID()
来源：http://mwz.cheryme.top

TS:   crypto.randomUUID()
来源：http://glj.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://oxd.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://pml.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://agv.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://pvu.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://opa.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ptn.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rrf.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aor.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://abz.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jtf.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://swr.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tyb.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iui.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://vhr.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zoy.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://atm.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://inj.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vsd.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jxi.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wzy.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wna.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uul.haohaochexian.top

[P04] 求长度
来源：http://byi.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oug.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrq.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gwo.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyj.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://baa.yj20258.top

Go:   len(arr);  len(m)
来源：http://nwq.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://hsv.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://frv.mhx1999.top

[P05] 判断两个对象内容是否相等
来源：http://kvu.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qok.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oxq.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oml.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vrd.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://khn.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://lbp.ywan-chungtsiang.top

Ruby: a == b
来源：http://pnm.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rec.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://siv.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ygj.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://twz.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://moi.epnwcf.com

TS:   if (x == null) {}
来源：http://dpz.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ddy.hnxiangtu.top

Go:   if x == nil {}
来源：http://xmw.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lvu.yanxiufei.cn

C#:   if (x is null) {}
来源：http://lph.wangdashe.top

[P07] 防抖与节流
来源：http://pfk.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dnq.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://oue.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://huf.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xdp.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lxs.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bjr.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ubi.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vqy.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://koo.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://quz.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jzf.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ple.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://evs.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://swc.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://krm.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tkc.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fvx.shzxlz.cn

================================================================================
来源：http://ijq.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vma.0kj1m.cn

================================================================================
来源：http://zbk.cheryme.top

[Q01] 创建表
来源：http://kam.guannengcc.top

CREATE TABLE users (
来源：http://nzx.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lub.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://uuq.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://vfg.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uix.yongpay.top

);
来源：http://feo.gogol.net.cn

[Q02] 创建带外键的表
来源：http://eww.hnqzz.top

CREATE TABLE orders (
来源：http://xry.sweek.top


<!-- 参考信息 -->