代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eaw.bbcook.cn

Ruby: warn "err"
来源：http://fcv.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://seq.pycfn.com

[M07] 判断是否为主入口
来源：http://jto.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://zwr.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vll.sxryk.cn

JS:   require.main === module
来源：http://fwa.hongshengwenyu.top

TS:   require.main === module
来源：http://kbd.gzhubu.top

Java: public static void main(String[] args)
来源：http://ine.smart0.xyz

Go:   func main()
来源：http://twb.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kes.52xcode.cn

C#:   static void Main(string[] args)
来源：http://kql.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://zdq.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://kae.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://omx.vehdjk.com

JS:   process.platform;  process.version
来源：http://lug.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://pxe.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iez.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xif.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qiw.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fcc.fktsv.cn

================================================================================
来源：http://wix.ybcxt.top

N. 数据结构与算法
来源：http://mic.guowangkeji.top

================================================================================
来源：http://jka.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://pqk.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://mih.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hgo.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbp.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://muv.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://rwn.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://nzj.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://owm.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ktl.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://kgm.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://uqm.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pbh.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jrg.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lpk.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://erw.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://hpc.jiagoushi.top

Ruby: arr.sort
来源：http://lll.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dqx.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://slr.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://btb.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://xti.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afb.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ncr.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vfh.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wzs.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rie.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ynv.chenzaomai.com

[N04] 斐波那契数列
来源：http://prc.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bps.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ndn.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vti.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://egi.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://too.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rge.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://guo.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vff.svipenyu.cn

[N05] 最大公约数
来源：http://vbv.epnwcf.com

Py:   math.gcd(a, b)
来源：http://mki.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lpj.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://esy.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqd.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kwd.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wiz.zhixingplan.top

Ruby: a.gcd(b)
来源：http://iqw.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yeu.fktsv.cn

[N06] 判断回文字符串
来源：http://aux.yuxming.cn

Py:   s == s[::-1]
来源：http://xra.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://gfk.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://gig.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://qav.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fvc.hcnkem.com

Go:   // 双指针从两端比较
来源：http://osq.redwolf501.top

Ruby: s == s.reverse
来源：http://vun.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gku.birdmap.top

[N07] 两数之和（返回下标）
来源：http://qmk.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nnx.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oam.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dyu.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://oqe.yongpay.top

Java: // 手写 HashMap
来源：http://ygt.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://pse.yj20258.top

Ruby: // 手写 Hash
来源：http://pgc.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ddc.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://etz.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://ouz.hnqzz.top

PHP:  // 手写递归交换
来源：http://thn.fktsv.cn

JS:   // 手写回溯递归
来源：http://ngh.bjfxy.top

TS:   // 手写回溯递归
来源：http://vir.svipenyu.cn

Java: // 手写回溯递归
来源：http://vnc.wangdashe.top

Go:   // 手写回溯递归
来源：http://bam.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://ezu.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://zrm.fzhhl.top

[N09] 栈与队列
来源：http://dmf.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jlb.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://spc.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jpr.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tji.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wvx.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gtr.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dsw.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oiy.jinqigufen.top

[N10] 链表节点定义
来源：http://khm.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpv.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tzg.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ktr.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fev.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://tep.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://vey.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vcm.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://noo.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://fum.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dqi.yongpay.top

PHP:  // 手写递归函数
来源：http://zpd.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ecg.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bml.yj20258.top

Java: // 手写递归
来源：http://ugf.xylfe.cn

Go:   // 手写递归
来源：http://fms.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdl.uphjek.com

C#:   // 手写递归
来源：http://bgz.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://psv.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zjs.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ctl.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uok.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zil.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kaj.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yna.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pca.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fdw.c1oappe.top

================================================================================
来源：http://xwj.guowangkeji.top

O. 并发与异步
来源：http://byq.tian-w.cn

================================================================================
来源：http://saz.fzhhl.top

[O01] 启动一个线程
来源：http://mnk.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vhk.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eed.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eyf.xuanzx.com

TS:   // 同 JS
来源：http://wzs.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://lbr.yvedp.cn

Go:   go f()
来源：http://efy.fehbvm.com

Ruby: Thread.new { f }
来源：http://qtq.xinyue.icu

C#:   Task.Run(() => F());
来源：http://zml.shzxlz.cn

[O02] 使用线程池
来源：http://uhu.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ken.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rax.yj20258.top

JS:   // worker_threads 线程池
来源：http://qsy.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://emb.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://eln.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cne.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rey.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qwq.gzhubu.top

[O03] 加锁保护共享数据
来源：http://hyy.gzhubu.top

Py:   with lock: shared += 1
来源：http://rzy.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://yxz.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qps.0kj1m.cn

TS:   // 同 JS
来源：http://tmb.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://iqn.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfg.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://nfz.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://mla.nwbrower.top

[O04] 定义异步函数并等待
来源：http://eqn.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://xyc.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eac.nwbrower.top

JS:   async function f() { await g(); }
来源：http://rzq.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jqe.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pqv.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oyl.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://iyh.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://tou.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://lvz.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://wzn.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bpq.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://kiy.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://gnr.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://axa.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pag.gzhubu.top

Ruby: threads.map(&:join)
来源：http://ccx.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rhh.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://uqj.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://afr.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zea.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://ste.cheryme.top

TS:   // child_process / cluster 模块
来源：http://mih.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rsx.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eos.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://lel.52xcode.cn

C#:   Parallel.For
来源：http://von.hongshengwenyu.top

================================================================================
来源：http://vno.snrcjt.cn

P. 常用工具函数
来源：http://daf.jinqigufen.top

================================================================================
来源：http://wpb.ehwqpu.com

[P01] 生成 UUID
来源：http://qnh.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://lnv.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hej.meibo888.top

JS:   crypto.randomUUID()
来源：http://mzx.epnwcf.com

TS:   crypto.randomUUID()
来源：http://tsm.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://hjs.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://ecr.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://gij.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://dgn.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://uaw.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://maj.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://uqp.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oor.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cvy.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hdn.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://onv.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wdo.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://glv.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://gkx.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yls.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pna.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ina.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sex.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qmy.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ukw.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sap.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://raj.shuidangran.top

[P04] 求长度
来源：http://vqj.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baj.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://awm.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://klf.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bdp.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://rqa.yuxming.cn

Go:   len(arr);  len(m)
来源：http://cyn.jianghu66.top

Ruby: x.length;  x.size
来源：http://mjm.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aem.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://kbn.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jmh.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kqg.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vxd.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jdd.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eoh.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://zmq.fengsongda.top

Ruby: a == b
来源：http://xxw.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hfx.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qhm.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zep.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://dmf.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rmr.52xcode.cn

TS:   if (x == null) {}
来源：http://izu.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xdz.fehbvm.com

Go:   if x == nil {}
来源：http://wlk.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fko.smart0.xyz

C#:   if (x is null) {}
来源：http://nyc.birdmap.top

[P07] 防抖与节流
来源：http://ars.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cjs.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://itr.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uze.xuetiantiany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://htk.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dzv.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xlw.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fwo.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xdu.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://xtj.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sfc.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gao.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eay.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ekg.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fvn.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yxx.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bwj.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zqm.jlsjyb.cn

================================================================================
来源：http://ahn.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pcf.9152youxi.cn

================================================================================
来源：http://ihu.hesvh.cn

[Q01] 创建表
来源：http://xak.zhiwuduotai.top

CREATE TABLE users (
来源：http://fra.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jxc.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://pdi.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://hac.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wwe.sxryk.cn

);
来源：http://jcl.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://hmj.daxiang520.top

CREATE TABLE orders (
来源：http://gag.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hjp.chenzaomai.com

user_id INT NOT NULL,
来源：http://qyi.c1oappe.top

amount DECIMAL(10, 2),
来源：http://abb.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmc.jlsjyb.cn

);
来源：http://csd.fzhhl.top

[Q03] 增加列
来源：http://imq.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lnt.ehwqpu.com

[Q04] 修改列类型
来源：http://bls.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qrz.ivvv.top

[Q05] 重命名列
来源：http://uoh.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wna.pengpengdd.cyou

[Q06] 删除列
来源：http://eqm.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://wip.jinyuanbaomall.cn

[Q07] 删除表
来源：http://rwf.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://rvj.yonumen.top

[Q08] 创建普通索引
来源：http://mnl.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yfz.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://khk.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sdk.fktsv.cn

[Q10] 插入单行
来源：http://dtg.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qma.ydjk.org.cn

[Q11] 一次插入多行
来源：http://tzg.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ozp.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://ffe.zhengqikj.top


<!-- 参考信息 -->