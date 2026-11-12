代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pof.hnxiangtu.top

Ruby: warn "err"
来源：http://qei.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://ozi.ivvv.top

[M07] 判断是否为主入口
来源：http://hob.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://adz.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://swc.cucudq.cn

JS:   require.main === module
来源：http://fnj.xziqi.cn

TS:   require.main === module
来源：http://mpz.aizwys.cn

Java: public static void main(String[] args)
来源：http://kjt.yongpay.top

Go:   func main()
来源：http://bet.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lrm.uphjek.com

C#:   static void Main(string[] args)
来源：http://ehw.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://kps.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://ofa.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://yag.hnqzz.top

JS:   process.platform;  process.version
来源：http://iqh.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://lbi.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ran.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ctt.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://twd.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://psb.redwolf501.top

================================================================================
来源：http://ies.shzxlz.cn

N. 数据结构与算法
来源：http://qtr.hysaishi.cn

================================================================================
来源：http://jkt.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://rjy.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://jhq.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lsz.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfj.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snl.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://vps.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://eke.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gzj.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cib.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://osb.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://giq.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vfl.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hmr.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lzw.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rew.316326.xyz

Go:   slices.Sort(arr)
来源：http://ypp.chenzaomai.com

Ruby: arr.sort
来源：http://duj.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fei.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://voi.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cwq.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://gsb.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgj.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shi.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ryg.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://umb.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tdv.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ptw.yj20258888.top

[N04] 斐波那契数列
来源：http://guv.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yta.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vju.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rys.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ibx.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://spp.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vvm.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gyn.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iqu.iojbl.cn

[N05] 最大公约数
来源：http://vdn.aizwys.cn

Py:   math.gcd(a, b)
来源：http://phl.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kcz.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnp.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://efg.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wpw.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sfz.daria6918.cn

Ruby: a.gcd(b)
来源：http://eon.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hub.xylfe.cn

[N06] 判断回文字符串
来源：http://ehd.xziqi.cn

Py:   s == s[::-1]
来源：http://tzn.ydzc1.top

PHP:  $s === strrev($s);
来源：http://grv.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://yjx.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://oul.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sas.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://dxd.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://mpj.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iok.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://red.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rcr.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jnh.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://npn.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://sjf.tanke756.top

Java: // 手写 HashMap
来源：http://ppt.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://yag.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://ydi.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://tyg.sysykeji.top

[N08] 生成全排列
来源：http://tfc.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://jgm.guowangkeji.top

PHP:  // 手写递归交换
来源：http://wen.zdbjq.cn

JS:   // 手写回溯递归
来源：http://amq.daxiang520.top

TS:   // 手写回溯递归
来源：http://koo.yuanzhike.top

Java: // 手写回溯递归
来源：http://idg.zdqjudy.top

Go:   // 手写回溯递归
来源：http://dkg.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://kva.snrcjt.cn

C#:   // 手写回溯递归
来源：http://uqj.yueranfly.top

[N09] 栈与队列
来源：http://uib.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dor.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vcq.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://owd.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wvm.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jmq.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ppg.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jqy.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jke.zhengqikj.top

[N10] 链表节点定义
来源：http://vfx.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aoq.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://dsq.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dei.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vrn.uphjek.com

Java: class Node { int v; Node next; }
来源：http://woq.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lzb.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ifa.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yty.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://lbl.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://azw.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://bop.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipn.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrk.xinyue.icu

Java: // 手写递归
来源：http://mme.yangfankeji.com

Go:   // 手写递归
来源：http://gel.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qzq.nanxuanxn.top

C#:   // 手写递归
来源：http://exh.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yhx.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://owh.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rgz.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijb.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jge.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wvl.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://val.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yau.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zfc.sweek.top

================================================================================
来源：http://ckr.yongpay.top

O. 并发与异步
来源：http://exr.yuanzhike.top

================================================================================
来源：http://cmc.meibo888.top

[O01] 启动一个线程
来源：http://iju.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://szl.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ijj.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ktv.sjlbkw.cn

TS:   // 同 JS
来源：http://umu.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://nyl.kuanghao11.cn

Go:   go f()
来源：http://kvd.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://qrd.epnwcf.com

C#:   Task.Run(() => F());
来源：http://lje.9152youxi.cn

[O02] 使用线程池
来源：http://yuu.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mfj.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mft.ybcxt.top

JS:   // worker_threads 线程池
来源：http://vzy.daria6918.cn

TS:   // worker_threads 线程池
来源：http://guc.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xgi.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vin.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://llh.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vlf.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://cpv.xinyue.icu

Py:   with lock: shared += 1
来源：http://nmi.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://wpn.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gct.yueranfly.top

TS:   // 同 JS
来源：http://mjn.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://xwd.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://anf.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gau.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://ujg.bjfxy.top

[O04] 定义异步函数并等待
来源：http://drd.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://ssw.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ctw.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://ohr.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fih.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fvl.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gcm.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uer.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://dfs.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://lql.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://ywq.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aiw.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://qfn.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://sdj.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wtj.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zhr.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://fjd.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://qat.nwbrower.top

[O06] 使用进程池
来源：http://shi.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kxa.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tam.yonumen.top

JS:   // child_process / cluster 模块
来源：http://boh.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://kgs.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://did.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://orm.daria6918.cn

Ruby: // fork 块
来源：http://tqb.bjfxy.top

C#:   Parallel.For
来源：http://xqe.hnqzz.top

================================================================================
来源：http://lqa.pengpengdd.cyou

P. 常用工具函数
来源：http://nul.zdqjudy.top

================================================================================
来源：http://qxw.tarul.cn

[P01] 生成 UUID
来源：http://fxk.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://sdc.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qud.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://ngk.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://zua.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://wiz.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://bes.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://dzv.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://boi.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://jiv.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fma.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://imx.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yks.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nzq.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jqy.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kjd.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tls.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iph.hesvh.cn

[P03] 生成短随机字符串
来源：http://hbn.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aze.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://htf.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ljs.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oys.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vam.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oeg.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cpe.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ewv.vqdsnc.cn

[P04] 求长度
来源：http://aqb.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mag.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttc.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxh.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rlp.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://aij.nwbrower.top

Go:   len(arr);  len(m)
来源：http://ysa.hysaishi.cn

Ruby: x.length;  x.size
来源：http://jlz.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jxc.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://mwx.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zfv.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dki.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hri.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kia.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nkx.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://hbd.9152youxi.cn

Ruby: a == b
来源：http://dzu.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fem.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rfr.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vto.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://arz.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://now.aibaodan.cn

TS:   if (x == null) {}
来源：http://pby.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://oek.xylfe.cn

Go:   if x == nil {}
来源：http://sbf.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://job.gotoacloud.top

C#:   if (x is null) {}
来源：http://gja.fengsongda.top

[P07] 防抖与节流
来源：http://dxg.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ror.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://oyk.hnxiangtu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dut.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nrb.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://avx.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ckw.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://slq.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vda.sysykeji.top

[P08] 处理浮点精度问题
来源：http://vex.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://koy.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nnb.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ppb.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bjm.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kea.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aol.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dih.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ahm.cdnleiting.top

================================================================================
来源：http://cex.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xgv.zhiwuduotai.top

================================================================================
来源：http://apw.gaohongyu789.top

[Q01] 创建表
来源：http://sia.hesvh.cn

CREATE TABLE users (
来源：http://rox.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://exy.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://iro.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://oui.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zft.redwolf501.top

);
来源：http://fsx.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://heg.hysaishi.cn

CREATE TABLE orders (
来源：http://roa.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aoq.yongpay.top

user_id INT NOT NULL,
来源：http://tzm.nwbrower.top

amount DECIMAL(10, 2),
来源：http://ayf.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://arj.jinghuilouyu.cn

);
来源：http://zej.wangshuangyany.cn

[Q03] 增加列
来源：http://jrd.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wji.ybcxt.top

[Q04] 修改列类型
来源：http://xow.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ozs.guowangkeji.top

[Q05] 重命名列
来源：http://hgy.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vws.hammf.cn

[Q06] 删除列
来源：http://csh.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://swa.sysykeji.top

[Q07] 删除表
来源：http://okv.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://war.zycfv.cn

[Q08] 创建普通索引
来源：http://hvn.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iem.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://fqx.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yoh.ivvv.top

[Q10] 插入单行
来源：http://dhk.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lnm.zhengqikj.top

[Q11] 一次插入多行
来源：http://zgd.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qxc.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://efy.chenlongwang.top


<!-- 参考信息 -->