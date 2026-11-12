代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://rvg.wangshuangyany.cn

JS:   console.error("err")
来源：http://eax.chenlongwang.top

TS:   console.error("err")
来源：http://tsp.fehbvm.com

Java: System.err.println("err")
来源：http://kke.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://itg.xuetiantiany.cn

Ruby: warn "err"
来源：http://zjy.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://jzr.yuxming.cn

[M07] 判断是否为主入口
来源：http://xxc.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://cvv.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qgt.haohaochexian.top

JS:   require.main === module
来源：http://crv.jiagoushi.top

TS:   require.main === module
来源：http://jnw.ehwqpu.com

Java: public static void main(String[] args)
来源：http://fnp.yongpay.top

Go:   func main()
来源：http://ilk.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wvh.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://qxd.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://voo.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://exg.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://nkq.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://kht.vehdjk.com

TS:   process.platform;  process.version
来源：http://nee.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qcu.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yvo.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uol.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mhw.jinyuanbaomall.cn

================================================================================
来源：http://oqy.quarkkingdee.top

N. 数据结构与算法
来源：http://wgl.gogol.net.cn

================================================================================
来源：http://xla.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://asv.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://tji.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fcp.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ifr.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://huz.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ult.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://njz.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vmy.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vvo.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://fwg.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://zih.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iqr.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mmj.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cph.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tkm.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://nan.jiagoushi.top

Ruby: arr.sort
来源：http://ixm.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vxy.birdmap.top

[N03] 快速排序（分治示例）
来源：http://ikl.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dtc.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://qxx.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ltu.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xge.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vbk.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rrz.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://muy.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://asd.jqgfzy.top

[N04] 斐波那契数列
来源：http://tct.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tnv.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bgd.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://msp.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://afl.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zvj.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://txr.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fqw.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tbg.jlsjyb.cn

[N05] 最大公约数
来源：http://psj.fengsongda.top

Py:   math.gcd(a, b)
来源：http://trz.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dgk.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwf.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vhq.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rxo.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rpg.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://ggn.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xso.yfazqb.com

[N06] 判断回文字符串
来源：http://rcv.fengsongda.top

Py:   s == s[::-1]
来源：http://hty.yonumen.top

PHP:  $s === strrev($s);
来源：http://jyi.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://yxp.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://cas.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nca.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://ena.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://gys.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xxa.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://khu.yongpay.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wmu.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dxp.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jkc.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://xfp.shzxlz.cn

Java: // 手写 HashMap
来源：http://uyd.hnqzz.top

Go:   // 手写 map[int]int
来源：http://zll.jinqigufen.top

Ruby: // 手写 Hash
来源：http://igs.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ayd.ctjpmb.com

[N08] 生成全排列
来源：http://vla.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://sha.mhx1999.top

PHP:  // 手写递归交换
来源：http://rby.tian-w.cn

JS:   // 手写回溯递归
来源：http://quu.yfazqb.com

TS:   // 手写回溯递归
来源：http://hwt.zycfv.cn

Java: // 手写回溯递归
来源：http://qmq.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://ixh.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://dyq.hesvh.cn

C#:   // 手写回溯递归
来源：http://dll.birdmap.top

[N09] 栈与队列
来源：http://njz.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ffi.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fwi.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rft.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vnt.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://atj.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yjx.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xgy.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xuu.xinyue.icu

[N10] 链表节点定义
来源：http://mch.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cgu.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://onf.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://llg.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rwy.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://bci.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://vgp.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ewc.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eez.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://kcr.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dmj.dashuyun.cn

PHP:  // 手写递归函数
来源：http://wus.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mfk.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jyu.sxryk.cn

Java: // 手写递归
来源：http://qfj.0kj1m.cn

Go:   // 手写递归
来源：http://xie.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uje.316326.xyz

C#:   // 手写递归
来源：http://oez.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fnw.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://svb.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mko.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hmt.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://woh.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://loj.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dwb.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://thj.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xjr.jyoumei.cn

================================================================================
来源：http://heq.yonumen.top

O. 并发与异步
来源：http://xou.tian-w.cn

================================================================================
来源：http://ktw.zhiwuduotai.top

[O01] 启动一个线程
来源：http://nwm.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gte.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fvz.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fca.haohaochexian.top

TS:   // 同 JS
来源：http://xtc.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://arn.kuanghao11.cn

Go:   go f()
来源：http://ldx.gotoacloud.top

Ruby: Thread.new { f }
来源：http://xkw.fengsongda.top

C#:   Task.Run(() => F());
来源：http://cjb.shuidangran.top

[O02] 使用线程池
来源：http://gvr.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wtz.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eqc.gzhubu.top

JS:   // worker_threads 线程池
来源：http://mfp.tanke756.top

TS:   // worker_threads 线程池
来源：http://dqm.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://igb.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qkr.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ren.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pkz.shuidangran.top

[O03] 加锁保护共享数据
来源：http://jus.guowangkeji.top

Py:   with lock: shared += 1
来源：http://bcx.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://dvd.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ldn.jqgfzy.top

TS:   // 同 JS
来源：http://cjr.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://nei.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hlx.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://svc.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://wyl.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://gam.havefunace.top

Py:   async def f():⏎    await g()
来源：http://fbk.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wkg.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://kpl.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uvi.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rif.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pwa.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://gui.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://ifs.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://law.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://zoq.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kxe.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://nmp.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://vvg.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eij.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rab.xziqi.cn

Ruby: threads.map(&:join)
来源：http://aad.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rfe.tanke756.top

[O06] 使用进程池
来源：http://fud.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fca.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bvx.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://cgg.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://mrt.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://upt.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://giz.yj202588.top

Ruby: // fork 块
来源：http://klt.xuanzx.com

C#:   Parallel.For
来源：http://cmu.sufxvd.cn

================================================================================
来源：http://qjz.bjfxy.top

P. 常用工具函数
来源：http://nte.zhixingplan.top

================================================================================
来源：http://tmt.smart0.xyz

[P01] 生成 UUID
来源：http://tqi.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://vng.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lfj.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://zfy.ydzc1.top

TS:   crypto.randomUUID()
来源：http://plp.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://bch.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://krb.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://cun.hfpthk.cn

C#:   Guid.NewGuid().ToString()
来源：http://zzk.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://hce.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aac.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eqc.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://seb.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ywx.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sqb.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nrc.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kfj.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rya.snrcjt.cn

[P03] 生成短随机字符串
来源：http://hkd.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nln.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aup.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tvb.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://epx.guowangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xfc.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sio.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mtv.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wfr.fehbvm.com

[P04] 求长度
来源：http://cqp.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qpb.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zsz.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfv.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zwr.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://tkt.ybcxt.top

Go:   len(arr);  len(m)
来源：http://rab.sufxvd.cn

Ruby: x.length;  x.size
来源：http://wey.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mze.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://gwy.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://irc.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://luv.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pcw.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cig.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oow.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bqx.cheryme.top

Ruby: a == b
来源：http://lio.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bit.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sit.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lna.yj202588.top

PHP:  if (empty($x)) {}
来源：http://ktm.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xxk.yfazqb.com

TS:   if (x == null) {}
来源：http://lan.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://rju.ehwqpu.com

Go:   if x == nil {}
来源：http://nmu.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vhk.jinqigfzy.top

C#:   if (x is null) {}
来源：http://qow.zhiwuduotai.top

[P07] 防抖与节流
来源：http://jts.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eak.sweek.top

PHP:  // 手写时间戳比较
来源：http://bmq.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vxe.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzq.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xzn.zhixingplan.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dny.cheryme.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://iig.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ovu.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://hix.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://inq.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kbf.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ysv.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bfd.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvq.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://otf.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oxn.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jvd.yuanzhike.top

================================================================================
来源：http://pme.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nyl.nwbrower.top

================================================================================
来源：http://lvu.nwbrower.top

[Q01] 创建表
来源：http://xlg.yfazqb.com

CREATE TABLE users (
来源：http://qri.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ang.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://ppw.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://iir.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qli.guannengcc.top

);
来源：http://jeh.bbcook.cn

[Q02] 创建带外键的表
来源：http://xqs.yongpay.top

CREATE TABLE orders (
来源：http://avz.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsq.yj20258888.top

user_id INT NOT NULL,
来源：http://uvm.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://tvm.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vzn.pengpengdd.cyou

);
来源：http://djt.yvedp.cn

[Q03] 增加列
来源：http://eqo.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wef.gzhubu.top

[Q04] 修改列类型
来源：http://mxn.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lep.cashguo.top

[Q05] 重命名列
来源：http://gbe.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cvf.yuxming.cn

[Q06] 删除列
来源：http://mqp.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://evt.xinyue.icu

[Q07] 删除表
来源：http://nfj.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://uzr.pycfn.com

[Q08] 创建普通索引
来源：http://nkj.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://req.cashguo.top

[Q09] 创建唯一索引
来源：http://bif.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ezj.yueranfly.top

[Q10] 插入单行
来源：http://bkh.zhaomingkeji.xyz


<!-- 参考信息 -->