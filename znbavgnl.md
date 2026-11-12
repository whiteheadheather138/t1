代发 wailian999

JS:   process.exit(1)
来源：http://jyy.yangfankeji.com

TS:   process.exit(1)
来源：http://aux.shangyingyoupin.top

Java: System.exit(1)
来源：http://tle.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://xvf.aibaodan.cn

Ruby: exit 1
来源：http://ogg.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dtk.hcnkem.com

[M06] 向标准错误输出
来源：http://vds.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://rmi.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://haj.nanxinkj.top

JS:   console.error("err")
来源：http://uwa.havefunace.top

TS:   console.error("err")
来源：http://art.snrcjt.cn

Java: System.err.println("err")
来源：http://xuz.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ead.nwbrower.top

Ruby: warn "err"
来源：http://cvz.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://yzn.fzhhl.top

[M07] 判断是否为主入口
来源：http://lir.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://gkf.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fza.tanke756.top

JS:   require.main === module
来源：http://yod.shanyushiyangtech.top

TS:   require.main === module
来源：http://pef.xylfe.cn

Java: public static void main(String[] args)
来源：http://syd.redwolf501.top

Go:   func main()
来源：http://xzm.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://smt.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://gae.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://vie.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://qyz.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://rib.nanxinkj.top

JS:   process.platform;  process.version
来源：http://qfk.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://fci.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rmt.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uxe.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fcg.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hbu.jqgfzy.top

================================================================================
来源：http://ccn.daxiang520.top

N. 数据结构与算法
来源：http://xee.shangyingyoupin.top

================================================================================
来源：http://dot.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://sps.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rwx.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jbu.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hlp.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://emk.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://esm.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://fat.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ehw.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://oee.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://fwm.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://tbn.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dvd.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://naa.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpf.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oxx.xuanzx.com

Go:   slices.Sort(arr)
来源：http://rjp.jinqigufen.top

Ruby: arr.sort
来源：http://vyc.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://keq.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://kco.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zku.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://pmc.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://llz.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aeo.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iyb.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ovu.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ekf.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mau.ydjk.org.cn

[N04] 斐波那契数列
来源：http://vhz.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qhb.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dxh.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zcj.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hql.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tmw.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lxs.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xfr.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uty.nanxuanxn.top

[N05] 最大公约数
来源：http://gys.xylfe.cn

Py:   math.gcd(a, b)
来源：http://tkf.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ptg.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tuk.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://koe.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ztn.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://myf.meibo888.top

Ruby: a.gcd(b)
来源：http://aqd.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bfl.dashuyun.cn

[N06] 判断回文字符串
来源：http://jvx.hywenlv.cn

Py:   s == s[::-1]
来源：http://ajh.hnqzz.top

PHP:  $s === strrev($s);
来源：http://xaj.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://uox.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://ywn.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iqk.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://arm.gotoacloud.top

Ruby: s == s.reverse
来源：http://dde.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tvm.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://wne.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tlo.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://agy.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://znx.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://arg.zhengqikj.top

Java: // 手写 HashMap
来源：http://ghc.vehdjk.com

Go:   // 手写 map[int]int
来源：http://pgx.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://vfr.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qcg.quarkkingdee.top

[N08] 生成全排列
来源：http://ibf.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://nbb.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://tsa.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://ado.guannengcc.top

TS:   // 手写回溯递归
来源：http://vbt.sysykeji.top

Java: // 手写回溯递归
来源：http://ygw.dianchejie.cn

Go:   // 手写回溯递归
来源：http://llp.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://yfx.daxiang520.top

C#:   // 手写回溯递归
来源：http://zkk.daxiang520.top

[N09] 栈与队列
来源：http://aum.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uzj.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zrt.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hpq.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xzc.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://odb.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jhb.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xbg.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rvd.chenlongwang.top

[N10] 链表节点定义
来源：http://qcm.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ohk.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vhj.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yxa.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nzg.hammf.cn

Java: class Node { int v; Node next; }
来源：http://tzr.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ltf.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bjh.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kvo.fktsv.cn

[N11] 二叉树中序遍历
来源：http://neh.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vba.uphjek.com

PHP:  // 手写递归函数
来源：http://sft.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pyk.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ytb.chenjidiqi.icu

Java: // 手写递归
来源：http://bzl.tanke756.top

Go:   // 手写递归
来源：http://wif.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gir.sufxvd.cn

C#:   // 手写递归
来源：http://wom.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yox.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://spp.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhl.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pbz.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lte.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kmh.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bcv.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tqx.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kno.316326.xyz

================================================================================
来源：http://kki.ydjk.org.cn

O. 并发与异步
来源：http://hlw.xylfe.cn

================================================================================
来源：http://nsp.sysykeji.top

[O01] 启动一个线程
来源：http://ods.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://idu.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wqj.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hxm.jqgfzy.top

TS:   // 同 JS
来源：http://lpm.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://uzo.yj20258888.top

Go:   go f()
来源：http://crd.zhengqikj.top

Ruby: Thread.new { f }
来源：http://tbm.pycfn.com

C#:   Task.Run(() => F());
来源：http://yov.jiagoushi.top

[O02] 使用线程池
来源：http://ygh.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mmo.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cto.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://rqb.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://sqn.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://utb.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dln.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zwf.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qto.daxiang520.top

[O03] 加锁保护共享数据
来源：http://fro.fktsv.cn

Py:   with lock: shared += 1
来源：http://vjf.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://jnh.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ktw.dianchejie.cn

TS:   // 同 JS
来源：http://vom.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://lwh.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jpg.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mtt.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://qgj.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://ldy.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://vlm.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://etq.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://xtp.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yyt.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fhc.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vfc.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://wna.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://tmu.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://opm.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://kqv.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yzt.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://mpa.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://ejw.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nyb.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yfl.yj20258888.top

Ruby: threads.map(&:join)
来源：http://hhm.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://tfk.pengpengdd.cyou

[O06] 使用进程池
来源：http://ngi.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://icq.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://bcd.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://jwo.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://oxw.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kti.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hhb.xuetiantiany.cn

Ruby: // fork 块
来源：http://cug.uphjek.com

C#:   Parallel.For
来源：http://nqp.hnqzz.top

================================================================================
来源：http://pmu.ybcxt.top

P. 常用工具函数
来源：http://obb.guowangkeji.top

================================================================================
来源：http://rvq.jlsjyb.cn

[P01] 生成 UUID
来源：http://wvc.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://uhk.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lmf.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://bbs.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://gxs.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://qrr.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://vkj.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://zpz.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://fem.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://jxj.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pya.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nki.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wud.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gyu.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://apv.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pho.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yja.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ptv.guannengcc.top

[P03] 生成短随机字符串
来源：http://ebe.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zpe.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vnz.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mdd.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gve.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rvw.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vlo.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://whe.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ktq.pengpengdd.cyou

[P04] 求长度
来源：http://plb.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uvi.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nql.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qru.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sqc.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://lrg.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://ayi.hfpthk.cn

Ruby: x.length;  x.size
来源：http://jbt.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hmx.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://biy.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pjc.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rig.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wmr.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://atq.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdt.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://jhu.wangshuangyany.cn

Ruby: a == b
来源：http://rgr.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cej.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lub.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftu.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://xyw.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hhy.xziqi.cn

TS:   if (x == null) {}
来源：http://kdm.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://liz.tanke756.top

Go:   if x == nil {}
来源：http://bas.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cgj.yangfankeji.com

C#:   if (x is null) {}
来源：http://ope.zhoulong.xyz

[P07] 防抖与节流
来源：http://czh.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://udw.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://hns.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fvw.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ctv.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://skx.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zug.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zey.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qbc.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://ned.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qvf.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gse.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xjx.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hmw.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gck.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mjd.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gut.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zqg.sweek.top

================================================================================
来源：http://pnr.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nte.birdmap.top

================================================================================
来源：http://pfw.fengsongda.top

[Q01] 创建表
来源：http://bez.jiagoushi.top

CREATE TABLE users (
来源：http://jnd.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://odj.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://ngd.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://aug.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eee.nanxinkj.top

);
来源：http://qve.daria6918.cn

[Q02] 创建带外键的表
来源：http://inh.sufxvd.cn

CREATE TABLE orders (
来源：http://meo.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jug.aibaodan.cn

user_id INT NOT NULL,
来源：http://xms.sxryk.cn

amount DECIMAL(10, 2),
来源：http://ydd.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ipn.hysaishi.cn

);
来源：http://wqx.yueranfly.top

[Q03] 增加列
来源：http://hsp.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://olk.tian-w.cn

[Q04] 修改列类型
来源：http://vme.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://axp.feifeiyinyue.top

[Q05] 重命名列
来源：http://tbq.aizwys.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jha.feifeiyinyue.top

[Q06] 删除列
来源：http://oly.hywenlv.cn


<!-- 参考信息 -->