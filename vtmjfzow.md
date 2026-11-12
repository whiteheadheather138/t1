代发 wailian999

JS:   process.exit(1)
来源：http://rkb.ivvv.top

TS:   process.exit(1)
来源：http://vqc.bbcook.cn

Java: System.exit(1)
来源：http://skh.yj202588.top

Go:   os.Exit(1)
来源：http://uuz.daxiang520.top

Ruby: exit 1
来源：http://rkb.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rxc.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://fef.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://sba.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pek.bjfxy.top

JS:   console.error("err")
来源：http://mzw.redwolf501.top

TS:   console.error("err")
来源：http://cxk.fktsv.cn

Java: System.err.println("err")
来源：http://ngi.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mwv.zhoulong.xyz

Ruby: warn "err"
来源：http://gkv.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://dni.yonumen.top

[M07] 判断是否为主入口
来源：http://ksw.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://pwk.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ajt.epnwcf.com

JS:   require.main === module
来源：http://hks.vqdsnc.cn

TS:   require.main === module
来源：http://ddr.sufxvd.cn

Java: public static void main(String[] args)
来源：http://tis.yj20258.top

Go:   func main()
来源：http://wmj.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ert.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://ldq.316326.xyz

[M08] 获取系统与运行时信息
来源：http://mep.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://mxw.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://fkb.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://ddb.yueranfly.top

TS:   process.platform;  process.version
来源：http://qoj.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tzu.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fbc.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vkp.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://vcg.yvedp.cn

================================================================================
来源：http://oyz.nwbrower.top

N. 数据结构与算法
来源：http://qgi.hywenlv.cn

================================================================================
来源：http://ndn.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://ckh.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://vdk.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://opp.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://umn.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pud.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://kyp.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://wfn.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vdq.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://ogy.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://tva.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://tmm.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tdg.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zog.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vro.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://plj.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://fhl.yuanzhike.top

Ruby: arr.sort
来源：http://qmo.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rfk.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://jfa.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jnt.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://hxu.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ebd.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oav.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zht.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aez.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tqx.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nvw.yj20258888.top

[N04] 斐波那契数列
来源：http://ywy.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iec.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xqe.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wwc.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojf.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yzs.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vys.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wmr.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rba.hnxiangtu.top

[N05] 最大公约数
来源：http://agf.pycfn.com

Py:   math.gcd(a, b)
来源：http://liw.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lgi.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ior.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eae.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ggz.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jyf.ivvv.top

Ruby: a.gcd(b)
来源：http://jki.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kxx.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://agh.cheryme.top

Py:   s == s[::-1]
来源：http://ybj.vehdjk.com

PHP:  $s === strrev($s);
来源：http://moc.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://dzv.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://lel.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mbj.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://ulw.xuanzx.com

Ruby: s == s.reverse
来源：http://xua.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vdb.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://sdq.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pej.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lrk.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ozl.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://hub.c1oappe.top

Java: // 手写 HashMap
来源：http://wca.ivvv.top

Go:   // 手写 map[int]int
来源：http://djm.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://nkj.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://etj.fehbvm.com

[N08] 生成全排列
来源：http://sjy.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://tco.zdbjq.cn

PHP:  // 手写递归交换
来源：http://xvm.52xcode.cn

JS:   // 手写回溯递归
来源：http://phw.fktsv.cn

TS:   // 手写回溯递归
来源：http://tcj.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://zwu.cqqwz.cn

Go:   // 手写回溯递归
来源：http://wpv.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://dfn.pycfn.com

C#:   // 手写回溯递归
来源：http://dzq.ydjk.org.cn

[N09] 栈与队列
来源：http://pvo.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://khk.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vgd.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://htn.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nzl.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yem.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bas.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vlp.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eac.vehdjk.com

[N10] 链表节点定义
来源：http://nnb.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vif.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://avm.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hvh.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://koa.hammf.cn

Java: class Node { int v; Node next; }
来源：http://mya.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://spt.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pdo.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fvq.sweek.top

[N11] 二叉树中序遍历
来源：http://knj.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aqd.jqgfzy.top

PHP:  // 手写递归函数
来源：http://vnd.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbc.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dre.cheryme.top

Java: // 手写递归
来源：http://lkt.aibaodan.cn

Go:   // 手写递归
来源：http://tia.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yfp.sjlbkw.cn

C#:   // 手写递归
来源：http://kfi.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zbh.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zrt.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://upc.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vor.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xda.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ezd.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cor.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pmc.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://skg.bbcook.cn

================================================================================
来源：http://sju.hesvh.cn

O. 并发与异步
来源：http://vgs.birdmap.top

================================================================================
来源：http://qqy.zhijiandao.cn

[O01] 启动一个线程
来源：http://iyv.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aep.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jtt.bbcook.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://egx.tianlin.xyz

TS:   // 同 JS
来源：http://wpa.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://pxv.svipenyu.cn

Go:   go f()
来源：http://mrs.gotoacloud.top

Ruby: Thread.new { f }
来源：http://jlp.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://sum.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://gpz.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bgd.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ncq.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://plo.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://ztj.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://cpp.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pgy.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zzd.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mcq.bbcook.cn

[O03] 加锁保护共享数据
来源：http://ibs.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://qzn.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://its.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fae.pycfn.com

TS:   // 同 JS
来源：http://ynk.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://azb.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://egy.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sww.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://ojc.yvedp.cn

[O04] 定义异步函数并等待
来源：http://qiw.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://uoq.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ctt.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://fpt.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zqd.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xbg.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gli.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://iph.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://hfi.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://jac.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://sqs.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lrs.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://vzc.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://bup.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://skm.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gew.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://kvr.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fds.cqqwz.cn

[O06] 使用进程池
来源：http://jac.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://csc.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kuu.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://lfi.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://tzw.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cib.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oja.fktsv.cn

Ruby: // fork 块
来源：http://ntr.zhoulong.xyz

C#:   Parallel.For
来源：http://qhl.vehdjk.com

================================================================================
来源：http://ivc.jqgfzy.top

P. 常用工具函数
来源：http://cqg.jqgufenzy.top

================================================================================
来源：http://fyp.aizwys.cn

[P01] 生成 UUID
来源：http://yqe.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://nbm.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yrg.cucudq.cn

JS:   crypto.randomUUID()
来源：http://hwt.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://rvn.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://xln.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://yzo.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://nne.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://ocj.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://uth.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ayu.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pxu.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://egd.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tjd.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dih.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://alq.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vxx.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iqx.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://pke.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://emk.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sjv.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ghj.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ntv.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://efx.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pzm.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://olh.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nqd.chenjidiqi.icu

[P04] 求长度
来源：http://hjc.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xwl.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://onn.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bkh.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uze.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://yat.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://kac.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://epi.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nlt.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://uzq.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xdl.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ult.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nyt.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qyy.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uyf.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://kbr.iojbl.cn

Ruby: a == b
来源：http://mwp.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://okl.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vhz.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mbz.yj202588.top

PHP:  if (empty($x)) {}
来源：http://eer.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://avd.sysykeji.top

TS:   if (x == null) {}
来源：http://nmh.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dln.0kj1m.cn

Go:   if x == nil {}
来源：http://qvd.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ubb.quarkkingdee.top

C#:   if (x is null) {}
来源：http://ssv.chenlongwang.top

[P07] 防抖与节流
来源：http://rqy.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oil.316326.xyz

PHP:  // 手写时间戳比较
来源：http://vlr.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xft.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ebd.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xlo.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vxs.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qjq.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dbh.redwolf501.top

[P08] 处理浮点精度问题
来源：http://aho.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xur.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hdw.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tve.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wan.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tti.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pwm.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oyx.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bqv.yj20258888.top

================================================================================
来源：http://zys.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hnk.nwbrower.top

================================================================================
来源：http://vga.yanxiufei.cn

[Q01] 创建表
来源：http://kwx.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://trf.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fng.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://ccq.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://abr.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cfy.yj20258.top

);
来源：http://nsn.sufxvd.cn

[Q02] 创建带外键的表
来源：http://jxj.dashuyun.cn

CREATE TABLE orders (
来源：http://xix.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvb.sxryk.cn

user_id INT NOT NULL,
来源：http://xcz.hnqzz.top

amount DECIMAL(10, 2),
来源：http://vll.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cwg.smart0.xyz

);
来源：http://fyd.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://mig.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xij.ydjk.org.cn

[Q04] 修改列类型
来源：http://zfz.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kdh.daria6918.cn

[Q05] 重命名列
来源：http://gzu.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bkd.jinqigufen.top

[Q06] 删除列
来源：http://bhj.kuanghao11.cn


<!-- 参考信息 -->