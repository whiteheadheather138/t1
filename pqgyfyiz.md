代发 wailian999

Java: public static void main(String[] args)
来源：http://dnw.shuidangran.top

Go:   func main()
来源：http://tpj.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://svo.yj20258888.top

C#:   static void Main(string[] args)
来源：http://efw.cheryme.top

[M08] 获取系统与运行时信息
来源：http://qxj.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://zwj.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://jvx.andypj.xyz

JS:   process.platform;  process.version
来源：http://mrn.meibo888.top

TS:   process.platform;  process.version
来源：http://anj.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xdb.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eec.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tmp.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gpg.jinqigfzy.top

================================================================================
来源：http://ecl.jqgfzy.top

N. 数据结构与算法
来源：http://rej.sufxvd.cn

================================================================================
来源：http://baz.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://zva.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://isk.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pyr.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://unt.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://krl.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dnc.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://nui.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qmz.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://fau.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://kxv.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://dtt.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jnn.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ywh.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cuy.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sfw.yueranfly.top

Go:   slices.Sort(arr)
来源：http://nky.hcnkem.com

Ruby: arr.sort
来源：http://cpu.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ipd.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://hfs.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://slg.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://maj.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vnh.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://clf.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rzz.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zoy.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tjx.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uen.ppjwa.cn

[N04] 斐波那契数列
来源：http://xxg.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bcm.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xms.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://som.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nez.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yij.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jms.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kdx.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dgk.guowangkeji.top

[N05] 最大公约数
来源：http://eoh.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://aqm.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xzy.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwx.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://koa.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rnd.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xjs.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://nne.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rdl.yanxiufei.cn

[N06] 判断回文字符串
来源：http://yyu.vehdjk.com

Py:   s == s[::-1]
来源：http://zso.daria6918.cn

PHP:  $s === strrev($s);
来源：http://ntw.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://wtb.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://zwl.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mvp.guannengcc.top

Go:   // 双指针从两端比较
来源：http://chw.jiagoushi.top

Ruby: s == s.reverse
来源：http://jka.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hgl.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://kwe.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rsw.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aiz.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hsy.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://tze.yj20258.top

Java: // 手写 HashMap
来源：http://uck.daxiang520.top

Go:   // 手写 map[int]int
来源：http://wgn.yangfankeji.com

Ruby: // 手写 Hash
来源：http://hle.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://ajb.mhx1999.top

[N08] 生成全排列
来源：http://puh.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://odn.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://gqf.9152youxi.cn

JS:   // 手写回溯递归
来源：http://gkj.cheryme.top

TS:   // 手写回溯递归
来源：http://guy.yonumen.top

Java: // 手写回溯递归
来源：http://uxe.fzhhl.top

Go:   // 手写回溯递归
来源：http://cqv.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://icv.yj20258888.top

C#:   // 手写回溯递归
来源：http://abe.ctjpmb.com

[N09] 栈与队列
来源：http://web.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eym.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://voe.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rfp.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aez.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lwi.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wbc.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rca.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fqx.mhx1999.top

[N10] 链表节点定义
来源：http://eld.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dgv.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://scb.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lgk.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hsg.sweek.top

Java: class Node { int v; Node next; }
来源：http://sgc.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kfw.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gno.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://chr.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://ntn.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bab.daxiang520.top

PHP:  // 手写递归函数
来源：http://ehv.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ysm.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qjo.xuetiantiany.cn

Java: // 手写递归
来源：http://rpf.mhx1999.top

Go:   // 手写递归
来源：http://npl.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://twp.hammf.cn

C#:   // 手写递归
来源：http://ucs.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zkz.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyf.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ifx.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thw.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gkn.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oon.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vmh.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyz.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zac.redwolf501.top

================================================================================
来源：http://jco.shzxlz.cn

O. 并发与异步
来源：http://puz.dianchejie.cn

================================================================================
来源：http://usm.shuidangran.top

[O01] 启动一个线程
来源：http://jou.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xkp.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kqd.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://con.zhiwuduotai.top

TS:   // 同 JS
来源：http://cjt.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://nda.sysykeji.top

Go:   go f()
来源：http://uuq.gzhubu.top

Ruby: Thread.new { f }
来源：http://vvf.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://eqh.sufxvd.cn

[O02] 使用线程池
来源：http://dyu.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qth.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dbf.pycfn.com

JS:   // worker_threads 线程池
来源：http://aks.tian-w.cn

TS:   // worker_threads 线程池
来源：http://wei.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://azf.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://szw.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://euc.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fvw.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://anx.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://fxx.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://chl.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fmj.redwolf501.top

TS:   // 同 JS
来源：http://zqx.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://rbt.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gpp.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xxi.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://axd.hammf.cn

[O04] 定义异步函数并等待
来源：http://rmw.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://jxz.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zjv.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://faq.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://wrf.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://svy.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tcp.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://iuj.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://iol.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://kre.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://dyk.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mvl.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://lsj.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://iyk.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xiq.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yaw.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://vmj.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ahf.birdmap.top

[O06] 使用进程池
来源：http://zuq.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vjy.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://njr.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://wch.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://jbz.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xdk.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mkk.yueranfly.top

Ruby: // fork 块
来源：http://doq.shanyushiyangtech.top

C#:   Parallel.For
来源：http://bmn.ctjpmb.com

================================================================================
来源：http://aeg.shangyingyoupin.top

P. 常用工具函数
来源：http://vmt.zhoulong.xyz

================================================================================
来源：http://qku.fzhhl.top

[P01] 生成 UUID
来源：http://fbs.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://gfd.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nep.feifeiyinyue.top

JS:   crypto.randomUUID()
来源：http://krk.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://qxw.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://skf.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://rdf.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://typ.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://wrw.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://hrn.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yiz.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://yst.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lzl.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pkk.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gxz.gzhubu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xis.xziqi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zhy.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ywc.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://abj.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gyc.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dnq.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vre.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gyf.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gqy.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pww.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://whv.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lxl.yangfankeji.com

[P04] 求长度
来源：http://ltr.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kqq.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bsp.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kos.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fqm.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://cde.yfazqb.com

Go:   len(arr);  len(m)
来源：http://nqi.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://srn.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xtp.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://gyx.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eve.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wnr.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xbh.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pyo.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ctu.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tjq.hesvh.cn

Ruby: a == b
来源：http://stg.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xox.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fob.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rqi.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://ipc.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cyq.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://vbi.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://das.zycfv.cn

Go:   if x == nil {}
来源：http://ibu.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bof.yonumen.top

C#:   if (x is null) {}
来源：http://lnx.chenlongwang.top

[P07] 防抖与节流
来源：http://gup.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mfn.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://gny.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhc.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://goj.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://njv.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hkq.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://teq.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bpn.cheryme.top

[P08] 处理浮点精度问题
来源：http://nwq.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://muw.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uzn.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bro.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ult.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hhw.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ewf.yj20258888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xbb.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zod.xylfe.cn

================================================================================
来源：http://stu.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cgp.yj202588.top

================================================================================
来源：http://mrb.fzhhl.top

[Q01] 创建表
来源：http://flr.fktsv.cn

CREATE TABLE users (
来源：http://tyj.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://etg.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://uia.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://nad.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xgl.epnwcf.com

);
来源：http://tps.cheryme.top

[Q02] 创建带外键的表
来源：http://qdx.52xcode.cn

CREATE TABLE orders (
来源：http://gjm.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rrk.hywenlv.cn

user_id INT NOT NULL,
来源：http://bxw.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://ivx.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sho.smart0.xyz

);
来源：http://ndu.jinqigfzy.top

[Q03] 增加列
来源：http://xpg.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ppa.snrcjt.cn

[Q04] 修改列类型
来源：http://zov.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yzq.hnxiangtu.top

[Q05] 重命名列
来源：http://tau.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://csm.daria6918.cn

[Q06] 删除列
来源：http://ect.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vga.shangyingyoupin.top

[Q07] 删除表
来源：http://inn.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://xkh.cqqwz.cn

[Q08] 创建普通索引
来源：http://jys.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lgc.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://hlo.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dqk.cdnleiting.top

[Q10] 插入单行
来源：http://qwf.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ymj.9152youxi.cn

[Q11] 一次插入多行
来源：http://qtk.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mqj.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://ttd.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://qwn.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hpa.sysykeji.top

[Q13] 忽略重复插入
来源：http://fgo.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eci.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://okn.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://llj.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://awx.xylfe.cn

[Q15] 查询全部
来源：http://hvq.redwolf501.top


<!-- 参考信息 -->