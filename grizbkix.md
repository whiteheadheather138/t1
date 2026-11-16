代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://ucz.hfpthk.cn

JS:   console.error("err")
来源：http://vxf.kuanghao11.cn

TS:   console.error("err")
来源：http://eyz.zdqjudy.top

Java: System.err.println("err")
来源：http://wes.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gpg.bbcook.cn

Ruby: warn "err"
来源：http://swr.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://wpa.ydzc1.top

[M07] 判断是否为主入口
来源：http://arr.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://unt.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yxf.svipenyu.cn

JS:   require.main === module
来源：http://ppz.cheryme.top

TS:   require.main === module
来源：http://rqx.birdmap.top

Java: public static void main(String[] args)
来源：http://eso.gotoacloud.top

Go:   func main()
来源：http://asg.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wuk.hammf.cn

C#:   static void Main(string[] args)
来源：http://amy.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://gfa.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://xcb.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://gbd.cheryme.top

JS:   process.platform;  process.version
来源：http://gif.shuidangran.top

TS:   process.platform;  process.version
来源：http://pno.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bhc.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zht.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hpz.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gag.ydjk.org.cn

================================================================================
来源：http://tlz.tianlin.xyz

N. 数据结构与算法
来源：http://cbq.52xcode.cn

================================================================================
来源：http://qxu.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://vhu.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kyb.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lls.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zca.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nhi.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fpj.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://xsm.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jvx.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://aws.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://wtd.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://sht.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://snn.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qbt.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://faf.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dbi.bjfxy.top

Go:   slices.Sort(arr)
来源：http://piz.hnqzz.top

Ruby: arr.sort
来源：http://zls.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ykl.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://moq.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://chk.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://yzn.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mpb.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bqf.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xvk.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://roc.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gea.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://qfc.jiagoushi.top

[N04] 斐波那契数列
来源：http://oti.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ocn.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xag.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bbd.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nzc.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://stu.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lpk.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ttk.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uem.yuanzhike.top

[N05] 最大公约数
来源：http://ubr.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://skh.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ysk.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrj.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugw.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eur.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nul.hfpthk.cn

Ruby: a.gcd(b)
来源：http://fae.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bxj.tanke756.top

[N06] 判断回文字符串
来源：http://evl.vehdjk.com

Py:   s == s[::-1]
来源：http://xtz.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://mqg.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://wfe.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://hnm.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pfj.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://mqg.yueranfly.top

Ruby: s == s.reverse
来源：http://glo.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ihv.cashguo.top

[N07] 两数之和（返回下标）
来源：http://ukn.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://guf.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://swg.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ppa.sweek.top

TS:   // 手写 Map<string, number>
来源：http://nxx.zhongyouzk.top

Java: // 手写 HashMap
来源：http://kvo.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://mwy.hfpthk.cn

Ruby: // 手写 Hash
来源：http://hqe.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://spn.chenlongwang.top

[N08] 生成全排列
来源：http://yut.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://cec.chenlongwang.top

PHP:  // 手写递归交换
来源：http://mce.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://mna.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://oiu.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://alq.xziqi.cn

Go:   // 手写回溯递归
来源：http://kuq.svipenyu.cn

Ruby: arr.permutation.to_a
来源：http://ymg.yfazqb.com

C#:   // 手写回溯递归
来源：http://fbe.cashguo.top

[N09] 栈与队列
来源：http://zde.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yhp.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://haf.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gdq.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rvs.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dqd.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ctu.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jkp.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://syv.c1oappe.top

[N10] 链表节点定义
来源：http://sqb.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nyb.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sjm.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://abk.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ezn.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://dyd.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://jtv.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ozz.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yyd.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://rrp.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bvi.sufxvd.cn

PHP:  // 手写递归函数
来源：http://fmv.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbl.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ets.andypj.xyz

Java: // 手写递归
来源：http://gev.gogol.net.cn

Go:   // 手写递归
来源：http://sse.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://diq.sufxvd.cn

C#:   // 手写递归
来源：http://jdv.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oeu.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ldf.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://des.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vqx.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvp.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sgd.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://izd.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjs.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nbo.jqgfzy.top

================================================================================
来源：http://gqa.epnwcf.com

O. 并发与异步
来源：http://jbo.hfpthk.cn

================================================================================
来源：http://ubk.fehbvm.com

[O01] 启动一个线程
来源：http://izo.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bwc.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rke.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kem.zhijiandao.cn

TS:   // 同 JS
来源：http://ldq.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://kfv.zhaomingkeji.xyz

Go:   go f()
来源：http://fuj.tanke756.top

Ruby: Thread.new { f }
来源：http://yqx.redwolf501.top

C#:   Task.Run(() => F());
来源：http://elz.ehwqpu.com

[O02] 使用线程池
来源：http://gjb.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tyi.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uhr.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://woj.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://zzq.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://mmw.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://saa.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uiu.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bce.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://dow.52xcode.cn

Py:   with lock: shared += 1
来源：http://gkg.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://xou.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://brj.jianghu66.top

TS:   // 同 JS
来源：http://rxm.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://tkc.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pzs.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://emn.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://ipx.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://hyt.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://csi.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zgk.xinyue.icu

JS:   async function f() { await g(); }
来源：http://pms.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uec.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jxz.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cjf.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://ree.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://ecg.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://cnp.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://thy.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://osx.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://zdt.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://ccq.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hlt.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ypj.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://qyo.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gqt.cashguo.top

[O06] 使用进程池
来源：http://kod.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kwx.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jvw.tanke756.top

JS:   // child_process / cluster 模块
来源：http://muk.cashguo.top

TS:   // child_process / cluster 模块
来源：http://cdy.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://egn.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vkz.hysaishi.cn

Ruby: // fork 块
来源：http://jih.hysaishi.cn

C#:   Parallel.For
来源：http://vmo.hnxiangtu.top

================================================================================
来源：http://hrx.guowangkeji.top

P. 常用工具函数
来源：http://qdo.birdmap.top

================================================================================
来源：http://cpc.ppjwa.cn

[P01] 生成 UUID
来源：http://cbf.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://ldn.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cum.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://qae.sysykeji.top

TS:   crypto.randomUUID()
来源：http://cvj.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://ukj.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://lnx.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://ilq.nanxinkj.top

C#:   Guid.NewGuid().ToString()
来源：http://qij.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://bzb.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vba.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pmh.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xwx.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gta.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hwy.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iti.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lvd.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://akp.gogol.net.cn

[P03] 生成短随机字符串
来源：http://fqm.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fic.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pqx.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://thc.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekf.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lyy.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mvw.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mcb.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dey.yonumen.top

[P04] 求长度
来源：http://bfs.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://flq.havefunace.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rdl.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kfn.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcy.cucudq.cn

Java: list.size();  map.size();  s.length()
来源：http://yxw.ydzc1.top

Go:   len(arr);  len(m)
来源：http://pza.fengsongda.top

Ruby: x.length;  x.size
来源：http://ytu.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rni.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://gqv.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ywq.yongpay.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jfm.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kfl.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ieq.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cjm.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yeo.mhx1999.top

Ruby: a == b
来源：http://sxg.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pfe.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mmz.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://crn.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://jts.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://chn.yangfankeji.com

TS:   if (x == null) {}
来源：http://dyc.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://eao.aibaodan.cn

Go:   if x == nil {}
来源：http://pxb.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xnw.yuxming.cn

C#:   if (x is null) {}
来源：http://gvc.dianchejie.cn

[P07] 防抖与节流
来源：http://ohh.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://asd.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://xru.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hks.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrp.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vww.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pqo.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iyy.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lbi.sweek.top

[P08] 处理浮点精度问题
来源：http://tat.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eey.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fdf.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kog.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xml.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bve.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wbw.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ncs.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ytz.xylfe.cn

================================================================================
来源：http://lzj.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nhj.hammf.cn

================================================================================
来源：http://xen.c1oappe.top

[Q01] 创建表
来源：http://bnf.zycfv.cn

CREATE TABLE users (
来源：http://kcg.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lsw.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://abp.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://ggv.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mto.zhaomingkeji.xyz

);
来源：http://aby.sysykeji.top

[Q02] 创建带外键的表
来源：http://ewp.meibo888.top

CREATE TABLE orders (
来源：http://fvi.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kxh.fehbvm.com

user_id INT NOT NULL,
来源：http://dvm.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://aoe.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ecf.hnqzz.top

);
来源：http://uss.quarkkingdee.top

[Q03] 增加列
来源：http://rri.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eck.nanxinkj.top

[Q04] 修改列类型
来源：http://yks.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lcz.shuidangran.top

[Q05] 重命名列
来源：http://spa.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zmu.yanxiufei.cn

[Q06] 删除列
来源：http://jvd.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://gua.sjlbkw.cn

[Q07] 删除表
来源：http://mqi.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://haj.jinqigfzy.top

[Q08] 创建普通索引
来源：http://rzv.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://web.yongpay.top

[Q09] 创建唯一索引
来源：http://tnl.aibaodan.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qvu.jinghuilouyu.cn

[Q10] 插入单行
来源：http://vrz.gogol.net.cn


<!-- 参考信息 -->