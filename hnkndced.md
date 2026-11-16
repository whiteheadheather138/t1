代发 wailian999

Py:   if __name__ == "__main__":
来源：http://uia.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iqv.guowangkeji.top

JS:   require.main === module
来源：http://ram.jinghuilouyu.cn

TS:   require.main === module
来源：http://xko.52xcode.cn

Java: public static void main(String[] args)
来源：http://nph.andypj.xyz

Go:   func main()
来源：http://rke.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tij.epnwcf.com

C#:   static void Main(string[] args)
来源：http://iqy.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://mof.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://oon.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://nzi.gzhubu.top

JS:   process.platform;  process.version
来源：http://meb.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://xmh.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ixq.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://smc.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dic.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xal.tianlin.xyz

================================================================================
来源：http://qap.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://tnf.hnxiangtu.top

================================================================================
来源：http://lbr.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://yhe.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://wfy.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://osi.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msl.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vxf.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wdh.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://cdj.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nuc.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://usv.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://pac.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://klb.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jrx.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nnr.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bje.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fgh.vehdjk.com

Go:   slices.Sort(arr)
来源：http://ijq.sweek.top

Ruby: arr.sort
来源：http://hbd.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fzy.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://wrn.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gbg.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://lrx.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://txk.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zrl.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufc.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwj.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kiw.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://syp.yuxming.cn

[N04] 斐波那契数列
来源：http://byr.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://glx.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nnk.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oss.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tem.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hpy.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zoa.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ebl.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jux.fzhhl.top

[N05] 最大公约数
来源：http://tzq.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://ccj.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://npp.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hli.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcj.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://igo.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sfs.tian-w.cn

Ruby: a.gcd(b)
来源：http://ksb.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mgj.dashuyun.cn

[N06] 判断回文字符串
来源：http://zds.gotoacloud.top

Py:   s == s[::-1]
来源：http://ykd.52xcode.cn

PHP:  $s === strrev($s);
来源：http://kci.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://xto.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://svh.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sgk.ybcxt.top

Go:   // 双指针从两端比较
来源：http://yde.tianlin.xyz

Ruby: s == s.reverse
来源：http://joe.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://abo.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://gmj.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vzg.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cga.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hzn.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://aix.gaohongyu789.top

Java: // 手写 HashMap
来源：http://gun.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://apj.yuxming.cn

Ruby: // 手写 Hash
来源：http://dpo.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://ljh.sxryk.cn

[N08] 生成全排列
来源：http://ids.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://nik.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://hek.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://fhy.meibo888.top

TS:   // 手写回溯递归
来源：http://jxh.quarkkingdee.top

Java: // 手写回溯递归
来源：http://opl.jinqigufen.top

Go:   // 手写回溯递归
来源：http://dis.yongpay.top

Ruby: arr.permutation.to_a
来源：http://dxe.xuanzx.com

C#:   // 手写回溯递归
来源：http://sal.vqdsnc.cn

[N09] 栈与队列
来源：http://azv.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vdi.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ohw.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://smd.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mbn.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://clr.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uvg.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://skr.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://crj.jlsjyb.cn

[N10] 链表节点定义
来源：http://riu.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gva.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dtw.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lpw.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wkr.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://txv.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cdr.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ohi.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://sod.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://erh.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xiv.zdqjudy.top

PHP:  // 手写递归函数
来源：http://gqv.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lwa.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rdv.yvedp.cn

Java: // 手写递归
来源：http://bgv.52xcode.cn

Go:   // 手写递归
来源：http://xyz.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://afc.cqqwz.cn

C#:   // 手写递归
来源：http://npp.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://che.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ftm.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wmh.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mmz.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbo.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ibk.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cjx.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ljj.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ubf.zhiwuduotai.top

================================================================================
来源：http://pzi.chenzaomai.com

O. 并发与异步
来源：http://rnx.gotoacloud.top

================================================================================
来源：http://atz.gzhubu.top

[O01] 启动一个线程
来源：http://zge.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vyk.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eri.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://goc.ydjk.org.cn

TS:   // 同 JS
来源：http://uyv.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://kcw.jqgufenzy.top

Go:   go f()
来源：http://gbe.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://ljl.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://tbu.xingfuxueyuan.xyz

[O02] 使用线程池
来源：http://sbk.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ukc.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cxq.uphjek.com

JS:   // worker_threads 线程池
来源：http://ghg.tanke756.top

TS:   // worker_threads 线程池
来源：http://twr.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://xsr.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://slk.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ohr.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eeu.xziqi.cn

[O03] 加锁保护共享数据
来源：http://pyg.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://hxl.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://htk.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rmd.dianchejie.cn

TS:   // 同 JS
来源：http://qnn.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://wfr.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wpw.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://aks.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://mxn.zycfv.cn

[O04] 定义异步函数并等待
来源：http://izq.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://vgb.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jht.tanke756.top

JS:   async function f() { await g(); }
来源：http://ned.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hmg.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tut.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mhd.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://gnp.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://uhn.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://amc.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://lue.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rzp.cashguo.top

JS:   await Promise.all(tasks)
来源：http://crg.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://qpj.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qez.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zoc.tanke756.top

Ruby: threads.map(&:join)
来源：http://leg.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://knq.jqgufenzy.top

[O06] 使用进程池
来源：http://hlp.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lxg.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zxm.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://ggu.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://mwi.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sas.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gzj.dianchejie.cn

Ruby: // fork 块
来源：http://obj.dianchejie.cn

C#:   Parallel.For
来源：http://fge.yvedp.cn

================================================================================
来源：http://hqx.uphjek.com

P. 常用工具函数
来源：http://odn.redwolf501.top

================================================================================
来源：http://nrw.mhx1999.top

[P01] 生成 UUID
来源：http://tth.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://ifr.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zzc.cucudq.cn

JS:   crypto.randomUUID()
来源：http://llm.wangdashe.top

TS:   crypto.randomUUID()
来源：http://hec.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://gnj.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://pth.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://mbt.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://jik.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://deo.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xeu.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qej.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nxw.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wxr.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://idh.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nfr.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uwg.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kyi.svipenyu.cn

[P03] 生成短随机字符串
来源：http://tts.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://maf.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iur.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxs.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://udt.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ejv.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dvl.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nto.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://epb.sweek.top

[P04] 求长度
来源：http://irp.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gys.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lak.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://moz.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qvf.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://bmy.cheryme.top

Go:   len(arr);  len(m)
来源：http://agk.yuxming.cn

Ruby: x.length;  x.size
来源：http://tfp.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gqb.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://gbi.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://pwv.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://avd.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iqj.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oyd.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nkl.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://enp.zhijiandao.cn

Ruby: a == b
来源：http://xrr.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jzw.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://byu.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ypo.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://wcn.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pad.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://xvt.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wgj.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://lyr.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jcp.mhx1999.top

C#:   if (x is null) {}
来源：http://vgl.cucudq.cn

[P07] 防抖与节流
来源：http://kvb.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cly.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://ooy.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pht.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azd.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lsl.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://epc.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hta.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oth.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://wwa.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xye.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ssk.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hje.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://szy.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rqa.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ikb.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vpj.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lgg.jiagoushi.top

================================================================================
来源：http://emq.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wqf.chenlongwang.top

================================================================================
来源：http://wmo.hfpthk.cn

[Q01] 创建表
来源：http://ars.ydzc1.top

CREATE TABLE users (
来源：http://tnk.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://akx.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://xhi.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://dnu.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tlv.zdbjq.cn

);
来源：http://osz.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://wnj.dashuyun.cn

CREATE TABLE orders (
来源：http://rwa.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ljv.zhixingplan.top

user_id INT NOT NULL,
来源：http://las.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://sbv.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jpr.fanxiaobao.xyz

);
来源：http://khr.shuidangran.top

[Q03] 增加列
来源：http://oxe.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://olc.hcnkem.com

[Q04] 修改列类型
来源：http://sif.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pqs.mhx1999.top

[Q05] 重命名列
来源：http://toi.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zan.xziqi.cn

[Q06] 删除列
来源：http://suu.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://fuq.yj20258888.top

[Q07] 删除表
来源：http://gli.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://atj.pycfn.com

[Q08] 创建普通索引
来源：http://cxx.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tpg.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://ckh.aibaodan.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://usi.cqqwz.cn

[Q10] 插入单行
来源：http://ftn.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vev.yj202588.top

[Q11] 一次插入多行
来源：http://ncn.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ltf.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://paf.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://mix.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zrw.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://kja.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nno.zhongyouzk.top


<!-- 参考信息 -->