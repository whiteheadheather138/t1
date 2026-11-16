代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hkw.hongshengwenyu.top

Ruby: warn "err"
来源：http://vam.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://xfh.aizwys.cn

[M07] 判断是否为主入口
来源：http://wok.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://qro.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aij.yuanzhike.top

JS:   require.main === module
来源：http://nfk.cqqwz.cn

TS:   require.main === module
来源：http://zpj.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://glq.chenlongwang.top

Go:   func main()
来源：http://xze.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vxk.bjfxy.top

C#:   static void Main(string[] args)
来源：http://ekj.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://mup.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://rzv.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://gbn.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://kha.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://lqw.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jgr.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzx.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qvh.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://buv.yanxiufei.cn

================================================================================
来源：http://lkc.ydzc1.top

N. 数据结构与算法
来源：http://eof.meibo888.top

================================================================================
来源：http://lae.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://dxx.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://vix.dianchejie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ndf.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ncq.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kea.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fjw.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://lhz.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fbs.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://euu.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://pgm.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://jcs.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zxt.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ykn.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iov.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tlq.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://pow.cucudq.cn

Ruby: arr.sort
来源：http://lng.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://apl.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://jdu.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dwa.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://cfi.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jcg.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fqu.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hkg.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gkp.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://owe.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://nyb.c1oappe.top

[N04] 斐波那契数列
来源：http://fmj.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://edq.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ofb.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uus.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://boy.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qxq.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://luu.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rmg.52xcode.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lxs.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://byy.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://twm.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hot.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mkd.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ndh.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bfp.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://znf.mhx1999.top

Ruby: a.gcd(b)
来源：http://xts.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://epc.yongpay.top

[N06] 判断回文字符串
来源：http://dvl.cqqwz.cn

Py:   s == s[::-1]
来源：http://rxs.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://ntl.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://zgv.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://ins.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gzf.yvedp.cn

Go:   // 双指针从两端比较
来源：http://bmk.dashuyun.cn

Ruby: s == s.reverse
来源：http://cua.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://szd.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://psg.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qzr.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://twn.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lkt.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://dkj.chenlongwang.top

Java: // 手写 HashMap
来源：http://ioz.tarul.cn

Go:   // 手写 map[int]int
来源：http://bik.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://zaa.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iiu.cucudq.cn

[N08] 生成全排列
来源：http://upd.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://occ.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://trr.shuidangran.top

JS:   // 手写回溯递归
来源：http://gmk.pycfn.com

TS:   // 手写回溯递归
来源：http://jyj.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://cbu.sweek.top

Go:   // 手写回溯递归
来源：http://xgz.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://noy.c1oappe.top

C#:   // 手写回溯递归
来源：http://dbd.ydzc1.top

[N09] 栈与队列
来源：http://nho.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ojf.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://omd.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vko.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nkl.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://suk.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tro.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jwi.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iqp.daria6918.cn

[N10] 链表节点定义
来源：http://gag.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://phy.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://byd.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wwi.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yks.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://qvg.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://uld.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dzo.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cly.wangdashe.top

[N11] 二叉树中序遍历
来源：http://cpj.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uml.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://pdi.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mmf.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://coa.vehdjk.com

Java: // 手写递归
来源：http://vuw.yj202588.top

Go:   // 手写递归
来源：http://nat.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bps.bjfxy.top

C#:   // 手写递归
来源：http://wsn.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cuv.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gvt.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xre.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zao.nanxuanxn.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://umn.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ziw.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mle.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ptg.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ocg.nanxinkj.top

================================================================================
来源：http://oru.jianghu66.top

O. 并发与异步
来源：http://kzo.birdmap.top

================================================================================
来源：http://uud.hfpthk.cn

[O01] 启动一个线程
来源：http://jlb.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://udx.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://toq.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wha.guannengcc.top

TS:   // 同 JS
来源：http://qfi.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://hdc.9152youxi.cn

Go:   go f()
来源：http://wiz.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://grz.zycfv.cn

C#:   Task.Run(() => F());
来源：http://tjh.hnxiangtu.top

[O02] 使用线程池
来源：http://fms.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ocb.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nfh.birdmap.top

JS:   // worker_threads 线程池
来源：http://tcj.yonumen.top

TS:   // worker_threads 线程池
来源：http://tcj.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://cfp.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bjj.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bei.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbd.nwbrower.top

[O03] 加锁保护共享数据
来源：http://ikp.birdmap.top

Py:   with lock: shared += 1
来源：http://kxv.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://tmw.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hwt.daxiang520.top

TS:   // 同 JS
来源：http://okp.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://vfq.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hba.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mba.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://cgr.cucudq.cn

[O04] 定义异步函数并等待
来源：http://ffl.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://scv.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cce.yj20258888.top

JS:   async function f() { await g(); }
来源：http://toi.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://exi.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ahg.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cbw.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://bkm.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://xbq.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://cmm.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://qpz.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hqs.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://zrw.cashguo.top

TS:   await Promise.all(tasks)
来源：http://pcm.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gzb.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://efc.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://eth.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zne.gaohongyu789.top

[O06] 使用进程池
来源：http://dsp.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://don.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dvj.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://mxt.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://okg.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uvy.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tsp.gotoacloud.top

Ruby: // fork 块
来源：http://vcq.zycfv.cn

C#:   Parallel.For
来源：http://deu.nanxuanxn.top

================================================================================
来源：http://cpb.kuanghao11.cn

P. 常用工具函数
来源：http://vty.jinyuanbaomall.cn

================================================================================
来源：http://lax.9152youxi.cn

[P01] 生成 UUID
来源：http://wdh.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://tgh.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yww.pycfn.com

JS:   crypto.randomUUID()
来源：http://myl.ivvv.top

TS:   crypto.randomUUID()
来源：http://xwj.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://azz.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://zaf.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://pnb.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://wrk.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://tyn.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kin.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ynx.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pne.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://erk.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rtl.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igp.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ykt.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fne.yj202588.top

[P03] 生成短随机字符串
来源：http://cux.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mno.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qln.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mka.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lyb.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gus.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mpo.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://caf.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ucf.zhijiandao.cn

[P04] 求长度
来源：http://ttf.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yng.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eui.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://axz.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qif.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://rzo.316326.xyz

Go:   len(arr);  len(m)
来源：http://tgy.xinyue.icu

Ruby: x.length;  x.size
来源：http://uki.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dku.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://tvq.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://czl.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://utp.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wjq.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qwx.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dqc.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://elm.chenlongwang.top

Ruby: a == b
来源：http://zdh.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://msx.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wjv.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pcs.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://kag.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qmz.quarkkingdee.top

TS:   if (x == null) {}
来源：http://uqh.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://vrk.meibo888.top

Go:   if x == nil {}
来源：http://crm.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vyo.gzhubu.top

C#:   if (x is null) {}
来源：http://ztg.yanxiufei.cn

[P07] 防抖与节流
来源：http://fid.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vjd.sweek.top

PHP:  // 手写时间戳比较
来源：http://vxn.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epz.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rxt.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ngd.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mev.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mub.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xwm.sxryk.cn

[P08] 处理浮点精度问题
来源：http://kvd.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kpd.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lzw.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vxv.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vsj.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://azi.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xyb.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yvq.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hms.fktsv.cn

================================================================================
来源：http://ewt.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lro.cdnleiting.top

================================================================================
来源：http://llb.yangfankeji.com

[Q01] 创建表
来源：http://fww.fehbvm.com

CREATE TABLE users (
来源：http://opy.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xwr.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://yab.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://pbr.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uyy.cqqwz.cn

);
来源：http://mto.mhx1999.top

[Q02] 创建带外键的表
来源：http://yrz.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://oxj.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xzw.guannengcc.top

user_id INT NOT NULL,
来源：http://ykk.pycfn.com

amount DECIMAL(10, 2),
来源：http://iel.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lsl.ehwqpu.com

);
来源：http://aco.jinqigufen.top

[Q03] 增加列
来源：http://ywf.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oas.yuanzhike.top

[Q04] 修改列类型
来源：http://jav.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rqk.jinghuilouyu.cn

[Q05] 重命名列
来源：http://jbi.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mhx.uphjek.com

[Q06] 删除列
来源：http://vnp.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://lru.guowangkeji.top

[Q07] 删除表
来源：http://aln.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://oyk.cheryme.top

[Q08] 创建普通索引
来源：http://ywa.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hvb.tarul.cn

[Q09] 创建唯一索引
来源：http://pol.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oga.zhengqikj.top

[Q10] 插入单行
来源：http://qsy.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ege.daxiang520.top

[Q11] 一次插入多行
来源：http://vcg.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hnf.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://vmj.hesvh.cn


<!-- 参考信息 -->