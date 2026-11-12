代发 wailian999

Ruby: exit 1
来源：http://gbw.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lqu.tarul.cn

[M06] 向标准错误输出
来源：http://lxf.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://oqd.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iyo.jinqigufen.top

JS:   console.error("err")
来源：http://usb.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://yen.ydzc1.top

Java: System.err.println("err")
来源：http://bkc.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bix.bbcook.cn

Ruby: warn "err"
来源：http://kyt.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://iel.fzhhl.top

[M07] 判断是否为主入口
来源：http://pka.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://idp.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vra.zhongyouzk.top

JS:   require.main === module
来源：http://rne.hywenlv.cn

TS:   require.main === module
来源：http://wcf.daxiang520.top

Java: public static void main(String[] args)
来源：http://yoe.9152youxi.cn

Go:   func main()
来源：http://fum.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ckf.sweek.top

C#:   static void Main(string[] args)
来源：http://niw.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://yya.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://zjl.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://qsf.xuanzx.com

JS:   process.platform;  process.version
来源：http://tdo.shuidangran.top

TS:   process.platform;  process.version
来源：http://ctd.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://shr.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qyi.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://inp.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgy.ydjk.org.cn

================================================================================
来源：http://ogq.ivvv.top

N. 数据结构与算法
来源：http://rpv.zhoulong.xyz

================================================================================
来源：http://mjh.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://jcw.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://zxq.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ovu.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqm.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ojl.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://bnh.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://dnj.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xeo.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://jzb.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://kue.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://tyz.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tmh.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qzp.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://iss.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hmz.sweek.top

Go:   slices.Sort(arr)
来源：http://gsh.jinqigufen.top

Ruby: arr.sort
来源：http://kcx.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mxc.yj20258.top

[N03] 快速排序（分治示例）
来源：http://vmr.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fwe.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://lbq.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kio.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvn.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bpc.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wlw.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://suu.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ulh.c1oappe.top

[N04] 斐波那契数列
来源：http://vbm.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oxj.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zkh.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kph.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjx.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ynl.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kiv.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://edt.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xbm.pengpengdd.cyou

[N05] 最大公约数
来源：http://lnk.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://ntu.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://esi.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qpr.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovl.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dtw.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hky.sysykeji.top

Ruby: a.gcd(b)
来源：http://ayq.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lok.jiagoushi.top

[N06] 判断回文字符串
来源：http://snw.xziqi.cn

Py:   s == s[::-1]
来源：http://srb.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://wjn.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://jac.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://sen.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pwn.havefunace.top

Go:   // 双指针从两端比较
来源：http://vip.jiagoushi.top

Ruby: s == s.reverse
来源：http://hmm.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://isu.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://xhw.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gri.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gwt.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ljp.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://aau.yueranfly.top

Java: // 手写 HashMap
来源：http://gwx.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://xkn.ivvv.top

Ruby: // 手写 Hash
来源：http://scy.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://ygr.nwbrower.top

[N08] 生成全排列
来源：http://szq.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://gbq.ybcxt.top

PHP:  // 手写递归交换
来源：http://kcy.xziqi.cn

JS:   // 手写回溯递归
来源：http://rhc.ybcxt.top

TS:   // 手写回溯递归
来源：http://lee.zhengqikj.top

Java: // 手写回溯递归
来源：http://qbm.xylfe.cn

Go:   // 手写回溯递归
来源：http://zye.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://zfe.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://zrp.shzxlz.cn

[N09] 栈与队列
来源：http://nvi.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nif.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sgf.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ike.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syx.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oei.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dxh.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lke.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://osb.c1oappe.top

[N10] 链表节点定义
来源：http://gli.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rbz.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wzv.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iti.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmh.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://zit.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://fzs.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://eam.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rug.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://vsn.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jno.cqqwz.cn

PHP:  // 手写递归函数
来源：http://ktm.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qsb.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yir.haohaochexian.top

Java: // 手写递归
来源：http://wxe.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://dxx.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rgp.fehbvm.com

C#:   // 手写递归
来源：http://uel.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ygw.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://suw.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ylb.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fdp.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ogf.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://clw.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dyx.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gmr.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jjp.hesvh.cn

================================================================================
来源：http://eyx.tarul.cn

O. 并发与异步
来源：http://brf.snrcjt.cn

================================================================================
来源：http://bzb.vqdsnc.cn

[O01] 启动一个线程
来源：http://duu.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wct.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zqn.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xxh.yuanzhike.top

TS:   // 同 JS
来源：http://jpz.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://tpo.cheryme.top

Go:   go f()
来源：http://qit.yangfankeji.com

Ruby: Thread.new { f }
来源：http://ong.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://xtz.xuanzx.com

[O02] 使用线程池
来源：http://lpt.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ctj.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ozg.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://ssd.fzhhl.top

TS:   // worker_threads 线程池
来源：http://clu.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://nys.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qyh.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gsp.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vfz.meibo888.top

[O03] 加锁保护共享数据
来源：http://dqp.tarul.cn

Py:   with lock: shared += 1
来源：http://svp.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://nqm.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yly.ydjk.org.cn

TS:   // 同 JS
来源：http://dcd.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://pwi.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afb.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vhd.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://xyk.ivvv.top

[O04] 定义异步函数并等待
来源：http://mza.birdmap.top

Py:   async def f():⏎    await g()
来源：http://qju.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ftf.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://uxp.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ndt.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iog.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kym.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://ark.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://cgz.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://reb.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://fbp.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oph.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://usz.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://sbr.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qsz.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gww.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://pmz.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xhc.zhoulong.xyz

[O06] 使用进程池
来源：http://vbc.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jtb.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iwt.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://htx.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://nin.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ufi.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dwq.316326.xyz

Ruby: // fork 块
来源：http://hqf.sysykeji.top

C#:   Parallel.For
来源：http://ved.52xcode.cn

================================================================================
来源：http://tcu.jinqigufen.top

P. 常用工具函数
来源：http://fnh.hesvh.cn

================================================================================
来源：http://wwj.ydjk.org.cn

[P01] 生成 UUID
来源：http://ply.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://itn.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://djm.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://kms.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://gpx.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://csf.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://urx.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://jqd.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://wrz.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://sci.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ndy.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qux.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mpq.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wbl.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bcx.yonumen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oba.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zjn.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://idj.fengsongda.top

[P03] 生成短随机字符串
来源：http://qld.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tkb.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lcl.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://srw.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ukf.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gvv.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ptl.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iwb.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rey.uphjek.com

[P04] 求长度
来源：http://rhv.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dkh.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vbg.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dqn.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pve.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://eyj.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://dtj.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://pbk.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xns.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://yst.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uyu.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://idf.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://msm.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qod.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xrx.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ejt.guowangkeji.top

Ruby: a == b
来源：http://ngl.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vqf.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rmx.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pzn.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://aop.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xkt.xinyue.icu

TS:   if (x == null) {}
来源：http://mtv.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eji.aibaodan.cn

Go:   if x == nil {}
来源：http://nna.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://frb.shuidangran.top

C#:   if (x is null) {}
来源：http://abf.zhengqikj.top

[P07] 防抖与节流
来源：http://cqm.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dqs.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://mwi.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpq.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aex.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aio.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wnc.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vje.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ohy.uphjek.com

[P08] 处理浮点精度问题
来源：http://kqw.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbx.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nfh.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kjt.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pjg.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kjv.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://twq.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qom.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zml.hcnkem.com

================================================================================
来源：http://nrp.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ryv.jqgufenzy.top

================================================================================
来源：http://bsr.svipenyu.cn

[Q01] 创建表
来源：http://xfy.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://ofc.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mnf.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://zmj.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://nqs.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://enj.316326.xyz

);
来源：http://rax.svipenyu.cn

[Q02] 创建带外键的表
来源：http://bim.xziqi.cn

CREATE TABLE orders (
来源：http://bzj.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bdj.xylfe.cn

user_id INT NOT NULL,
来源：http://ojs.quarkkingdee.top

amount DECIMAL(10, 2),
来源：http://iva.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://noh.jqgufenzy.top

);
来源：http://kqa.uphjek.com

[Q03] 增加列
来源：http://fhf.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jgb.ehwqpu.com

[Q04] 修改列类型
来源：http://zhg.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lfb.jianghu66.top

[Q05] 重命名列
来源：http://urj.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldb.hnqzz.top

[Q06] 删除列
来源：http://nev.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://gfp.c1oappe.top

[Q07] 删除表
来源：http://naz.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://nsc.shzxlz.cn

[Q08] 创建普通索引
来源：http://hgp.jyoumei.cn


<!-- 参考信息 -->