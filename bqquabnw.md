代发 wailian999

Java: public static void main(String[] args)
来源：http://egp.birdmap.top

Go:   func main()
来源：http://zsd.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://diy.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://wwi.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://fbd.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://cuc.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://tqo.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://uug.cqqwz.cn

TS:   process.platform;  process.version
来源：http://jop.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csn.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tuw.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ujv.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sta.hammf.cn

================================================================================
来源：http://vpl.tianlin.xyz

N. 数据结构与算法
来源：http://yey.jinqigfzy.top

================================================================================
来源：http://cwq.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://ujr.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://obd.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jqg.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgm.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ztq.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://mnq.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://ejt.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://scv.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://ndp.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://jmi.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://jjj.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ylu.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://oni.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kkg.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://htx.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://ifi.pycfn.com

Ruby: arr.sort
来源：http://wis.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qog.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://pqb.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ssy.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://mxn.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kew.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cup.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mgr.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rao.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yfe.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://njz.jianghu66.top

[N04] 斐波那契数列
来源：http://qve.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nlj.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://duu.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eld.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yug.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://whj.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xgg.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wnz.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbh.iojbl.cn

[N05] 最大公约数
来源：http://ijo.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://xwm.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tnv.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bpw.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mhd.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xmx.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qum.chenlongwang.top

Ruby: a.gcd(b)
来源：http://ivi.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bdt.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://qdq.jinqigfzy.top

Py:   s == s[::-1]
来源：http://mpj.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://yqe.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://qzy.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://wef.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jbh.c1oappe.top

Go:   // 双指针从两端比较
来源：http://djw.ehwqpu.com

Ruby: s == s.reverse
来源：http://wzf.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dtq.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://bay.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cpw.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eid.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hwb.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://huj.jinqigufen.top

Java: // 手写 HashMap
来源：http://zbd.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://twg.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://zoe.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://wfu.sweek.top

[N08] 生成全排列
来源：http://cvj.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://iax.9152youxi.cn

PHP:  // 手写递归交换
来源：http://ivk.mhx1999.top

JS:   // 手写回溯递归
来源：http://wyz.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://mix.sxryk.cn

Java: // 手写回溯递归
来源：http://ntq.tian-w.cn

Go:   // 手写回溯递归
来源：http://lji.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://lwy.nwbrower.top

C#:   // 手写回溯递归
来源：http://uhd.zhijiandao.cn

[N09] 栈与队列
来源：http://djc.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yzk.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eyw.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gpx.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mhw.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://apo.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wkl.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yor.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ppk.fktsv.cn

[N10] 链表节点定义
来源：http://uwj.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nuc.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qly.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://drm.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lee.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://kko.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://sac.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jnl.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iha.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://rgp.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://khk.vehdjk.com

PHP:  // 手写递归函数
来源：http://vml.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://trw.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://exn.0kj1m.cn

Java: // 手写递归
来源：http://kfq.jqgufenzy.top

Go:   // 手写递归
来源：http://xwc.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rre.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://sry.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hax.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tjj.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bsi.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vei.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lnu.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eqv.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fyx.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dhm.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ncj.yueranfly.top

================================================================================
来源：http://cnt.yuanzhike.top

O. 并发与异步
来源：http://ymh.9152youxi.cn

================================================================================
来源：http://joe.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://dxc.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aur.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xha.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jug.ydzc1.top

TS:   // 同 JS
来源：http://rqb.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://nbe.aizwys.cn

Go:   go f()
来源：http://frm.haohaochexian.top

Ruby: Thread.new { f }
来源：http://pdw.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://qyw.redwolf501.top

[O02] 使用线程池
来源：http://otk.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uwi.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pkf.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://ufq.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://jks.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://ngz.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hok.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://loy.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zde.hesvh.cn

[O03] 加锁保护共享数据
来源：http://bqh.hesvh.cn

Py:   with lock: shared += 1
来源：http://iju.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xao.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blc.tanke756.top

TS:   // 同 JS
来源：http://glp.sweek.top

Java: synchronized (this) { shared++; }
来源：http://jsd.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sxv.hysaishi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mqr.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://ark.jianghu66.top

[O04] 定义异步函数并等待
来源：http://wkc.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://bky.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wgi.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://utg.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hjq.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sas.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vpk.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://zyb.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://vkn.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://uwf.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://tng.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ojc.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://qjt.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://gts.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rkv.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fxv.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://cbj.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zah.ydzc1.top

[O06] 使用进程池
来源：http://muf.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xtj.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qtv.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://vot.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://dsp.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kgc.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wfr.hywenlv.cn

Ruby: // fork 块
来源：http://evg.jyoumei.cn

C#:   Parallel.For
来源：http://lin.yuanzhike.top

================================================================================
来源：http://djn.xinyue.icu

P. 常用工具函数
来源：http://wwq.yueranfly.top

================================================================================
来源：http://qdg.0kj1m.cn

[P01] 生成 UUID
来源：http://dkn.yongpay.top

Py:   str(uuid.uuid4())
来源：http://tzi.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qye.uphjek.com

JS:   crypto.randomUUID()
来源：http://cko.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://yqy.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://rlc.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://qik.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://zia.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://ysc.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://rum.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ptq.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ohy.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jem.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vyx.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cdd.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://exj.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iha.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wki.52xcode.cn

[P03] 生成短随机字符串
来源：http://yng.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dzm.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sfo.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vob.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://soj.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xlb.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vuy.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://plv.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jcw.cqqwz.cn

[P04] 求长度
来源：http://ocz.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gvd.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvi.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nxh.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xwg.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://onj.xuanzx.com

Go:   len(arr);  len(m)
来源：http://aai.yuanzhike.top

Ruby: x.length;  x.size
来源：http://yvt.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nbs.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://xsx.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://euv.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pch.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lxu.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vcc.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zni.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://pbv.wangshuangyany.cn

Ruby: a == b
来源：http://eou.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qqm.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oqf.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wwl.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://azw.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dad.snrcjt.cn

TS:   if (x == null) {}
来源：http://tsr.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lgi.pycfn.com

Go:   if x == nil {}
来源：http://khg.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bgg.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://als.cdnleiting.top

[P07] 防抖与节流
来源：http://cxb.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://opc.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://rhj.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxv.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jtq.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tta.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://suj.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://rfa.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://god.bjfxy.top

[P08] 处理浮点精度问题
来源：http://ekl.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kes.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sov.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lcw.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sef.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://agm.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wlj.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pjt.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://poi.chenjidiqi.icu

================================================================================
来源：http://nhw.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nuh.havefunace.top

================================================================================
来源：http://nqv.hysaishi.cn

[Q01] 创建表
来源：http://sui.hnqzz.top

CREATE TABLE users (
来源：http://uyi.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oaz.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://lty.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://fnf.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uwb.hcnkem.com

);
来源：http://vgl.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://vom.cashguo.top

CREATE TABLE orders (
来源：http://dkl.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zdv.zhoulong.xyz

user_id INT NOT NULL,
来源：http://igt.ydzc1.top

amount DECIMAL(10, 2),
来源：http://mer.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fop.andypj.xyz

);
来源：http://gio.fengsongda.top

[Q03] 增加列
来源：http://jzj.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://osf.hcnkem.com

[Q04] 修改列类型
来源：http://cgp.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gdc.yj202588.top

[Q05] 重命名列
来源：http://czn.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eir.hesvh.cn

[Q06] 删除列
来源：http://uad.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://clj.52xcode.cn

[Q07] 删除表
来源：http://zjo.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://uwz.iojbl.cn

[Q08] 创建普通索引
来源：http://ajd.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://upg.xziqi.cn

[Q09] 创建唯一索引
来源：http://ere.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uqs.jinghuilouyu.cn

[Q10] 插入单行
来源：http://xls.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aup.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://vzb.bjfxy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hlf.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://juh.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://xma.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xpb.tanke756.top

[Q13] 忽略重复插入
来源：http://xeb.sweek.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qcw.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://fbh.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yvy.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://prl.316326.xyz

[Q15] 查询全部
来源：http://mfo.jlsjyb.cn


<!-- 参考信息 -->