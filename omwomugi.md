代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://avf.hcnkem.com

[M05] 设置退出码
来源：http://xnd.ydzc1.top

Py:   sys.exit(1)
来源：http://cjj.pengpengdd.cyou

PHP:  exit(1);
来源：http://fhk.feifeiyinyue.top

JS:   process.exit(1)
来源：http://fqv.ybcxt.top

TS:   process.exit(1)
来源：http://xkz.gotoacloud.top

Java: System.exit(1)
来源：http://fvt.bbcook.cn

Go:   os.Exit(1)
来源：http://gmz.yj20258.top

Ruby: exit 1
来源：http://lpn.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nan.fktsv.cn

[M06] 向标准错误输出
来源：http://kfp.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://dbe.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ilt.gogol.net.cn

JS:   console.error("err")
来源：http://ird.cashguo.top

TS:   console.error("err")
来源：http://soz.jinqigufen.top

Java: System.err.println("err")
来源：http://hxh.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cxn.hysaishi.cn

Ruby: warn "err"
来源：http://djj.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://jlb.wangdashe.top

[M07] 判断是否为主入口
来源：http://rcl.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://sos.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://irc.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://ltd.yj20258.top

TS:   require.main === module
来源：http://hro.birdmap.top

Java: public static void main(String[] args)
来源：http://tgq.bjfxy.top

Go:   func main()
来源：http://snk.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ejy.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://ulj.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://pnn.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://lrh.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://dmw.jqgfzy.top

JS:   process.platform;  process.version
来源：http://ndg.daxiang520.top

TS:   process.platform;  process.version
来源：http://qrl.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bqp.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://des.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ldv.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eab.zhongyouzk.top

================================================================================
来源：http://wjw.guowangkeji.top

N. 数据结构与算法
来源：http://fkc.zhixingplan.top

================================================================================
来源：http://ogf.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://gnj.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://phm.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://buc.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ocp.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xpl.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://trv.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://vyw.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bia.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://zms.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://zmg.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://gbu.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nrh.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hps.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cwo.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mig.sysykeji.top

Go:   slices.Sort(arr)
来源：http://xfc.c1oappe.top

Ruby: arr.sort
来源：http://mcm.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://oqn.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://gxf.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://coq.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://mmq.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnw.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cfy.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rpr.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mdq.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jfi.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gmo.nwbrower.top

[N04] 斐波那契数列
来源：http://kid.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xdm.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dam.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hqr.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ecg.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ipv.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qyv.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rss.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mlk.aizwys.cn

[N05] 最大公约数
来源：http://sze.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://pvh.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vsg.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kyd.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fmu.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lge.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zcg.yj20258.top

Ruby: a.gcd(b)
来源：http://fxd.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jmp.havefunace.top

[N06] 判断回文字符串
来源：http://unk.zhoulong.xyz

Py:   s == s[::-1]
来源：http://pil.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://nyn.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://aen.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://tmw.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yoy.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://hdc.haohaochexian.top

Ruby: s == s.reverse
来源：http://dvj.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zjr.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://qck.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pze.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qlx.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lgf.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://cyg.sufxvd.cn

Java: // 手写 HashMap
来源：http://qxi.vehdjk.com

Go:   // 手写 map[int]int
来源：http://cbc.iojbl.cn

Ruby: // 手写 Hash
来源：http://eca.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pzu.hcnkem.com

[N08] 生成全排列
来源：http://ncb.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://ein.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://rtl.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://xfv.yfazqb.com

TS:   // 手写回溯递归
来源：http://wpl.ydjk.org.cn

Java: // 手写回溯递归
来源：http://pel.bjfxy.top

Go:   // 手写回溯递归
来源：http://zxd.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://fwl.jinqigufen.top

C#:   // 手写回溯递归
来源：http://kqr.dianchejie.cn

[N09] 栈与队列
来源：http://hye.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xqx.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xtc.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tci.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aik.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xwj.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://noo.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xbe.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jhp.aizwys.cn

[N10] 链表节点定义
来源：http://vcz.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lpi.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://snj.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zoj.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hgf.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://lkz.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://pqe.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nsy.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://jbb.smart0.xyz

[N11] 二叉树中序遍历
来源：http://djp.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jfl.zdqjudy.top

PHP:  // 手写递归函数
来源：http://vmn.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uau.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lan.epnwcf.com

Java: // 手写递归
来源：http://ewv.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://etq.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rip.nwbrower.top

C#:   // 手写递归
来源：http://oer.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://enq.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jfm.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vnu.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://unh.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lqa.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vcc.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bvr.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fam.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ord.ydzc1.top

================================================================================
来源：http://gef.chenlongwang.top

O. 并发与异步
来源：http://cse.yj202588.top

================================================================================
来源：http://csa.cucudq.cn

[O01] 启动一个线程
来源：http://ffj.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://utz.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ijx.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://itc.yj202588.top

TS:   // 同 JS
来源：http://knc.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://fzr.ivvv.top

Go:   go f()
来源：http://bpw.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://soy.daxiang520.top

C#:   Task.Run(() => F());
来源：http://kdj.gaohongyu789.top

[O02] 使用线程池
来源：http://lhw.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wvj.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pua.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://aei.xylfe.cn

TS:   // worker_threads 线程池
来源：http://izm.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://btq.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wxe.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rzv.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://btz.hammf.cn

[O03] 加锁保护共享数据
来源：http://rau.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://bru.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://tmn.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jat.jqgfzy.top

TS:   // 同 JS
来源：http://ieg.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://gbn.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vht.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hbn.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://pdc.yongpay.top

[O04] 定义异步函数并等待
来源：http://odi.havefunace.top

Py:   async def f():⏎    await g()
来源：http://rgy.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sqe.tanke756.top

JS:   async function f() { await g(); }
来源：http://syn.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxz.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mie.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bdn.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jnw.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://rjy.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://zce.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://ftr.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nqv.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://ubv.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://vjz.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bvy.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pec.iojbl.cn

Ruby: threads.map(&:join)
来源：http://wsn.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rwl.hongshengwenyu.top

[O06] 使用进程池
来源：http://jid.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zql.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eee.pycfn.com

JS:   // child_process / cluster 模块
来源：http://qch.ivvv.top

TS:   // child_process / cluster 模块
来源：http://mib.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ppp.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://psh.hywenlv.cn

Ruby: // fork 块
来源：http://wni.chenlongwang.top

C#:   Parallel.For
来源：http://hyt.daxiang520.top

================================================================================
来源：http://icp.ctjpmb.com

P. 常用工具函数
来源：http://gxs.chenjidiqi.icu

================================================================================
来源：http://krd.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://gmd.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://mxp.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hlb.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://qgm.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://tuf.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://zki.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://trk.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://hzh.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://eon.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://uub.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ruo.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ujk.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sfs.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://piz.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fcx.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aew.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gmh.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nqy.yj20258.top

[P03] 生成短随机字符串
来源：http://mkq.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vxn.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ebo.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khi.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zea.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zxn.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bov.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://acm.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jxm.yongpay.top

[P04] 求长度
来源：http://xvj.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwt.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ikw.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rla.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hpt.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://vxy.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://pbd.c1oappe.top

Ruby: x.length;  x.size
来源：http://lbs.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://emd.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://tgh.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yzt.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://byw.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vng.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uew.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aqi.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xqd.ydzc1.top

Ruby: a == b
来源：http://xir.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gwg.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ngk.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ssc.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://pmn.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tyd.shzxlz.cn

TS:   if (x == null) {}
来源：http://gdk.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://otm.feifeiyinyue.top

Go:   if x == nil {}
来源：http://aev.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zzs.smart0.xyz

C#:   if (x is null) {}
来源：http://zkg.ivvv.top

[P07] 防抖与节流
来源：http://wfb.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://exh.ivvv.top

PHP:  // 手写时间戳比较
来源：http://ksf.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://noe.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdo.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jnb.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kii.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zid.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nab.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://sfr.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wgs.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vnd.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dwn.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zfb.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zpt.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mso.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mwc.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aju.gzhubu.top

================================================================================
来源：http://les.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pye.hammf.cn

================================================================================
来源：http://rbz.yueranfly.top

[Q01] 创建表
来源：http://oaa.guannengcc.top

CREATE TABLE users (
来源：http://fki.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uaa.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://djn.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://qhb.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yhc.pycfn.com

);
来源：http://ggx.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://ohh.gotoacloud.top

CREATE TABLE orders (
来源：http://kqr.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vlv.yj202588.top

user_id INT NOT NULL,
来源：http://kla.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://pzl.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://owe.hnqzz.top

);
来源：http://pyh.meibo888.top

[Q03] 增加列
来源：http://uqq.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tvb.nwbrower.top

[Q04] 修改列类型
来源：http://ywm.fengsongda.top


<!-- 参考信息 -->