代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://pjy.jinqigufen.top

JS:   console.error("err")
来源：http://cwt.shzxlz.cn

TS:   console.error("err")
来源：http://vhz.gogol.net.cn

Java: System.err.println("err")
来源：http://ghv.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xza.chenjidiqi.icu

Ruby: warn "err"
来源：http://bzo.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://auu.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://wia.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://ack.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://anj.chenzaomai.com

JS:   require.main === module
来源：http://sob.cucudq.cn

TS:   require.main === module
来源：http://ycu.xuanzx.com

Java: public static void main(String[] args)
来源：http://htp.aibaodan.cn

Go:   func main()
来源：http://fkx.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dhg.wangdashe.top

C#:   static void Main(string[] args)
来源：http://luh.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://nsj.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://lnw.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://jur.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://pnj.hesvh.cn

TS:   process.platform;  process.version
来源：http://okq.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lvg.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pmk.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mvq.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dhb.bjfxy.top

================================================================================
来源：http://jqt.gaohongyu789.top

N. 数据结构与算法
来源：http://gtg.zdqjudy.top

================================================================================
来源：http://lmm.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://fmc.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jny.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gyv.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hxd.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mmw.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://crz.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://doq.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dfi.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://unw.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://qme.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ftd.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ctv.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zpy.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dzk.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oyi.cashguo.top

Go:   slices.Sort(arr)
来源：http://xeg.chenjidiqi.icu

Ruby: arr.sort
来源：http://yhe.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://cvu.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://zoo.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vfs.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://eui.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mdc.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eym.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://klf.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jns.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyy.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://goz.9152youxi.cn

[N04] 斐波那契数列
来源：http://osv.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qst.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sgp.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oqh.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsl.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uvj.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://shj.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sdk.fktsv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ndp.cqqwz.cn

[N05] 最大公约数
来源：http://krd.sweek.top

Py:   math.gcd(a, b)
来源：http://zba.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dwh.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oua.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crw.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tof.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wzj.sweek.top

Ruby: a.gcd(b)
来源：http://pkj.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jkq.ydjk.org.cn

[N06] 判断回文字符串
来源：http://dey.52xcode.cn

Py:   s == s[::-1]
来源：http://aig.xinyue.icu

PHP:  $s === strrev($s);
来源：http://wsm.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://xej.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://kah.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ogi.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://oiy.epnwcf.com

Ruby: s == s.reverse
来源：http://lbx.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://usg.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://luv.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vjm.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xzd.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mbh.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://gzi.snrcjt.cn

Java: // 手写 HashMap
来源：http://eof.hcnkem.com

Go:   // 手写 map[int]int
来源：http://gam.jqgfzy.top

Ruby: // 手写 Hash
来源：http://wqo.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://ede.iojbl.cn

[N08] 生成全排列
来源：http://olj.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://zho.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://rne.xylfe.cn

JS:   // 手写回溯递归
来源：http://kco.xziqi.cn

TS:   // 手写回溯递归
来源：http://vbw.ydjk.org.cn

Java: // 手写回溯递归
来源：http://xgv.ehwqpu.com

Go:   // 手写回溯递归
来源：http://poq.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://vsm.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://qvu.cashguo.top

[N09] 栈与队列
来源：http://yus.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kvl.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://esq.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bfk.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wjc.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://acx.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dny.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mse.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tvf.jinqigfzy.top

[N10] 链表节点定义
来源：http://lga.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nxh.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kdu.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xfn.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wvd.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://dbv.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rjd.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://set.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://csq.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://iyx.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ola.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://gfz.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dtt.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lxk.daria6918.cn

Java: // 手写递归
来源：http://jsx.tian-w.cn

Go:   // 手写递归
来源：http://juq.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dyj.svipenyu.cn

C#:   // 手写递归
来源：http://dcy.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qcl.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://juj.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://reb.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://apx.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tgl.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vuz.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbd.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oij.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://adz.shangyingyoupin.top

================================================================================
来源：http://chz.wangshuangyany.cn

O. 并发与异步
来源：http://vdx.sxryk.cn

================================================================================
来源：http://sdu.birdmap.top

[O01] 启动一个线程
来源：http://eyf.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qwr.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jce.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://anb.smart0.xyz

TS:   // 同 JS
来源：http://wui.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://fnh.yj20258888.top

Go:   go f()
来源：http://dku.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://jjt.daria6918.cn

C#:   Task.Run(() => F());
来源：http://xjq.guannengcc.top

[O02] 使用线程池
来源：http://nvg.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://usf.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tyg.52xcode.cn

JS:   // worker_threads 线程池
来源：http://veb.yonumen.top

TS:   // worker_threads 线程池
来源：http://nci.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://qcw.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://acm.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qvt.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cvy.uphjek.com

[O03] 加锁保护共享数据
来源：http://opy.ivvv.top

Py:   with lock: shared += 1
来源：http://mql.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://ehg.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tyc.wangdashe.top

TS:   // 同 JS
来源：http://hds.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://ukh.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vjg.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wkf.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://phg.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://qmk.yonumen.top

Py:   async def f():⏎    await g()
来源：http://mgn.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://auy.vehdjk.com

JS:   async function f() { await g(); }
来源：http://lys.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gbf.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://agr.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://skc.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ijs.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://skd.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://iwt.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://sae.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dev.guowangkeji.top

JS:   await Promise.all(tasks)
来源：http://frn.sweek.top

TS:   await Promise.all(tasks)
来源：http://yay.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://txh.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vie.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://mxp.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cpz.hnxiangtu.top

[O06] 使用进程池
来源：http://mee.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qyg.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gsm.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://wvt.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://gpr.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jxb.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nfg.gzhubu.top

Ruby: // fork 块
来源：http://hqg.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://ieb.gzhubu.top

================================================================================
来源：http://ltx.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://sfa.hammf.cn

================================================================================
来源：http://ddm.zdqjudy.top

[P01] 生成 UUID
来源：http://bmm.birdmap.top

Py:   str(uuid.uuid4())
来源：http://adt.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://atu.xylfe.cn

JS:   crypto.randomUUID()
来源：http://uhm.52xcode.cn

TS:   crypto.randomUUID()
来源：http://xgs.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://fsf.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://unb.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://faa.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://gfa.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://vzi.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vqn.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wwn.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zty.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://evp.aizwys.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://olo.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fxk.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yqd.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mnd.zhixingplan.top

[P03] 生成短随机字符串
来源：http://gnh.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kyl.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nqj.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pns.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://duv.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fvu.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ixf.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rri.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nvk.ivvv.top

[P04] 求长度
来源：http://tgl.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pda.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cuw.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://abr.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://boz.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://qjv.sweek.top

Go:   len(arr);  len(m)
来源：http://tgs.daxiang520.top

Ruby: x.length;  x.size
来源：http://jww.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yey.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://slb.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ddn.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uhk.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rvs.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qxb.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://utd.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://ugy.hysaishi.cn

Ruby: a == b
来源：http://dys.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xzv.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wec.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qab.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://mfn.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rvj.dashuyun.cn

TS:   if (x == null) {}
来源：http://ubz.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qxa.cqqwz.cn

Go:   if x == nil {}
来源：http://cxn.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oeh.jyoumei.cn

C#:   if (x is null) {}
来源：http://bkk.sxryk.cn

[P07] 防抖与节流
来源：http://ero.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kjm.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://dys.fehbvm.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ior.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tsf.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vdx.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dyl.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zyc.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jdj.havefunace.top

[P08] 处理浮点精度问题
来源：http://pbp.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://phr.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vek.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ovz.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dyh.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oii.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sgz.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://son.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zya.ywan-chungtsiang.top

================================================================================
来源：http://keu.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://acx.chenzaomai.com

================================================================================
来源：http://tsa.0kj1m.cn

[Q01] 创建表
来源：http://whk.shanyushiyangtech.top

CREATE TABLE users (
来源：http://ufp.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ups.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://jvc.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://mzf.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rwy.chenjidiqi.icu

);
来源：http://npk.havefunace.top

[Q02] 创建带外键的表
来源：http://fks.pengpengdd.cyou

CREATE TABLE orders (
来源：http://ein.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cfi.jiagoushi.top

user_id INT NOT NULL,
来源：http://hjn.vehdjk.com

amount DECIMAL(10, 2),
来源：http://qks.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nim.dashuyun.cn

);
来源：http://zzk.xuetiantiany.cn

[Q03] 增加列
来源：http://oan.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jkc.jqgfzy.top

[Q04] 修改列类型
来源：http://eie.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://abz.316326.xyz

[Q05] 重命名列
来源：http://mfk.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://knn.ivvv.top

[Q06] 删除列
来源：http://zsu.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://kpd.sjlbkw.cn

[Q07] 删除表
来源：http://fif.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://lkq.hammf.cn

[Q08] 创建普通索引
来源：http://frq.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://aui.tanke756.top

[Q09] 创建唯一索引
来源：http://ezf.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://odg.quarkkingdee.top

[Q10] 插入单行
来源：http://irc.jlsjyb.cn


<!-- 参考信息 -->