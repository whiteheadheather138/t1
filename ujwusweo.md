代发 wailian999

Py:   if __name__ == "__main__":
来源：http://qtq.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fyv.aibaodan.cn

JS:   require.main === module
来源：http://uhu.jiagoushi.top

TS:   require.main === module
来源：http://ctn.guowangkeji.top

Java: public static void main(String[] args)
来源：http://oje.cdnleiting.top

Go:   func main()
来源：http://vgw.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kaz.cashguo.top

C#:   static void Main(string[] args)
来源：http://knl.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://fpy.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://yqw.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://hmt.aibaodan.cn

JS:   process.platform;  process.version
来源：http://nii.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://zai.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vrm.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://syy.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mge.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jco.haohaochexian.top

================================================================================
来源：http://lcj.fzhhl.top

N. 数据结构与算法
来源：http://wox.jlsjyb.cn

================================================================================
来源：http://nps.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://mkg.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://smq.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://czo.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lwl.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwk.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yef.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://ioo.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wze.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://vbl.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://ari.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://tge.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aqx.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://egq.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mqd.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yxg.hcnkem.com

Go:   slices.Sort(arr)
来源：http://eyp.hongshengwenyu.top

Ruby: arr.sort
来源：http://sqs.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rem.birdmap.top

[N03] 快速排序（分治示例）
来源：http://fup.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ily.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://xuq.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://czh.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hvx.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sxg.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://epi.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ogl.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://hun.pycfn.com

[N04] 斐波那契数列
来源：http://puu.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mzv.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tma.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kyv.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qrc.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cbq.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yju.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hvc.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fpx.ydjk.org.cn

[N05] 最大公约数
来源：http://gah.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://rjy.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ext.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://atr.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lwz.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mur.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hxw.chenlongwang.top

Ruby: a.gcd(b)
来源：http://mgl.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ioz.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://faa.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://tcd.hnqzz.top

PHP:  $s === strrev($s);
来源：http://hyt.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://nfr.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://qgs.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ocv.sweek.top

Go:   // 双指针从两端比较
来源：http://kak.fzhhl.top

Ruby: s == s.reverse
来源：http://rth.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://icu.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://rze.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pti.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ign.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xzv.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://ypo.shzxlz.cn

Java: // 手写 HashMap
来源：http://lmu.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://wlg.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://qcn.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://xig.pycfn.com

[N08] 生成全排列
来源：http://zqx.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://aiu.hnqzz.top

PHP:  // 手写递归交换
来源：http://tnp.redwolf501.top

JS:   // 手写回溯递归
来源：http://veh.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://tik.gzhubu.top

Java: // 手写回溯递归
来源：http://uku.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://uxt.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://yos.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://zch.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://rly.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xqr.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uqc.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qjy.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mqq.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rhr.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kgs.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qng.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ykh.zdqjudy.top

[N10] 链表节点定义
来源：http://hjh.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qgl.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cek.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://crc.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ghj.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://tmu.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://qir.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rgf.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fcy.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://uiu.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bjw.daxiang520.top

PHP:  // 手写递归函数
来源：http://qnt.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aaq.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://szb.sweek.top

Java: // 手写递归
来源：http://hno.shanyushiyangtech.top

Go:   // 手写递归
来源：http://hyr.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oyd.316326.xyz

C#:   // 手写递归
来源：http://eha.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://umr.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://upb.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ycr.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ndg.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bde.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fnc.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nyk.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dfu.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lcq.fanxiaobao.xyz

================================================================================
来源：http://baq.xuanzx.com

O. 并发与异步
来源：http://hxu.ppjwa.cn

================================================================================
来源：http://rcq.gaohongyu789.top

[O01] 启动一个线程
来源：http://ees.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dbx.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rea.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zxx.jinqigfzy.top

TS:   // 同 JS
来源：http://upc.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://bmy.zhaomingkeji.xyz

Go:   go f()
来源：http://xgw.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://iat.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://ujg.zdqjudy.top

[O02] 使用线程池
来源：http://ewo.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kxm.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wjf.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://ipr.xylfe.cn

TS:   // worker_threads 线程池
来源：http://uxr.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dmx.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cco.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kfj.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mvf.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://jwx.hammf.cn

Py:   with lock: shared += 1
来源：http://bpy.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://lyk.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hgf.guowangkeji.top

TS:   // 同 JS
来源：http://mej.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://awq.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xps.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://apv.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://pjj.cashguo.top

[O04] 定义异步函数并等待
来源：http://iww.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://ojp.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tps.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://its.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tnn.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aed.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ttw.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qgf.hammf.cn

C#:   async Task F() { await G(); }
来源：http://vdu.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://pgs.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://ymy.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mah.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://ujh.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://fuz.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oex.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jqf.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://iye.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mtj.xuanzx.com

[O06] 使用进程池
来源：http://czo.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wac.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rni.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://lfm.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://arp.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gma.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mvc.zdqjudy.top

Ruby: // fork 块
来源：http://lxe.nanxinkj.top

C#:   Parallel.For
来源：http://skh.tianlin.xyz

================================================================================
来源：http://zdq.jianghu66.top

P. 常用工具函数
来源：http://ldg.yongpay.top

================================================================================
来源：http://jbv.xziqi.cn

[P01] 生成 UUID
来源：http://ixu.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://vei.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rmy.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://flp.fktsv.cn

TS:   crypto.randomUUID()
来源：http://wts.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://ceh.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://xll.cashguo.top

Ruby: SecureRandom.uuid
来源：http://npf.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://zsq.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://hdv.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sdy.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gms.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uvw.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lmw.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://voh.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vdn.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nqh.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ian.zdqjudy.top

[P03] 生成短随机字符串
来源：http://hqa.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gvb.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lde.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zkb.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gsq.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ykp.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kdh.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://owy.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fea.jinyuanbaomall.cn

[P04] 求长度
来源：http://joa.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vsq.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://maa.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bju.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qds.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://equ.cashguo.top

Go:   len(arr);  len(m)
来源：http://xta.cqqwz.cn

Ruby: x.length;  x.size
来源：http://ktt.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://gnm.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://eta.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://aji.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mxf.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pcx.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://scv.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nil.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://hxb.nanxuanxn.top

Ruby: a == b
来源：http://cir.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iaw.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nya.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bmg.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://iqi.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://chk.ydjk.org.cn

TS:   if (x == null) {}
来源：http://vzu.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ywe.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://dzu.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kfe.cashguo.top

C#:   if (x is null) {}
来源：http://rvz.ydzc1.top

[P07] 防抖与节流
来源：http://orx.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nfj.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://wmc.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfq.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtb.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hpi.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kbf.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nrx.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rjx.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://zmw.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aim.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hyy.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mfb.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vcm.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://axp.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ggh.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ggz.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wpc.yfazqb.com

================================================================================
来源：http://atr.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pqu.ywan-chungtsiang.top

================================================================================
来源：http://xyr.gogol.net.cn

[Q01] 创建表
来源：http://gph.316326.xyz

CREATE TABLE users (
来源：http://ffc.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rej.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://iau.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://vgk.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rhn.zhixingplan.top

);
来源：http://pwl.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://hbo.haohaochexian.top

CREATE TABLE orders (
来源：http://hjd.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozi.dashuyun.cn

user_id INT NOT NULL,
来源：http://rnr.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://mry.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jkj.ehwqpu.com

);
来源：http://dxr.hnqzz.top

[Q03] 增加列
来源：http://ffi.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hjb.guannengcc.top

[Q04] 修改列类型
来源：http://pde.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://inu.wangdashe.top

[Q05] 重命名列
来源：http://axt.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cxg.jlsjyb.cn

[Q06] 删除列
来源：http://ujx.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://per.xinyue.icu

[Q07] 删除表
来源：http://drz.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://pos.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://smi.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eus.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://aem.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jrw.hfpthk.cn

[Q10] 插入单行
来源：http://ner.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hvl.dashuyun.cn

[Q11] 一次插入多行
来源：http://xtb.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ehj.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://lmp.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nmi.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fzs.epnwcf.com

[Q13] 忽略重复插入
来源：http://zmw.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zbf.ppjwa.cn


<!-- 参考信息 -->