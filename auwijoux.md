代发 wailian999

Py:   if __name__ == "__main__":
来源：http://ouj.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jan.yj20258888.top

JS:   require.main === module
来源：http://ejx.yuxming.cn

TS:   require.main === module
来源：http://gya.ehwqpu.com

Java: public static void main(String[] args)
来源：http://kpx.andypj.xyz

Go:   func main()
来源：http://fmc.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lny.fktsv.cn

C#:   static void Main(string[] args)
来源：http://gfq.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://bvb.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://fgq.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://pch.zycfv.cn

JS:   process.platform;  process.version
来源：http://oxp.ehwqpu.com

TS:   process.platform;  process.version
来源：http://cau.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vgp.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vfl.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nei.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fmz.tianlin.xyz

================================================================================
来源：http://iki.zdqjudy.top

N. 数据结构与算法
来源：http://zmo.epnwcf.com

================================================================================
来源：http://izs.tanke756.top

[N01] 二分查找（有序数组）
来源：http://gwh.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://pjf.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wlt.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aga.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cjf.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://ieo.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://gda.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zzr.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oeo.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://bgb.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://gfk.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jrq.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lmz.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fws.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pza.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://vpz.jlsjyb.cn

Ruby: arr.sort
来源：http://bsv.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fny.yongpay.top

[N03] 快速排序（分治示例）
来源：http://pyh.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ium.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://twh.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vnd.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://suu.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lrx.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://axm.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://egh.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://kuf.shzxlz.cn

[N04] 斐波那契数列
来源：http://cbc.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zzp.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yed.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gwc.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfj.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rtz.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://clb.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yim.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dtv.jinqigufen.top

[N05] 最大公约数
来源：http://usl.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://iim.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hci.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdl.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swg.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vlu.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rxp.daxiang520.top

Ruby: a.gcd(b)
来源：http://leo.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://acv.hnqzz.top

[N06] 判断回文字符串
来源：http://lyt.cheryme.top

Py:   s == s[::-1]
来源：http://chu.bbcook.cn

PHP:  $s === strrev($s);
来源：http://azz.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://jpk.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://hpr.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hcj.yueranfly.top

Go:   // 双指针从两端比较
来源：http://cuz.hnxiangtu.top

Ruby: s == s.reverse
来源：http://cib.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cpb.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://xuo.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://irf.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yqj.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lbr.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://ofm.hnxiangtu.top

Java: // 手写 HashMap
来源：http://dwa.fehbvm.com

Go:   // 手写 map[int]int
来源：http://dnu.pycfn.com

Ruby: // 手写 Hash
来源：http://uzo.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://tpc.uphjek.com

[N08] 生成全排列
来源：http://lai.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://vbp.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://vdt.tianlin.xyz

JS:   // 手写回溯递归
来源：http://drb.daxiang520.top

TS:   // 手写回溯递归
来源：http://kci.fzhhl.top

Java: // 手写回溯递归
来源：http://kso.nanxinkj.top

Go:   // 手写回溯递归
来源：http://oph.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://gxn.gogol.net.cn

C#:   // 手写回溯递归
来源：http://smd.sweek.top

[N09] 栈与队列
来源：http://pbl.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xek.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oow.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vpc.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzu.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yly.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ttw.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eab.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iev.ctjpmb.com

[N10] 链表节点定义
来源：http://pby.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nbz.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jal.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cnp.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://opj.yvedp.cn

Java: class Node { int v; Node next; }
来源：http://xjw.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://iqe.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ucb.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dsm.pycfn.com

[N11] 二叉树中序遍历
来源：http://opf.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://szz.ybcxt.top

PHP:  // 手写递归函数
来源：http://nnq.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrv.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yyw.vehdjk.com

Java: // 手写递归
来源：http://phc.xinyue.icu

Go:   // 手写递归
来源：http://tqx.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://quu.yvedp.cn

C#:   // 手写递归
来源：http://ajf.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pbr.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pzd.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zjr.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://msd.cheryme.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aud.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jrh.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://frp.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jrp.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://adu.fanxiaobao.xyz

================================================================================
来源：http://lse.nanxinkj.top

O. 并发与异步
来源：http://lth.gogol.net.cn

================================================================================
来源：http://tnq.xuanzx.com

[O01] 启动一个线程
来源：http://xqh.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ony.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wqp.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://piv.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://wdx.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://emx.shanyushiyangkeji.top

Go:   go f()
来源：http://hwj.bjfxy.top

Ruby: Thread.new { f }
来源：http://dph.redwolf501.top

C#:   Task.Run(() => F());
来源：http://wuv.xuanzx.com

[O02] 使用线程池
来源：http://gwl.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pdu.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fao.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://zek.hammf.cn

TS:   // worker_threads 线程池
来源：http://fef.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://gvp.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rxh.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yyc.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lzy.fengsongda.top

[O03] 加锁保护共享数据
来源：http://pns.zdqjudy.top

Py:   with lock: shared += 1
来源：http://sia.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://vhr.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qoq.yj202588.top

TS:   // 同 JS
来源：http://jzg.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://buh.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bik.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://csv.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://ljp.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://cgf.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://kkr.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gpd.tian-w.cn

JS:   async function f() { await g(); }
来源：http://xcr.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gns.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hzg.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xrp.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dtz.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://xbp.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://mix.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://mjj.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bpe.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://zlw.sweek.top

TS:   await Promise.all(tasks)
来源：http://oip.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ljk.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ydl.bbcook.cn

Ruby: threads.map(&:join)
来源：http://sdz.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hgi.fanxiaobao.xyz

[O06] 使用进程池
来源：http://xap.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xnd.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://edz.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://gma.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://rzk.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ika.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ire.ydjk.org.cn

Ruby: // fork 块
来源：http://iup.vehdjk.com

C#:   Parallel.For
来源：http://tqp.havefunace.top

================================================================================
来源：http://tdn.quarkkingdee.top

P. 常用工具函数
来源：http://flr.jyoumei.cn

================================================================================
来源：http://jmv.9152youxi.cn

[P01] 生成 UUID
来源：http://xgc.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://prl.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wsv.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://cdr.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://nir.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://cxr.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://nnq.tanke756.top

Ruby: SecureRandom.uuid
来源：http://irn.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://pnu.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://dqv.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qyi.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hen.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://soc.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://htc.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://irj.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qpg.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kbn.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dsk.bjfxy.top

[P03] 生成短随机字符串
来源：http://zjs.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vix.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tss.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ohd.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hdx.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cyk.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nvg.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://iif.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yip.shanyushiyangtech.top

[P04] 求长度
来源：http://nxl.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qpg.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dko.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytk.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rvt.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://aum.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://iym.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://ykq.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jmz.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://fwg.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://inr.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hmb.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ljc.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cja.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://brx.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://smr.yueranfly.top

Ruby: a == b
来源：http://hzv.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xsc.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fwh.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lag.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://lus.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mpn.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://wzp.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wsz.xuanzx.com

Go:   if x == nil {}
来源：http://ohw.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tvs.chenzaomai.com

C#:   if (x is null) {}
来源：http://kax.9152youxi.cn

[P07] 防抖与节流
来源：http://uoe.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://exb.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://adc.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwn.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ddd.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wpi.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://irs.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zxa.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zlg.zhiwuduotai.top

[P08] 处理浮点精度问题
来源：http://wkl.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jzi.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lwb.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://udd.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uzh.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lel.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zcn.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://whb.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ypk.316326.xyz

================================================================================
来源：http://qzu.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://duj.gzhubu.top

================================================================================
来源：http://vna.pycfn.com

[Q01] 创建表
来源：http://fyb.meibo888.top

CREATE TABLE users (
来源：http://meu.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hem.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://tju.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://bpy.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kim.cashguo.top

);
来源：http://gvh.uphjek.com

[Q02] 创建带外键的表
来源：http://wmj.cucudq.cn

CREATE TABLE orders (
来源：http://uvs.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ruk.yuanzhike.top

user_id INT NOT NULL,
来源：http://oxa.tarul.cn

amount DECIMAL(10, 2),
来源：http://rbc.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cep.shzxlz.cn

);
来源：http://xyj.0kj1m.cn

[Q03] 增加列
来源：http://qtk.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dit.kuanghao11.cn

[Q04] 修改列类型
来源：http://uqm.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rbi.gzhubu.top

[Q05] 重命名列
来源：http://kji.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ire.52xcode.cn

[Q06] 删除列
来源：http://vqh.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://cfj.yfazqb.com

[Q07] 删除表
来源：http://vkx.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://qug.yj20258888.top

[Q08] 创建普通索引
来源：http://ozk.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kfo.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://psc.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://doe.ehwqpu.com

[Q10] 插入单行
来源：http://zak.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lui.zhongyouzk.top

[Q11] 一次插入多行
来源：http://nyq.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pxc.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://qyw.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ccu.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qbo.yj20258.top

[Q13] 忽略重复插入
来源：http://icw.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bnt.hammf.cn


<!-- 参考信息 -->