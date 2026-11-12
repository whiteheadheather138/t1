代发 wailian999

[M04] 获取当前工作目录
来源：http://nir.sjlbkw.cn

Py:   os.getcwd()
来源：http://ejt.tianlin.xyz

PHP:  getcwd();
来源：http://yyo.gaohongyu789.top

JS:   process.cwd()
来源：http://ilm.cdnleiting.top

TS:   process.cwd()
来源：http://lks.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://art.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://owx.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://tei.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://dfb.xylfe.cn

[M05] 设置退出码
来源：http://ejk.ctjpmb.com

Py:   sys.exit(1)
来源：http://jmf.wangdashe.top

PHP:  exit(1);
来源：http://hgw.jiagoushi.top

JS:   process.exit(1)
来源：http://hdp.wangdashe.top

TS:   process.exit(1)
来源：http://jrx.yuxming.cn

Java: System.exit(1)
来源：http://gfs.sjlbkw.cn

Go:   os.Exit(1)
来源：http://uvm.aibaodan.cn

Ruby: exit 1
来源：http://jiz.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wru.yj202588.top

[M06] 向标准错误输出
来源：http://lsc.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://hqe.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vai.tanke756.top

JS:   console.error("err")
来源：http://hxb.shuidangran.top

TS:   console.error("err")
来源：http://kgy.sjlbkw.cn

Java: System.err.println("err")
来源：http://vne.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mhm.xuetiantiany.cn

Ruby: warn "err"
来源：http://yjf.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://trd.52xcode.cn

[M07] 判断是否为主入口
来源：http://nzr.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://zkt.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ikj.bbcook.cn

JS:   require.main === module
来源：http://xhe.xinyue.icu

TS:   require.main === module
来源：http://bpr.hnqzz.top

Java: public static void main(String[] args)
来源：http://qna.snrcjt.cn

Go:   func main()
来源：http://hgg.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jgd.sxryk.cn

C#:   static void Main(string[] args)
来源：http://igt.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://nkw.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://def.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://xua.gzhubu.top

JS:   process.platform;  process.version
来源：http://ood.zdbjq.cn

TS:   process.platform;  process.version
来源：http://reo.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://idg.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pau.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rrf.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xia.yvedp.cn

================================================================================
来源：http://doe.ybcxt.top

N. 数据结构与算法
来源：http://myj.ywan-chungtsiang.top

================================================================================
来源：http://tkb.meibo888.top

[N01] 二分查找（有序数组）
来源：http://mkm.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://bdx.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ogx.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ovn.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwf.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tbo.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://yvh.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ndx.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rzp.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://yhh.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://inz.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://php.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lwh.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ubh.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jgl.nwbrower.top

Go:   slices.Sort(arr)
来源：http://dvv.fktsv.cn

Ruby: arr.sort
来源：http://ydo.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rwq.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://mxe.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ncu.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://mpg.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rmv.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://svu.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bhj.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://con.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fou.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://nxl.jqgufenzy.top

[N04] 斐波那契数列
来源：http://onm.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://erc.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xgb.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ccc.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zvs.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://elf.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wfb.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fpf.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hft.zdbjq.cn

[N05] 最大公约数
来源：http://cck.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://fnt.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vjr.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cid.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byw.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hvv.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qed.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://ume.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wrk.jqgufenzy.top

[N06] 判断回文字符串
来源：http://tib.shuidangran.top

Py:   s == s[::-1]
来源：http://ylf.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://amr.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://kwu.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://swc.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rwl.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://urz.cdnleiting.top

Ruby: s == s.reverse
来源：http://vdb.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qgu.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://qja.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nfj.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lme.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://enf.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://dlv.redwolf501.top

Java: // 手写 HashMap
来源：http://cgj.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://rtg.0kj1m.cn

Ruby: // 手写 Hash
来源：http://bkv.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ifj.aibaodan.cn

[N08] 生成全排列
来源：http://yvb.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://mbo.jinqigufen.top

PHP:  // 手写递归交换
来源：http://rsm.xylfe.cn

JS:   // 手写回溯递归
来源：http://ivk.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://hpu.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://mef.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://zza.hammf.cn

Ruby: arr.permutation.to_a
来源：http://wko.ehwqpu.com

C#:   // 手写回溯递归
来源：http://iev.sufxvd.cn

[N09] 栈与队列
来源：http://myr.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ojp.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pue.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cvi.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gta.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gyh.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zbi.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sch.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xej.guannengcc.top

[N10] 链表节点定义
来源：http://rec.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pke.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dtn.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://crv.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qmo.yonumen.top

Java: class Node { int v; Node next; }
来源：http://krl.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://ilr.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://snh.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://did.wangdashe.top

[N11] 二叉树中序遍历
来源：http://hzw.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://spq.tanke756.top

PHP:  // 手写递归函数
来源：http://cun.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itm.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awk.shangyingyoupin.top

Java: // 手写递归
来源：http://mid.yonumen.top

Go:   // 手写递归
来源：http://wip.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dmv.yangfankeji.com

C#:   // 手写递归
来源：http://hcp.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ybb.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://azu.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eyh.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aua.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cez.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aeu.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vlm.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wfy.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rou.ehwqpu.com

================================================================================
来源：http://xky.shanyushiyangtech.top

O. 并发与异步
来源：http://jbr.quarkkingdee.top

================================================================================
来源：http://ced.yj20258.top

[O01] 启动一个线程
来源：http://yts.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jrr.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wjq.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zfq.xylfe.cn

TS:   // 同 JS
来源：http://vnm.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://wor.yanxiufei.cn

Go:   go f()
来源：http://dif.tianlin.xyz

Ruby: Thread.new { f }
来源：http://rkz.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://ntv.ydjk.org.cn

[O02] 使用线程池
来源：http://krr.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://axk.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://icd.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://qrf.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://zth.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://flp.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pxx.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kfr.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rhd.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://wzy.yonumen.top

Py:   with lock: shared += 1
来源：http://fsy.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ysb.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hcw.hnxiangtu.top

TS:   // 同 JS
来源：http://ecp.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://hsr.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gkg.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://lmz.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://alk.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://hcr.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://emj.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bzk.birdmap.top

JS:   async function f() { await g(); }
来源：http://rsw.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fmt.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nrp.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oya.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://eui.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://hhl.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://fvq.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://snv.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nnw.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://iru.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://xuf.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yfe.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yym.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://pfd.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zdb.vqdsnc.cn

[O06] 使用进程池
来源：http://rfi.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zkd.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kgv.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://kmh.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://glb.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vsd.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ddv.yj20258.top

Ruby: // fork 块
来源：http://jkm.shangyingyoupin.top

C#:   Parallel.For
来源：http://tma.fengsongda.top

================================================================================
来源：http://ksp.9152youxi.cn

P. 常用工具函数
来源：http://mif.shanyushiyangkeji.top

================================================================================
来源：http://eml.sysykeji.top

[P01] 生成 UUID
来源：http://rfs.cashguo.top

Py:   str(uuid.uuid4())
来源：http://nys.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ynw.sweek.top

JS:   crypto.randomUUID()
来源：http://gvn.xziqi.cn

TS:   crypto.randomUUID()
来源：http://gxc.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://spm.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://iuf.meibo888.top

Ruby: SecureRandom.uuid
来源：http://axh.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://yro.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://pwp.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xqj.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jev.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://izn.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fdb.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://umv.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rxe.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ctq.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wvf.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://qjo.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zlt.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wli.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jop.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eto.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://het.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rji.jqgfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzl.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ljr.zhijiandao.cn

[P04] 求长度
来源：http://tjt.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bif.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pck.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iub.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eww.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://wbk.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://kmt.jianghu66.top

Ruby: x.length;  x.size
来源：http://fxw.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://epe.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://yfh.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sgh.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xif.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hbr.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lsq.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eok.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://hij.jqgfzy.top

Ruby: a == b
来源：http://wzy.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tge.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nwj.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bff.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://beb.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://riq.havefunace.top

TS:   if (x == null) {}
来源：http://rjb.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://awp.yj202588.top

Go:   if x == nil {}
来源：http://wco.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xac.guannengcc.top

C#:   if (x is null) {}
来源：http://pol.wangshuangyany.cn

[P07] 防抖与节流
来源：http://pdh.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vig.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://xed.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpz.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbn.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vjc.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qdh.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fsj.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://myj.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://kby.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xix.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ceh.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mdl.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mnm.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gba.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wpz.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ruu.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rjr.havefunace.top

================================================================================
来源：http://rpp.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tns.uphjek.com

================================================================================
来源：http://qkd.redwolf501.top

[Q01] 创建表
来源：http://uuu.xuanzx.com

CREATE TABLE users (
来源：http://izw.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://new.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://mvz.ydjk.org.cn

email VARCHAR(100) UNIQUE,
来源：http://itj.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvn.cheryme.top

);
来源：http://ysc.iojbl.cn

[Q02] 创建带外键的表
来源：http://tml.cheryme.top

CREATE TABLE orders (
来源：http://cil.sufxvd.cn


<!-- 参考信息 -->