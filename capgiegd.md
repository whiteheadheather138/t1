代发 wailian999

Py:   if __name__ == "__main__":
来源：http://ltw.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wyo.xuetiantiany.cn

JS:   require.main === module
来源：http://uia.bbcook.cn

TS:   require.main === module
来源：http://avv.hfpthk.cn

Java: public static void main(String[] args)
来源：http://sws.hnxiangtu.top

Go:   func main()
来源：http://ajp.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eah.epnwcf.com

C#:   static void Main(string[] args)
来源：http://dnc.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://oxj.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://cfa.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://nyd.daxiang520.top

JS:   process.platform;  process.version
来源：http://fqz.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://bku.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qru.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://swp.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://asg.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xjj.yuxming.cn

================================================================================
来源：http://lmt.vqdsnc.cn

N. 数据结构与算法
来源：http://ncy.zhengqikj.top

================================================================================
来源：http://mus.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://wir.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xbv.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ulk.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fvo.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzg.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iji.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://bqc.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hiz.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://nzb.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://nkn.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://pxd.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fxm.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kbb.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cjl.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lqa.yj20258888.top

Go:   slices.Sort(arr)
来源：http://ivx.jqgfzy.top

Ruby: arr.sort
来源：http://lmh.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://atr.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://wtw.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oqt.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://wry.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://smt.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wrb.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yon.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pcp.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mno.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jzr.yfazqb.com

[N04] 斐波那契数列
来源：http://ogo.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://viu.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yrx.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cqi.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yri.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hah.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hha.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://boq.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bij.svipenyu.cn

[N05] 最大公约数
来源：http://nid.yueranfly.top

Py:   math.gcd(a, b)
来源：http://vsc.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vlc.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qog.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crp.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qhx.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jio.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://yua.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gkk.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://xbc.zhixingplan.top

Py:   s == s[::-1]
来源：http://thw.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://wuv.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://jyh.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://lnv.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ugy.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://itw.tianlin.xyz

Ruby: s == s.reverse
来源：http://qhj.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://pfa.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://pxe.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cuh.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hcn.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tje.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://eln.guowangkeji.top

Java: // 手写 HashMap
来源：http://jxh.52xcode.cn

Go:   // 手写 map[int]int
来源：http://wik.tian-w.cn

Ruby: // 手写 Hash
来源：http://vom.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://ber.zhongyouzk.top

[N08] 生成全排列
来源：http://pbj.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://jpl.yj202588.top

PHP:  // 手写递归交换
来源：http://yro.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://bkk.bbcook.cn

TS:   // 手写回溯递归
来源：http://tkc.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://pfl.hywenlv.cn

Go:   // 手写回溯递归
来源：http://emm.shzxlz.cn

Ruby: arr.permutation.to_a
来源：http://mdi.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://kgk.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://wgk.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jtp.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ben.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nat.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zms.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cyk.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jrx.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fag.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://krd.fktsv.cn

[N10] 链表节点定义
来源：http://klu.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iqp.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tbu.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mgj.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lwh.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://mdy.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://mau.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vzh.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ufp.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://luq.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pat.guannengcc.top

PHP:  // 手写递归函数
来源：http://osc.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivn.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpz.jinqigfzy.top

Java: // 手写递归
来源：http://eey.fanxiaobao.xyz

Go:   // 手写递归
来源：http://lkc.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nag.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://agp.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tdw.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wgu.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mrj.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nrc.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrv.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lmi.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hvn.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mle.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fxo.fktsv.cn

================================================================================
来源：http://bzi.pycfn.com

O. 并发与异步
来源：http://hea.aizwys.cn

================================================================================
来源：http://hah.0kj1m.cn

[O01] 启动一个线程
来源：http://dxm.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://npv.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gno.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ouz.tarul.cn

TS:   // 同 JS
来源：http://zjr.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://dzz.yongpay.top

Go:   go f()
来源：http://vlw.guannengcc.top

Ruby: Thread.new { f }
来源：http://php.sweek.top

C#:   Task.Run(() => F());
来源：http://xxz.aizwys.cn

[O02] 使用线程池
来源：http://buj.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://izc.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ewx.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://ces.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://xmr.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://nfw.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ets.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ola.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://odc.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://cxq.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://ojl.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://npo.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ner.jiagoushi.top

TS:   // 同 JS
来源：http://lvo.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://pgv.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uiq.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pnt.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://pla.smart0.xyz

[O04] 定义异步函数并等待
来源：http://jys.cheryme.top

Py:   async def f():⏎    await g()
来源：http://gzg.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://psx.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://cfr.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zcg.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uir.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kof.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://lif.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://ddv.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://uze.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://esg.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mdv.tarul.cn

JS:   await Promise.all(tasks)
来源：http://seo.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://lyz.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kli.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://laf.yj20258.top

Ruby: threads.map(&:join)
来源：http://mpp.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ezv.pycfn.com

[O06] 使用进程池
来源：http://koq.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://omp.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mfu.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://ter.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://gxi.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://irf.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zxx.shuidangran.top

Ruby: // fork 块
来源：http://oou.xinyue.icu

C#:   Parallel.For
来源：http://zqt.sufxvd.cn

================================================================================
来源：http://efs.c1oappe.top

P. 常用工具函数
来源：http://oby.chenlongwang.top

================================================================================
来源：http://umn.yongpay.top

[P01] 生成 UUID
来源：http://fbh.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://ywu.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nys.guannengcc.top

JS:   crypto.randomUUID()
来源：http://qly.mhx1999.top

TS:   crypto.randomUUID()
来源：http://jyy.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://gal.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://poc.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://eej.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://abw.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://fka.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://icg.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dya.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cov.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sao.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mbb.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://soi.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wep.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pty.yj20258888.top

[P03] 生成短随机字符串
来源：http://geo.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lgp.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hxh.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yzs.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ilu.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rty.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://agh.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjr.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgs.svipenyu.cn

[P04] 求长度
来源：http://zdi.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wuc.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fxf.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rfj.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ped.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://xhf.ivvv.top

Go:   len(arr);  len(m)
来源：http://igm.xinyue.icu

Ruby: x.length;  x.size
来源：http://qex.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xrg.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://gun.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rle.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cxy.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rhr.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wuq.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eft.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://rxb.ywan-chungtsiang.top

Ruby: a == b
来源：http://qmd.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jus.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ggp.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jkk.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://oql.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lqz.316326.xyz

TS:   if (x == null) {}
来源：http://nno.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://hec.ybcxt.top

Go:   if x == nil {}
来源：http://iql.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cnr.tanke756.top

C#:   if (x is null) {}
来源：http://ikk.mhx1999.top

[P07] 防抖与节流
来源：http://ejb.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fon.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://nwz.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ncu.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjd.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kli.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qcv.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqh.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ugh.epnwcf.com

[P08] 处理浮点精度问题
来源：http://abx.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hyp.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yrr.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lbw.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nat.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ksi.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fmr.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tcj.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gou.vqdsnc.cn

================================================================================
来源：http://yzq.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wss.fzhhl.top

================================================================================
来源：http://xag.zhixingplan.top

[Q01] 创建表
来源：http://qgg.c1oappe.top

CREATE TABLE users (
来源：http://tow.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jyt.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://mog.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://qmb.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cne.tanke756.top

);
来源：http://vlf.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://mxp.sjlbkw.cn

CREATE TABLE orders (
来源：http://zlm.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bpr.yj20258.top

user_id INT NOT NULL,
来源：http://xys.ydzc1.top

amount DECIMAL(10, 2),
来源：http://hlw.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sdn.hysaishi.cn

);
来源：http://qzm.chenlongwang.top

[Q03] 增加列
来源：http://gxp.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yiu.ctjpmb.com

[Q04] 修改列类型
来源：http://mzy.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pck.gotoacloud.top

[Q05] 重命名列
来源：http://wtd.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xbc.fehbvm.com

[Q06] 删除列
来源：http://qsg.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://qhd.ehwqpu.com

[Q07] 删除表
来源：http://pye.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://ssl.hywenlv.cn

[Q08] 创建普通索引
来源：http://rwh.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wmw.smart0.xyz

[Q09] 创建唯一索引
来源：http://vjn.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aav.hnxiangtu.top

[Q10] 插入单行
来源：http://yui.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ois.hnxiangtu.top

[Q11] 一次插入多行
来源：http://ulg.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kuq.pycfn.com

[Q12] 插入后取自增 ID
来源：http://kxi.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://amk.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gzt.yonumen.top

[Q13] 忽略重复插入
来源：http://gvn.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zjf.jlsjyb.cn


<!-- 参考信息 -->