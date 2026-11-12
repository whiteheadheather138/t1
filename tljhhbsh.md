代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://tuw.xylfe.cn

[M05] 设置退出码
来源：http://ilb.fengsongda.top

Py:   sys.exit(1)
来源：http://edf.cheryme.top

PHP:  exit(1);
来源：http://aws.yj202588.top

JS:   process.exit(1)
来源：http://baq.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://ktd.xuanzx.com

Java: System.exit(1)
来源：http://twb.nwbrower.top

Go:   os.Exit(1)
来源：http://mwb.hnxiangtu.top

Ruby: exit 1
来源：http://jyt.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dsu.hcnkem.com

[M06] 向标准错误输出
来源：http://wew.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://eki.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ybi.fengsongda.top

JS:   console.error("err")
来源：http://dnk.ivvv.top

TS:   console.error("err")
来源：http://ajh.ppjwa.cn

Java: System.err.println("err")
来源：http://lir.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pmq.cqqwz.cn

Ruby: warn "err"
来源：http://ykt.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://uxf.gogol.net.cn

[M07] 判断是否为主入口
来源：http://tut.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://uiw.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfc.jinqigfzy.top

JS:   require.main === module
来源：http://dup.iojbl.cn

TS:   require.main === module
来源：http://xxq.yuxming.cn

Java: public static void main(String[] args)
来源：http://axd.sxryk.cn

Go:   func main()
来源：http://wrw.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pcz.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://nwk.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://arn.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://ozr.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://ddl.zhengqikj.top

JS:   process.platform;  process.version
来源：http://znt.jinqigufen.top

TS:   process.platform;  process.version
来源：http://ifd.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://brz.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fhy.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vbc.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://opw.sweek.top

================================================================================
来源：http://mmh.snrcjt.cn

N. 数据结构与算法
来源：http://gif.wangdashe.top

================================================================================
来源：http://xmd.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://wyg.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://sar.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zej.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ooo.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oog.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pot.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://akw.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://faz.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://qgf.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://uxc.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://nvk.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jtd.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://tvp.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lcw.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://csq.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://kcs.shzxlz.cn

Ruby: arr.sort
来源：http://xvk.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pnd.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://ovb.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ckp.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://phn.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gtg.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://glr.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yry.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://snl.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hky.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://zhr.hfpthk.cn

[N04] 斐波那契数列
来源：http://njg.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vig.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yei.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvn.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://url.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xub.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ipx.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vta.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fms.sjlbkw.cn

[N05] 最大公约数
来源：http://vjz.fzhhl.top

Py:   math.gcd(a, b)
来源：http://xag.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tcy.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpi.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rlc.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://svh.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kbj.fengsongda.top

Ruby: a.gcd(b)
来源：http://cas.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uqf.jinqigufen.top

[N06] 判断回文字符串
来源：http://jtb.sysykeji.top

Py:   s == s[::-1]
来源：http://lry.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://lzn.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://zqw.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://tnp.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tqe.sysykeji.top

Go:   // 双指针从两端比较
来源：http://zut.tarul.cn

Ruby: s == s.reverse
来源：http://euo.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pla.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://kxr.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jbw.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pjh.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eru.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://gvk.52xcode.cn

Java: // 手写 HashMap
来源：http://ven.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://cdp.vehdjk.com

Ruby: // 手写 Hash
来源：http://svb.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://cne.dianchejie.cn

[N08] 生成全排列
来源：http://lfu.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://wfp.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://acj.hfpthk.cn

JS:   // 手写回溯递归
来源：http://qnt.chenlongwang.top

TS:   // 手写回溯递归
来源：http://nal.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://iyp.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://xik.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://sdi.zhixingplan.top

C#:   // 手写回溯递归
来源：http://rpv.gaohongyu789.top

[N09] 栈与队列
来源：http://oex.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mkh.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wel.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://auy.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ywo.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://psb.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xgr.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rvm.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://onk.yj202588.top

[N10] 链表节点定义
来源：http://bsp.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oox.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://fdp.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rpn.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mra.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://qgc.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://ukx.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ksb.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kwi.nwbrower.top

[N11] 二叉树中序遍历
来源：http://buy.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dbx.ydzc1.top

PHP:  // 手写递归函数
来源：http://lxt.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://drv.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sfq.bbcook.cn

Java: // 手写递归
来源：http://nyg.kuanghao11.cn

Go:   // 手写递归
来源：http://mdq.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nki.svipenyu.cn

C#:   // 手写递归
来源：http://wwv.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qtt.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://src.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tss.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://grx.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wdw.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wwf.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dko.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ndc.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://psl.zdqjudy.top

================================================================================
来源：http://xag.gzhubu.top

O. 并发与异步
来源：http://uzr.mhx1999.top

================================================================================
来源：http://grx.havefunace.top

[O01] 启动一个线程
来源：http://vre.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wnq.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fbg.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hhh.quarkkingdee.top

TS:   // 同 JS
来源：http://yrj.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://csx.ppjwa.cn

Go:   go f()
来源：http://oyb.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://nxs.yj20258888.top

C#:   Task.Run(() => F());
来源：http://iwk.shzxlz.cn

[O02] 使用线程池
来源：http://nsq.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dni.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://amk.316326.xyz

JS:   // worker_threads 线程池
来源：http://dok.jyoumei.cn

TS:   // worker_threads 线程池
来源：http://zeb.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rrj.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qyk.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hew.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ayf.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://itu.jianghu66.top

Py:   with lock: shared += 1
来源：http://enp.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://ppv.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ied.yongpay.top

TS:   // 同 JS
来源：http://krn.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://xkp.ydzc1.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ggg.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://muv.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://stg.cashguo.top

[O04] 定义异步函数并等待
来源：http://glp.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://qsz.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lua.yfazqb.com

JS:   async function f() { await g(); }
来源：http://rel.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://ywv.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qtw.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://reo.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://wbg.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://lzo.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://yxp.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://bvi.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lgt.tanke756.top

JS:   await Promise.all(tasks)
来源：http://uok.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://wmr.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pdn.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://epi.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://zbx.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://qkc.hnxiangtu.top

[O06] 使用进程池
来源：http://uag.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmo.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uaf.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://asu.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://riv.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gkv.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rlh.mhx1999.top

Ruby: // fork 块
来源：http://gxk.jinghuilouyu.cn

C#:   Parallel.For
来源：http://cfh.cqqwz.cn

================================================================================
来源：http://kpf.vqdsnc.cn

P. 常用工具函数
来源：http://jyq.fktsv.cn

================================================================================
来源：http://far.redwolf501.top

[P01] 生成 UUID
来源：http://djg.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://bov.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://icj.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://adh.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://idc.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://cpf.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://yvz.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://bit.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://fzd.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://lxu.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ydx.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bjk.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://msw.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lhx.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cdu.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uqh.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://txt.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wxp.cqqwz.cn

[P03] 生成短随机字符串
来源：http://akh.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tau.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gcp.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://phc.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jwn.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rdb.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lko.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xtu.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://saq.cheryme.top

[P04] 求长度
来源：http://nry.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ioy.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tph.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rdi.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ooz.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://vwp.yuxming.cn

Go:   len(arr);  len(m)
来源：http://ujn.yj20258888.top

Ruby: x.length;  x.size
来源：http://kgu.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vvd.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://ufx.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jcd.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zrd.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vmr.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bdk.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fsr.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fwp.jqgufenzy.top

Ruby: a == b
来源：http://lut.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nye.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://igp.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zpb.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://etm.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pja.andypj.xyz

TS:   if (x == null) {}
来源：http://aby.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zpa.xziqi.cn

Go:   if x == nil {}
来源：http://gpx.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qel.tian-w.cn

C#:   if (x is null) {}
来源：http://eeq.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://nmb.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fzt.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://gxc.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ugx.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aks.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xml.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jyk.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gkr.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xdc.gzhubu.top

[P08] 处理浮点精度问题
来源：http://jge.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lfr.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qjd.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ael.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ljv.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qvp.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dkt.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywn.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fgz.fanxiaobao.xyz

================================================================================
来源：http://emp.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uug.tanke756.top

================================================================================
来源：http://ycl.meibo888.top

[Q01] 创建表
来源：http://lrs.yueranfly.top

CREATE TABLE users (
来源：http://bfo.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ico.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://rsk.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://orf.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qbx.pengpengdd.cyou

);
来源：http://zuz.haohaochexian.top

[Q02] 创建带外键的表
来源：http://ltu.gotoacloud.top

CREATE TABLE orders (
来源：http://hxs.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qsa.epnwcf.com

user_id INT NOT NULL,
来源：http://eac.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://gdt.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://beo.nanxuanxn.top

);
来源：http://rmf.xinyue.icu

[Q03] 增加列
来源：http://axe.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zjz.vqdsnc.cn

[Q04] 修改列类型
来源：http://hzn.ywan-chungtsiang.top


<!-- 参考信息 -->