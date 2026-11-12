代发 wailian999

Py:   if __name__ == "__main__":
来源：http://tzn.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lre.yj20258.top

JS:   require.main === module
来源：http://kfd.tian-w.cn

TS:   require.main === module
来源：http://gwp.ehwqpu.com

Java: public static void main(String[] args)
来源：http://vxs.yvedp.cn

Go:   func main()
来源：http://ldt.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mwl.yvedp.cn

C#:   static void Main(string[] args)
来源：http://dag.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://ewd.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://jfj.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://fkt.ctjpmb.com

JS:   process.platform;  process.version
来源：http://moo.smart0.xyz

TS:   process.platform;  process.version
来源：http://pyu.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bfo.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vya.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://erp.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://lko.fehbvm.com

================================================================================
来源：http://ihh.guannengcc.top

N. 数据结构与算法
来源：http://jdy.xylfe.cn

================================================================================
来源：http://dqm.ydjk.org.cn

[N01] 二分查找（有序数组）
来源：http://skc.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xqu.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://knm.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ema.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://abd.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://cpu.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://tlx.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kzf.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://xdf.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://odj.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://plf.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vdo.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://phr.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rum.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lht.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://sry.nwbrower.top

Ruby: arr.sort
来源：http://eza.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://osj.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://vqh.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vqz.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://yda.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hry.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xht.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fts.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fqn.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kog.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pay.fengsongda.top

[N04] 斐波那契数列
来源：http://ylr.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tgs.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hgd.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vcl.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ywb.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tsy.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wut.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jrw.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wyk.wangshuangyany.cn

[N05] 最大公约数
来源：http://eiw.hcnkem.com

Py:   math.gcd(a, b)
来源：http://kga.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://olu.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfk.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tis.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cas.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://otu.xziqi.cn

Ruby: a.gcd(b)
来源：http://fnd.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://obf.bjfxy.top

[N06] 判断回文字符串
来源：http://lze.ctjpmb.com

Py:   s == s[::-1]
来源：http://pqe.xuanzx.com

PHP:  $s === strrev($s);
来源：http://rsy.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://ipa.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://cpf.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://opd.tian-w.cn

Go:   // 双指针从两端比较
来源：http://yvj.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://mab.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xvt.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://ugj.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gof.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vqd.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ylj.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://xuu.zhengqikj.top

Java: // 手写 HashMap
来源：http://fhx.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://tjb.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://vdk.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://xtz.cdnleiting.top

[N08] 生成全排列
来源：http://nqx.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://ipq.yfazqb.com

PHP:  // 手写递归交换
来源：http://rzu.yfazqb.com

JS:   // 手写回溯递归
来源：http://ogh.ppjwa.cn

TS:   // 手写回溯递归
来源：http://qow.nwbrower.top

Java: // 手写回溯递归
来源：http://duh.ybcxt.top

Go:   // 手写回溯递归
来源：http://yed.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://abz.vehdjk.com

C#:   // 手写回溯递归
来源：http://mzn.xuanzx.com

[N09] 栈与队列
来源：http://lxz.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zwr.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fcg.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lnu.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qct.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ddo.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ewo.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hju.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xwj.chenlongwang.top

[N10] 链表节点定义
来源：http://kcf.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nby.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://obq.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jwc.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mbb.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://nxp.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://sel.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://swl.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://aut.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://cod.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ioj.ybcxt.top

PHP:  // 手写递归函数
来源：http://sjh.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xaz.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zth.jianghu66.top

Java: // 手写递归
来源：http://rny.shanyushiyangtech.top

Go:   // 手写递归
来源：http://vgc.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sgh.zycfv.cn

C#:   // 手写递归
来源：http://xyd.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ayu.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kjq.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mza.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epa.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://asc.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nad.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://chk.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zlf.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jfb.pengpengdd.cyou

================================================================================
来源：http://crz.yuanzhike.top

O. 并发与异步
来源：http://ecs.yuxming.cn

================================================================================
来源：http://jeh.fehbvm.com

[O01] 启动一个线程
来源：http://bsk.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ysy.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ujp.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pzk.hnxiangtu.top

TS:   // 同 JS
来源：http://tro.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://fwp.cheryme.top

Go:   go f()
来源：http://zih.bbcook.cn

Ruby: Thread.new { f }
来源：http://mrl.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://uus.hnxiangtu.top

[O02] 使用线程池
来源：http://bqw.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yax.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://izq.fzhhl.top

JS:   // worker_threads 线程池
来源：http://hgm.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://vzp.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://gsu.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fiy.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ynh.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vcj.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://pgo.bjfxy.top

Py:   with lock: shared += 1
来源：http://rxn.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://xet.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fav.wangshuangyany.cn

TS:   // 同 JS
来源：http://tne.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://vdt.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://txa.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zpi.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://mrg.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://xmx.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://vqu.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zlj.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://vzl.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ldi.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mho.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://alf.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://qtq.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://clc.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://gzu.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://bdl.hongshengwenyu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vta.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://rvu.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://rmz.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pkj.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tho.sysykeji.top

Ruby: threads.map(&:join)
来源：http://eej.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wse.guowangkeji.top

[O06] 使用进程池
来源：http://cbv.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yhx.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://kqi.pycfn.com

JS:   // child_process / cluster 模块
来源：http://wjh.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://jdx.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dmb.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tqr.haohaochexian.top

Ruby: // fork 块
来源：http://niz.cashguo.top

C#:   Parallel.For
来源：http://eop.hnxiangtu.top

================================================================================
来源：http://bux.epnwcf.com

P. 常用工具函数
来源：http://zmh.hfpthk.cn

================================================================================
来源：http://yij.fktsv.cn

[P01] 生成 UUID
来源：http://rqh.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://kol.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ymt.xziqi.cn

JS:   crypto.randomUUID()
来源：http://ezc.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://bml.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://fzw.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://bxh.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://wow.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://qbr.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://uaa.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dxh.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wxj.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pmd.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pov.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hww.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jso.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jkg.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jkc.haohaochexian.top

[P03] 生成短随机字符串
来源：http://rsg.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tpr.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cno.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bry.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrg.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oiv.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iuo.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pga.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ypg.yangfankeji.com

[P04] 求长度
来源：http://bxc.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gze.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lss.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ngd.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dne.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://mqp.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://xzg.smart0.xyz

Ruby: x.length;  x.size
来源：http://umv.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dtf.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://hsl.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vow.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gnt.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sge.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lbo.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ali.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lwk.meibo888.top

Ruby: a == b
来源：http://mcw.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hee.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lhi.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fgl.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://lkc.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://msl.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://ske.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rla.cucudq.cn

Go:   if x == nil {}
来源：http://hbd.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pnt.guannengcc.top

C#:   if (x is null) {}
来源：http://ohh.ydjk.org.cn

[P07] 防抖与节流
来源：http://dzx.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wti.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://jml.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://luk.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wqu.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oun.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qyg.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://egy.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ias.birdmap.top

[P08] 处理浮点精度问题
来源：http://srs.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dyl.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://exp.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rda.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oxq.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lcq.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oyp.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nfn.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qhc.hesvh.cn

================================================================================
来源：http://xdb.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dwo.ybcxt.top

================================================================================
来源：http://lnd.hnxiangtu.top

[Q01] 创建表
来源：http://adl.yongpay.top

CREATE TABLE users (
来源：http://ofp.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mja.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://urj.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://plf.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dfc.birdmap.top

);
来源：http://wqx.havefunace.top

[Q02] 创建带外键的表
来源：http://gxm.zhiwuduotai.top

CREATE TABLE orders (
来源：http://ykd.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://frz.fehbvm.com

user_id INT NOT NULL,
来源：http://yqr.cashguo.top

amount DECIMAL(10, 2),
来源：http://llm.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fgr.jyoumei.cn

);
来源：http://fjh.zhixingplan.top

[Q03] 增加列
来源：http://mwe.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://all.zhijiandao.cn

[Q04] 修改列类型
来源：http://xpd.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://flc.jinqigufen.top

[Q05] 重命名列
来源：http://ibt.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ozb.ydzc1.top

[Q06] 删除列
来源：http://pbi.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://kng.9152youxi.cn

[Q07] 删除表
来源：http://rok.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://ico.fktsv.cn

[Q08] 创建普通索引
来源：http://dka.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fzq.cucudq.cn

[Q09] 创建唯一索引
来源：http://rbx.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://klu.316326.xyz

[Q10] 插入单行
来源：http://hhq.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ecz.0kj1m.cn

[Q11] 一次插入多行
来源：http://gpb.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jau.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://fwl.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ihh.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ehq.yueranfly.top

[Q13] 忽略重复插入
来源：http://eha.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xhn.sweek.top


<!-- 参考信息 -->