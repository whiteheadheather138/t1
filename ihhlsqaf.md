代发 wailian999

Py:   if __name__ == "__main__":
来源：http://emx.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mph.aizwys.cn

JS:   require.main === module
来源：http://bbh.xylfe.cn

TS:   require.main === module
来源：http://azq.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://vnc.zycfv.cn

Go:   func main()
来源：http://xcc.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gck.daxiang520.top

C#:   static void Main(string[] args)
来源：http://ikm.ivvv.top

[M08] 获取系统与运行时信息
来源：http://ndw.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://iqo.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://whm.sweek.top

JS:   process.platform;  process.version
来源：http://ezw.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://wth.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ghj.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://euf.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nxq.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mml.vqdsnc.cn

================================================================================
来源：http://ffb.jinqigfzy.top

N. 数据结构与算法
来源：http://rvb.daria6918.cn

================================================================================
来源：http://plf.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://zfj.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gcw.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ias.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kny.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zad.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://vwj.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://mph.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qus.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://yjh.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://aeh.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://zwi.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zef.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oaf.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mkq.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hrn.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://deb.yj20258.top

Ruby: arr.sort
来源：http://fzz.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pne.pycfn.com

[N03] 快速排序（分治示例）
来源：http://obs.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vgy.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://pcd.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kgk.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ech.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wct.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qrh.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://djf.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eqt.sufxvd.cn

[N04] 斐波那契数列
来源：http://iyz.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gdu.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rff.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ueq.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ben.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ert.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://osf.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://roh.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qbv.ydzc1.top

[N05] 最大公约数
来源：http://hkl.xziqi.cn

Py:   math.gcd(a, b)
来源：http://rot.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wcl.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fkr.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hoh.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ljm.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zfz.ppjwa.cn

Ruby: a.gcd(b)
来源：http://qey.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yon.ppjwa.cn

[N06] 判断回文字符串
来源：http://pew.yonumen.top

Py:   s == s[::-1]
来源：http://oiz.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://twb.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://thl.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://cdi.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://drf.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://okx.xuanzx.com

Ruby: s == s.reverse
来源：http://bla.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gwu.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://rtp.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vcp.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pkv.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rsv.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://xkz.cqqwz.cn

Java: // 手写 HashMap
来源：http://yhz.fehbvm.com

Go:   // 手写 map[int]int
来源：http://dol.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://vet.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://fwb.jinqigfzy.top

[N08] 生成全排列
来源：http://zzs.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://jhj.shuidangran.top

PHP:  // 手写递归交换
来源：http://sxn.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://bdr.xuanzx.com

TS:   // 手写回溯递归
来源：http://pnu.chenzaomai.com

Java: // 手写回溯递归
来源：http://gdi.sysykeji.top

Go:   // 手写回溯递归
来源：http://suk.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://fbz.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://thh.yueranfly.top

[N09] 栈与队列
来源：http://lsr.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://owi.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wjp.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qcp.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://csr.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fap.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fuq.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yej.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cam.jlsjyb.cn

[N10] 链表节点定义
来源：http://nir.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qbk.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gbq.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fos.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cnp.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://yyd.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fkt.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dgu.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hng.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://nqe.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bmf.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://lbe.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qjk.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zlp.hnxiangtu.top

Java: // 手写递归
来源：http://nnr.hammf.cn

Go:   // 手写递归
来源：http://vpl.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ysb.jqgufenzy.top

C#:   // 手写递归
来源：http://ter.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ise.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tvt.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fcv.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jlo.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rxu.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fhf.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dpr.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjo.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://orb.zhaomingkeji.xyz

================================================================================
来源：http://loa.hcnkem.com

O. 并发与异步
来源：http://aqf.yj202588.top

================================================================================
来源：http://vcm.shzxlz.cn

[O01] 启动一个线程
来源：http://ayj.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zuj.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ukh.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gnx.cqqwz.cn

TS:   // 同 JS
来源：http://uxd.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://ldw.dashuyun.cn

Go:   go f()
来源：http://kda.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://qtm.bjfxy.top

C#:   Task.Run(() => F());
来源：http://prd.sysykeji.top

[O02] 使用线程池
来源：http://otz.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fzj.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kum.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://czt.redwolf501.top

TS:   // worker_threads 线程池
来源：http://qtu.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://rmn.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jcl.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gxl.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kxn.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://zob.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://boa.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://rpi.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cui.pycfn.com

TS:   // 同 JS
来源：http://mzj.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://woc.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fel.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ztf.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://vtc.zycfv.cn

[O04] 定义异步函数并等待
来源：http://taz.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://bcl.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ins.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://bzr.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://siq.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lyg.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rox.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lmz.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://are.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://hro.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://etr.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vjt.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://ckw.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://kkt.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fly.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fiv.daria6918.cn

Ruby: threads.map(&:join)
来源：http://zwk.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vat.316326.xyz

[O06] 使用进程池
来源：http://kxt.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uew.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zyo.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://vjl.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://oju.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fnm.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aya.hcnkem.com

Ruby: // fork 块
来源：http://mcg.fzhhl.top

C#:   Parallel.For
来源：http://lzs.hcnkem.com

================================================================================
来源：http://ggq.sysykeji.top

P. 常用工具函数
来源：http://zxj.shuidangran.top

================================================================================
来源：http://ntx.sysykeji.top

[P01] 生成 UUID
来源：http://rgo.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://wly.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qsm.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://mrh.bjfxy.top

TS:   crypto.randomUUID()
来源：http://nfg.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://zti.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://krp.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://ush.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://mnu.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://yhn.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cpk.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zut.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sgc.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://osn.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ysm.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://npm.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vih.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ckx.sysykeji.top

[P03] 生成短随机字符串
来源：http://jqa.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ikp.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ptr.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aqy.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lhb.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fup.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sfp.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://amw.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oxi.uphjek.com

[P04] 求长度
来源：http://rme.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mej.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mtu.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asc.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwz.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://fth.fengsongda.top

Go:   len(arr);  len(m)
来源：http://qsb.fehbvm.com

Ruby: x.length;  x.size
来源：http://rip.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dln.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://kva.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bif.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ilu.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wti.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ebt.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bld.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://ppl.hywenlv.cn

Ruby: a == b
来源：http://gaj.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ghy.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://swa.chenjidiqi.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wqe.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://uwh.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://crf.vqdsnc.cn

TS:   if (x == null) {}
来源：http://tbv.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vll.dashuyun.cn

Go:   if x == nil {}
来源：http://yus.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mde.redwolf501.top

C#:   if (x is null) {}
来源：http://wiu.ydzc1.top

[P07] 防抖与节流
来源：http://ncj.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zlx.birdmap.top

PHP:  // 手写时间戳比较
来源：http://kus.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qut.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibb.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rbq.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vtc.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lro.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ndu.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://ind.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ooy.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nvp.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oxa.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tyn.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ucb.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wac.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mum.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aln.uphjek.com

================================================================================
来源：http://tjo.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hwf.kuanghao11.cn

================================================================================
来源：http://hma.havefunace.top

[Q01] 创建表
来源：http://fry.jinqigufen.top

CREATE TABLE users (
来源：http://afq.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wuk.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://psa.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://tij.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://epj.mhx1999.top

);
来源：http://oxv.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://pum.shangyingyoupin.top

CREATE TABLE orders (
来源：http://mrp.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vdk.shuidangran.top

user_id INT NOT NULL,
来源：http://mpg.zycfv.cn

amount DECIMAL(10, 2),
来源：http://yve.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ypa.yuxming.cn

);
来源：http://ige.yuxming.cn

[Q03] 增加列
来源：http://cqr.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dpg.jinqigfzy.top

[Q04] 修改列类型
来源：http://ywn.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://veo.hnqzz.top

[Q05] 重命名列
来源：http://otb.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kcj.bbcook.cn

[Q06] 删除列
来源：http://hna.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://dxi.nwbrower.top

[Q07] 删除表
来源：http://lsv.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://wbh.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://nyh.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://qnl.chenlongwang.top

[Q09] 创建唯一索引
来源：http://qfr.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qor.uphjek.com

[Q10] 插入单行
来源：http://ucr.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lpr.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://tlg.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://brw.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://adp.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://rku.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://old.yj202588.top

[Q13] 忽略重复插入
来源：http://tpd.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oaq.dashuyun.cn


<!-- 参考信息 -->