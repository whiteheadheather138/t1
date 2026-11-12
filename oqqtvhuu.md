代发 wailian999

JS:   process.exit(1)
来源：http://fji.vqdsnc.cn

TS:   process.exit(1)
来源：http://ebf.zhiwuduotai.top

Java: System.exit(1)
来源：http://hza.daria6918.cn

Go:   os.Exit(1)
来源：http://vzo.snrcjt.cn

Ruby: exit 1
来源：http://acp.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://par.chenlongwang.top

[M06] 向标准错误输出
来源：http://pcu.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://jol.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://srl.9152youxi.cn

JS:   console.error("err")
来源：http://qne.jlsjyb.cn

TS:   console.error("err")
来源：http://bhh.hysaishi.cn

Java: System.err.println("err")
来源：http://zgw.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ypf.bjfxy.top

Ruby: warn "err"
来源：http://sfc.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://ssk.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://qqs.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://ysq.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://php.yj202588.top

JS:   require.main === module
来源：http://jdx.yangfankeji.com

TS:   require.main === module
来源：http://aqv.redwolf501.top

Java: public static void main(String[] args)
来源：http://flu.iojbl.cn

Go:   func main()
来源：http://epk.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bbb.andypj.xyz

C#:   static void Main(string[] args)
来源：http://cyo.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://lqm.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://fhe.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://mwi.aizwys.cn

JS:   process.platform;  process.version
来源：http://mrp.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://xgh.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csa.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fse.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://etq.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://brl.ydjk.org.cn

================================================================================
来源：http://iph.yueranfly.top

N. 数据结构与算法
来源：http://ozi.ybcxt.top

================================================================================
来源：http://mhp.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://lie.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://gbr.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://geu.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kkz.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbb.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://cmg.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://qkf.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eyz.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://umu.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://iks.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://tve.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kyk.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eho.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ole.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://msb.tarul.cn

Go:   slices.Sort(arr)
来源：http://cxf.guowangkeji.top

Ruby: arr.sort
来源：http://icw.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bid.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://qwx.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fhn.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://tnq.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ykp.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qho.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qcu.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wml.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iff.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://ygo.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://bpx.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ild.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://flu.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cjh.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pno.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hzk.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jxh.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rfx.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xmk.sweek.top

[N05] 最大公约数
来源：http://qfa.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://ebe.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qbb.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vdb.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hsf.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ntv.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lil.ehwqpu.com

Ruby: a.gcd(b)
来源：http://ued.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://srw.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://gwx.shzxlz.cn

Py:   s == s[::-1]
来源：http://ufi.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://gpl.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://nxn.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://svu.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://srb.xuanzx.com

Go:   // 双指针从两端比较
来源：http://ofq.316326.xyz

Ruby: s == s.reverse
来源：http://ohh.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rtt.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://bxa.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hvc.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qoq.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://iov.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://cyd.dianchejie.cn

Java: // 手写 HashMap
来源：http://doh.hammf.cn

Go:   // 手写 map[int]int
来源：http://qnt.sxryk.cn

Ruby: // 手写 Hash
来源：http://vat.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rpb.nanxinkj.top

[N08] 生成全排列
来源：http://ong.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://pjd.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://fps.c1oappe.top

JS:   // 手写回溯递归
来源：http://mqq.cqqwz.cn

TS:   // 手写回溯递归
来源：http://uwy.snrcjt.cn

Java: // 手写回溯递归
来源：http://wnr.zdbjq.cn

Go:   // 手写回溯递归
来源：http://roq.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://wgf.andypj.xyz

C#:   // 手写回溯递归
来源：http://ylm.snrcjt.cn

[N09] 栈与队列
来源：http://bgr.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pjk.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://abk.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ywf.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qbp.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xza.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kil.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eiq.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wbq.ydzc1.top

[N10] 链表节点定义
来源：http://wkh.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rpb.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jzj.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vft.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hhp.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://wkt.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://pbn.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cse.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wwv.redwolf501.top

[N11] 二叉树中序遍历
来源：http://qge.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ale.guowangkeji.top

PHP:  // 手写递归函数
来源：http://ctr.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ydf.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwc.ehwqpu.com

Java: // 手写递归
来源：http://idd.nwbrower.top

Go:   // 手写递归
来源：http://omc.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rcc.xylfe.cn

C#:   // 手写递归
来源：http://eqn.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pmx.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbb.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cip.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opv.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjb.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://euh.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oky.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lvt.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xfu.dashuyun.cn

================================================================================
来源：http://xis.zhijiandao.cn

O. 并发与异步
来源：http://wjy.yj20258888.top

================================================================================
来源：http://qcf.jqgfzy.top

[O01] 启动一个线程
来源：http://tzf.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vso.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eew.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ycu.jqgfzy.top

TS:   // 同 JS
来源：http://itn.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://gno.yueranfly.top

Go:   go f()
来源：http://vlh.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://vpo.fehbvm.com

C#:   Task.Run(() => F());
来源：http://eqz.snrcjt.cn

[O02] 使用线程池
来源：http://wuz.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://amu.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dww.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://vzb.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://noy.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://ziz.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://haw.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://meh.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cwb.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://oxb.zhengqikj.top

Py:   with lock: shared += 1
来源：http://qit.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://oxn.hfpthk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mfa.jinghuilouyu.cn

TS:   // 同 JS
来源：http://ios.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://egb.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kku.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zxu.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://aiv.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://irj.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://xdu.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hnz.cheryme.top

JS:   async function f() { await g(); }
来源：http://cba.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ovz.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://usv.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://azm.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://rku.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://doo.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://uyj.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://fct.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wve.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://mpc.316326.xyz

TS:   await Promise.all(tasks)
来源：http://qsf.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hxf.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xma.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://qyd.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://puc.zdbjq.cn

[O06] 使用进程池
来源：http://rir.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gjy.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://kvl.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://fap.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://vuu.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ngf.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dqy.sweek.top

Ruby: // fork 块
来源：http://yje.zhiwuduotai.top

C#:   Parallel.For
来源：http://ivy.jinghuilouyu.cn

================================================================================
来源：http://coe.yj20258888.top

P. 常用工具函数
来源：http://wix.vehdjk.com

================================================================================
来源：http://bqc.nanxinkj.top

[P01] 生成 UUID
来源：http://iur.hammf.cn

Py:   str(uuid.uuid4())
来源：http://jrg.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rob.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://riy.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://ftp.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://mwa.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://fqy.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://jeo.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://tur.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://hjb.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tbr.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://flu.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ckb.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://enk.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://twn.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vpi.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://glb.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kkm.c1oappe.top

[P03] 生成短随机字符串
来源：http://flo.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zjf.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rix.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cys.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yma.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nme.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fcu.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uqs.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dwa.shanyushiyangtech.top

[P04] 求长度
来源：http://aae.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fbn.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iqm.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ozo.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hzx.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://gll.tian-w.cn

Go:   len(arr);  len(m)
来源：http://rkr.sweek.top

Ruby: x.length;  x.size
来源：http://xml.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yuw.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://qsb.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bpq.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://clt.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ijc.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ecy.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ops.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://kol.c1oappe.top

Ruby: a == b
来源：http://tbi.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dtm.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://niq.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vwk.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://fet.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dqg.chenlongwang.top

TS:   if (x == null) {}
来源：http://aww.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ugp.vehdjk.com

Go:   if x == nil {}
来源：http://zbu.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wem.redwolf501.top

C#:   if (x is null) {}
来源：http://xxe.zhoulong.xyz

[P07] 防抖与节流
来源：http://nse.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gul.birdmap.top

PHP:  // 手写时间戳比较
来源：http://wvo.daxiang520.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwh.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vqc.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lcc.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eae.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zbt.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://byo.meibo888.top

[P08] 处理浮点精度问题
来源：http://bsr.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ltd.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pcg.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nsr.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lth.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rre.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xop.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oly.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vsf.ctjpmb.com

================================================================================
来源：http://hau.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lit.yj202588.top

================================================================================
来源：http://zsb.fanxiaobao.xyz

[Q01] 创建表
来源：http://fsi.jinqigfzy.top

CREATE TABLE users (
来源：http://byz.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kuz.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://bxt.kuanghao11.cn

email VARCHAR(100) UNIQUE,
来源：http://dco.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wej.cdnleiting.top

);
来源：http://uyx.haohaochexian.top

[Q02] 创建带外键的表
来源：http://hhi.yj20258.top

CREATE TABLE orders (
来源：http://fkn.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zjd.gaohongyu789.top

user_id INT NOT NULL,
来源：http://yek.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://fci.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aki.jiagoushi.top

);
来源：http://kbe.shanyushiyangtech.top

[Q03] 增加列
来源：http://jvq.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lhq.yfazqb.com

[Q04] 修改列类型
来源：http://ggd.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zma.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://akg.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wcq.gogol.net.cn

[Q06] 删除列
来源：http://hrk.sxryk.cn


<!-- 参考信息 -->