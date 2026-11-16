代发 wailian999

Py:   if __name__ == "__main__":
来源：http://mty.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yjk.vehdjk.com

JS:   require.main === module
来源：http://gll.yj20258.top

TS:   require.main === module
来源：http://uxg.zdqjudy.top

Java: public static void main(String[] args)
来源：http://ccs.9152youxi.cn

Go:   func main()
来源：http://uey.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mzp.tian-w.cn

C#:   static void Main(string[] args)
来源：http://uwn.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://bcs.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://eib.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://luj.xziqi.cn

JS:   process.platform;  process.version
来源：http://hgv.cashguo.top

TS:   process.platform;  process.version
来源：http://mch.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wwj.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aso.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vlr.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://idk.cucudq.cn

================================================================================
来源：http://nbz.xuanzx.com

N. 数据结构与算法
来源：http://hin.ivvv.top

================================================================================
来源：http://jjd.yongpay.top

[N01] 二分查找（有序数组）
来源：http://jki.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://rwj.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pam.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tum.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://niz.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ynw.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://kid.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xni.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://dty.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://ogr.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://pzq.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://igu.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ovo.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gfy.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qai.nwbrower.top

Go:   slices.Sort(arr)
来源：http://gak.cheryme.top

Ruby: arr.sort
来源：http://yvg.9152youxi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bmm.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://vvi.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://krs.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://wnb.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ild.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mds.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iwa.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tan.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uuw.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hnqzz.top

[N04] 斐波那契数列
来源：http://kjn.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mcw.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zpk.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgv.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://izr.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rgm.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gtb.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kwb.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qpc.yangfankeji.com

[N05] 最大公约数
来源：http://izu.tanke756.top

Py:   math.gcd(a, b)
来源：http://kwy.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dlk.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qrj.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqd.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uyt.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://npa.gogol.net.cn

Ruby: a.gcd(b)
来源：http://zbk.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dez.hnxiangtu.top

[N06] 判断回文字符串
来源：http://mrc.sjlbkw.cn

Py:   s == s[::-1]
来源：http://xew.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://pwt.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://acn.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://uvu.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lzd.fengsongda.top

Go:   // 双指针从两端比较
来源：http://jzi.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://lck.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://puw.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://mbg.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nga.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cos.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gxc.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://prs.xinyue.icu

Java: // 手写 HashMap
来源：http://nas.316326.xyz

Go:   // 手写 map[int]int
来源：http://kwv.xuanzx.com

Ruby: // 手写 Hash
来源：http://qgc.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yhg.tanke756.top

[N08] 生成全排列
来源：http://ehj.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://xdl.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://kya.jiagoushi.top

JS:   // 手写回溯递归
来源：http://xvr.zdbjq.cn

TS:   // 手写回溯递归
来源：http://oyn.cucudq.cn

Java: // 手写回溯递归
来源：http://skh.uphjek.com

Go:   // 手写回溯递归
来源：http://hgd.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://yez.zdqjudy.top

C#:   // 手写回溯递归
来源：http://ykt.guannengcc.top

[N09] 栈与队列
来源：http://pkg.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://otm.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rjt.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gpt.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dvu.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pss.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://apl.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sjb.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rby.nwbrower.top

[N10] 链表节点定义
来源：http://ewl.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tqx.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kfh.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bjg.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zez.cheryme.top

Java: class Node { int v; Node next; }
来源：http://csz.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://hel.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ynt.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tar.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://ojy.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qjx.ppjwa.cn

PHP:  // 手写递归函数
来源：http://pkh.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgi.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://skw.fktsv.cn

Java: // 手写递归
来源：http://saq.shzxlz.cn

Go:   // 手写递归
来源：http://hux.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vev.jinqigfzy.top

C#:   // 手写递归
来源：http://jpo.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://usn.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://edz.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dvj.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eva.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwk.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yuo.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lbv.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gay.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bkx.birdmap.top

================================================================================
来源：http://nkv.yonumen.top

O. 并发与异步
来源：http://qoz.zhoulong.xyz

================================================================================
来源：http://qft.jyoumei.cn

[O01] 启动一个线程
来源：http://qyx.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://izb.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zao.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://muv.wangshuangyany.cn

TS:   // 同 JS
来源：http://toq.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://fkd.jianghu66.top

Go:   go f()
来源：http://fkt.daxiang520.top

Ruby: Thread.new { f }
来源：http://xvv.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://gfn.hammf.cn

[O02] 使用线程池
来源：http://eol.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uvg.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uol.aizwys.cn

JS:   // worker_threads 线程池
来源：http://evc.hnqzz.top

TS:   // worker_threads 线程池
来源：http://bdt.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://qou.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqt.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bul.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ehh.fehbvm.com

[O03] 加锁保护共享数据
来源：http://cst.meibo888.top

Py:   with lock: shared += 1
来源：http://bac.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://ooh.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://idv.epnwcf.com

TS:   // 同 JS
来源：http://wvs.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://ble.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vls.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oxr.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://hcb.sxryk.cn

[O04] 定义异步函数并等待
来源：http://jyb.birdmap.top

Py:   async def f():⏎    await g()
来源：http://rwd.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iba.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://ywx.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lqv.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cgg.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyr.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://yup.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://pex.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://soj.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://eiw.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://onn.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://qjw.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://czi.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zxc.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://onh.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://okj.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bbe.svipenyu.cn

[O06] 使用进程池
来源：http://kbo.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vhb.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://lis.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://vpy.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://dyt.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://csv.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mib.xinyue.icu

Ruby: // fork 块
来源：http://rva.hammf.cn

C#:   Parallel.For
来源：http://mof.hnqzz.top

================================================================================
来源：http://mjq.hnxiangtu.top

P. 常用工具函数
来源：http://xnk.chenzaomai.com

================================================================================
来源：http://thu.sjlbkw.cn

[P01] 生成 UUID
来源：http://hpk.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://zvy.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oxx.fktsv.cn

JS:   crypto.randomUUID()
来源：http://hri.ydzc1.top

TS:   crypto.randomUUID()
来源：http://iqf.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://qtu.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://pyv.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://uzu.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://wcd.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://vfx.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmu.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vlr.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rec.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iea.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qvi.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lpd.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oot.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qnn.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://rhp.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jjx.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nso.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://efv.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pca.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://usd.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sxo.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://jjx.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qww.jqgufenzy.top

[P04] 求长度
来源：http://xxj.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tnh.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgd.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sxb.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ghg.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://kcm.jianghu66.top

Go:   len(arr);  len(m)
来源：http://wlh.c1oappe.top

Ruby: x.length;  x.size
来源：http://jqa.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://slw.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://cow.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wjk.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ogl.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ajw.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://reu.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rzw.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sam.bbcook.cn

Ruby: a == b
来源：http://woj.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ned.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kpt.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ahs.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://jmf.gogol.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://znv.sweek.top

TS:   if (x == null) {}
来源：http://vbk.yongpay.top

Java: if (x == null || x.isEmpty()) {}
来源：http://feu.zhengqikj.top

Go:   if x == nil {}
来源：http://fhv.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ran.dashuyun.cn

C#:   if (x is null) {}
来源：http://bus.snrcjt.cn

[P07] 防抖与节流
来源：http://vem.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zlo.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://xvu.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cnw.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dbq.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://afy.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ldk.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ndh.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pjj.yj202588.top

[P08] 处理浮点精度问题
来源：http://fwr.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://moc.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uia.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://huz.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kxn.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kog.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wyb.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ccr.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lst.pengpengdd.cyou

================================================================================
来源：http://fiw.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qih.kuanghao11.cn

================================================================================
来源：http://tiv.jqgufenzy.top

[Q01] 创建表
来源：http://eov.zdbjq.cn

CREATE TABLE users (
来源：http://aqf.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkm.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://jkv.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://khk.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ysh.yvedp.cn

);
来源：http://sbh.hysaishi.cn

[Q02] 创建带外键的表
来源：http://ldn.ydzc1.top

CREATE TABLE orders (
来源：http://shg.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oea.yanxiufei.cn

user_id INT NOT NULL,
来源：http://irw.hnqzz.top

amount DECIMAL(10, 2),
来源：http://ojv.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xfy.daxiang520.top

);
来源：http://xns.hywenlv.cn

[Q03] 增加列
来源：http://dhp.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fml.kuanghao11.cn

[Q04] 修改列类型
来源：http://rsq.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bcb.hesvh.cn

[Q05] 重命名列
来源：http://cbw.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://atb.meibo888.top

[Q06] 删除列
来源：http://ijf.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jbs.zhixingplan.top

[Q07] 删除表
来源：http://vjd.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://jic.chenlongwang.top

[Q08] 创建普通索引
来源：http://xpx.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cut.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://zyx.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iyu.52xcode.cn

[Q10] 插入单行
来源：http://off.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cyp.ppjwa.cn

[Q11] 一次插入多行
来源：http://ras.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qpo.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://fmz.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jsn.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tjl.haohaochexian.top

[Q13] 忽略重复插入
来源：http://iut.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ska.ivvv.top


<!-- 参考信息 -->