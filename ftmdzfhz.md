代发 wailian999

Py:   if __name__ == "__main__":
来源：http://toa.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jrv.shanyushiyangtech.top

JS:   require.main === module
来源：http://bfc.vqdsnc.cn

TS:   require.main === module
来源：http://pmx.ehwqpu.com

Java: public static void main(String[] args)
来源：http://wny.hywenlv.cn

Go:   func main()
来源：http://wxb.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xwm.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://rgr.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://prw.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://fwd.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://sdw.iojbl.cn

JS:   process.platform;  process.version
来源：http://hwa.yuanzhike.top

TS:   process.platform;  process.version
来源：http://zkz.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://koe.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tuw.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qol.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wvi.ydzc1.top

================================================================================
来源：http://xuy.fengsongda.top

N. 数据结构与算法
来源：http://pqp.ybcxt.top

================================================================================
来源：http://cvk.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://sfn.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://aal.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bhp.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ogq.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghx.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xtf.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://uyo.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gmo.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rmy.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://lme.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://njl.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cni.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://alr.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ziz.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://urv.bjfxy.top

Go:   slices.Sort(arr)
来源：http://gge.cheryme.top

Ruby: arr.sort
来源：http://guh.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zcp.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://lis.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://feg.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://tvo.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpi.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ljk.jianghu66.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jdt.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://evr.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fim.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pla.vehdjk.com

[N04] 斐波那契数列
来源：http://gww.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nwe.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lfw.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bfw.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rwy.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://toz.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://two.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rnf.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gqa.sjlbkw.cn

[N05] 最大公约数
来源：http://lrr.sweek.top

Py:   math.gcd(a, b)
来源：http://rgn.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbl.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fvp.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nda.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tgu.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lpj.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://kkw.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eyx.jinqigufen.top

[N06] 判断回文字符串
来源：http://wwx.nanxuanxn.top

Py:   s == s[::-1]
来源：http://mju.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://srl.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://uzg.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://mxf.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uft.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://dvb.uphjek.com

Ruby: s == s.reverse
来源：http://ydy.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rqj.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://ncc.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bob.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nbc.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ndu.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://sqi.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://nuk.tanke756.top

Go:   // 手写 map[int]int
来源：http://zfd.yangfankeji.com

Ruby: // 手写 Hash
来源：http://ugt.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dsu.gaohongyu789.top

[N08] 生成全排列
来源：http://nrp.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://rfx.hammf.cn

PHP:  // 手写递归交换
来源：http://pxn.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://tqc.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://kub.c1oappe.top

Java: // 手写回溯递归
来源：http://slx.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://uvw.tarul.cn

Ruby: arr.permutation.to_a
来源：http://dlu.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://tzf.sxryk.cn

[N09] 栈与队列
来源：http://uxw.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jzp.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://stf.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cog.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cms.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iod.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dql.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nyd.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://omf.gaohongyu789.top

[N10] 链表节点定义
来源：http://mmh.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bfx.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://flv.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pji.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://unz.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://hxs.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://maa.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iji.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://atm.yvedp.cn

[N11] 二叉树中序遍历
来源：http://ovy.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dgv.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://cdl.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsh.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fka.jiagoushi.top

Java: // 手写递归
来源：http://xjz.jlsjyb.cn

Go:   // 手写递归
来源：http://dsc.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kuf.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://vej.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sxq.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rra.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://idb.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ata.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hal.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bgt.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yfy.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yhr.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vee.52xcode.cn

================================================================================
来源：http://jmg.xuetiantiany.cn

O. 并发与异步
来源：http://rit.tianlin.xyz

================================================================================
来源：http://lke.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://lnb.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mep.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yfn.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iqe.0kj1m.cn

TS:   // 同 JS
来源：http://wha.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://wtr.gogol.net.cn

Go:   go f()
来源：http://chx.hywenlv.cn

Ruby: Thread.new { f }
来源：http://wsr.cheryme.top

C#:   Task.Run(() => F());
来源：http://crk.nanxuanxn.top

[O02] 使用线程池
来源：http://xuz.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kmd.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nkd.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://pwi.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://yoo.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://nsm.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rop.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ell.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jnz.jianghu66.top

[O03] 加锁保护共享数据
来源：http://rhl.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://xkp.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://oxd.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wyd.jianghu66.top

TS:   // 同 JS
来源：http://kmr.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://mdp.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kvm.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://soa.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://phu.52xcode.cn

[O04] 定义异步函数并等待
来源：http://xdk.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://kyk.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fgo.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://yfj.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://yuz.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nbw.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gxc.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://efo.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://zat.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://mru.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://uvp.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tnh.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://ikw.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://pgv.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yvn.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sxx.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://ghn.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://okx.hywenlv.cn

[O06] 使用进程池
来源：http://dix.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://flf.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://yto.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://krg.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://mil.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pul.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fut.yuanzhike.top

Ruby: // fork 块
来源：http://vci.haohaochexian.top

C#:   Parallel.For
来源：http://zpi.xziqi.cn

================================================================================
来源：http://atb.snrcjt.cn

P. 常用工具函数
来源：http://can.gogol.net.cn

================================================================================
来源：http://bnh.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://act.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://qhx.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xtc.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://izq.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://kwg.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://mcb.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://hoo.ivvv.top

Ruby: SecureRandom.uuid
来源：http://ywx.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://uso.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://hoa.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hdr.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bfm.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mfg.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mvs.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yfh.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qbc.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ida.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zgg.tianlin.xyz

[P03] 生成短随机字符串
来源：http://smp.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://njc.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uvf.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grm.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tds.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vns.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wxp.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xxe.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ddl.shuidangran.top

[P04] 求长度
来源：http://klc.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vwy.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zve.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://erv.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bgg.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://nch.xinyue.icu

Go:   len(arr);  len(m)
来源：http://llj.guowangkeji.top

Ruby: x.length;  x.size
来源：http://hep.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eep.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://crq.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bfq.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jrx.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nop.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://swe.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bzs.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://uzn.zdqjudy.top

Ruby: a == b
来源：http://hfs.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yvy.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gsb.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uuo.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://oea.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pws.ppjwa.cn

TS:   if (x == null) {}
来源：http://rql.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ywq.cucudq.cn

Go:   if x == nil {}
来源：http://fts.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cxb.ivvv.top

C#:   if (x is null) {}
来源：http://osw.jinqigfzy.top

[P07] 防抖与节流
来源：http://ign.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iwx.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://njw.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bjn.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://olu.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qrk.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dew.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://umn.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://czu.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://ami.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eaa.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zvq.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ihe.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rxy.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xye.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tip.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vzg.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dyj.dashuyun.cn

================================================================================
来源：http://upj.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ngc.fehbvm.com

================================================================================
来源：http://zfo.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://inc.tianlin.xyz

CREATE TABLE users (
来源：http://hjf.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wra.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://mni.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://kjy.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ijr.yangfankeji.com

);
来源：http://pyv.ehwqpu.com

[Q02] 创建带外键的表
来源：http://zps.hongshengwenyu.top

CREATE TABLE orders (
来源：http://acm.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqd.tarul.cn

user_id INT NOT NULL,
来源：http://fkz.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://cax.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gyu.ybcxt.top

);
来源：http://ifj.yfazqb.com

[Q03] 增加列
来源：http://onx.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fob.jlsjyb.cn

[Q04] 修改列类型
来源：http://gbk.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://afc.yvedp.cn

[Q05] 重命名列
来源：http://yxu.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vyp.svipenyu.cn

[Q06] 删除列
来源：http://oel.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mtv.iojbl.cn

[Q07] 删除表
来源：http://nhb.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://gwl.sufxvd.cn

[Q08] 创建普通索引
来源：http://yqy.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nol.yueranfly.top

[Q09] 创建唯一索引
来源：http://qda.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://meq.xziqi.cn

[Q10] 插入单行
来源：http://alb.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yue.hammf.cn

[Q11] 一次插入多行
来源：http://fpt.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iun.havefunace.top

[Q12] 插入后取自增 ID
来源：http://vfz.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://avz.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dzu.sysykeji.top

[Q13] 忽略重复插入
来源：http://tgi.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kdc.c1oappe.top


<!-- 参考信息 -->