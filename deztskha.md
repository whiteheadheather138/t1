代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://afb.smart0.xyz

Ruby: warn "err"
来源：http://tsm.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://gxd.pycfn.com

[M07] 判断是否为主入口
来源：http://fas.ivvv.top

Py:   if __name__ == "__main__":
来源：http://kwy.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qah.daxiang520.top

JS:   require.main === module
来源：http://blg.mhx1999.top

TS:   require.main === module
来源：http://ucw.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://eqi.fehbvm.com

Go:   func main()
来源：http://wbc.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://trr.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://qmj.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://sue.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://bwk.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://hne.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://xlz.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://yvb.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eur.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gzt.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tzn.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xqv.gaohongyu789.top

================================================================================
来源：http://euk.hnqzz.top

N. 数据结构与算法
来源：http://fdz.hfpthk.cn

================================================================================
来源：http://hlc.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://gft.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://wep.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://luh.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fuq.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugm.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cdg.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://fqo.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://csw.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://ple.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://cfb.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://mnc.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ksk.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://myc.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eyd.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pgz.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://tyy.yvedp.cn

Ruby: arr.sort
来源：http://ers.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://fan.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://hlm.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wwd.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://nci.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qbd.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahu.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://slw.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rpe.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qta.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pfa.bbcook.cn

[N04] 斐波那契数列
来源：http://vip.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vvd.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzo.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsw.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmt.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lel.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hss.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cis.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tsl.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://alk.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://czy.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jzk.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hvy.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thu.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hyt.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wew.jiagoushi.top

Ruby: a.gcd(b)
来源：http://eap.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cgm.shzxlz.cn

[N06] 判断回文字符串
来源：http://fug.shzxlz.cn

Py:   s == s[::-1]
来源：http://vyk.52xcode.cn

PHP:  $s === strrev($s);
来源：http://jpu.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://ndb.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://sib.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kte.xylfe.cn

Go:   // 双指针从两端比较
来源：http://qhl.cqqwz.cn

Ruby: s == s.reverse
来源：http://fep.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qqr.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://nlg.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mmt.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eov.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://skb.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://vnf.xziqi.cn

Java: // 手写 HashMap
来源：http://ttg.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://nrk.hywenlv.cn

Ruby: // 手写 Hash
来源：http://rvl.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://hjx.xuanzx.com

[N08] 生成全排列
来源：http://vrq.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://nyv.xziqi.cn

PHP:  // 手写递归交换
来源：http://xrt.cucudq.cn

JS:   // 手写回溯递归
来源：http://sie.hnqzz.top

TS:   // 手写回溯递归
来源：http://wcd.jyoumei.cn

Java: // 手写回溯递归
来源：http://wce.hfpthk.cn

Go:   // 手写回溯递归
来源：http://ljv.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://ccf.zhixingplan.top

C#:   // 手写回溯递归
来源：http://jpi.haohaochexian.top

[N09] 栈与队列
来源：http://ssn.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gsa.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qll.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hcb.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bdx.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wls.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pew.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aqb.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnx.zdqjudy.top

[N10] 链表节点定义
来源：http://wrf.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xen.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uai.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://znw.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bqr.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://ryt.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bfm.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bsr.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lvg.cheryme.top

[N11] 二叉树中序遍历
来源：http://rjm.sysykeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yqg.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://mwp.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzu.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kle.meibo888.top

Java: // 手写递归
来源：http://xjl.fehbvm.com

Go:   // 手写递归
来源：http://hwx.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pzd.havefunace.top

C#:   // 手写递归
来源：http://nzv.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aac.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hnd.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pla.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sic.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ddz.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ynm.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gdr.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eas.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qho.cheryme.top

================================================================================
来源：http://zmm.yonumen.top

O. 并发与异步
来源：http://lgn.haohaochexian.top

================================================================================
来源：http://cys.ehwqpu.com

[O01] 启动一个线程
来源：http://vbg.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ebr.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kou.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xop.nanxinkj.top

TS:   // 同 JS
来源：http://ewf.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://upt.shangyingyoupin.top

Go:   go f()
来源：http://qhw.guowangkeji.top

Ruby: Thread.new { f }
来源：http://opl.zycfv.cn

C#:   Task.Run(() => F());
来源：http://evd.jqgufenzy.top

[O02] 使用线程池
来源：http://ovu.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rkb.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gfs.cheryme.top

JS:   // worker_threads 线程池
来源：http://xst.aizwys.cn

TS:   // worker_threads 线程池
来源：http://uyk.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://vqn.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://frt.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tln.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oer.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://uah.tarul.cn

Py:   with lock: shared += 1
来源：http://had.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://fff.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ves.cheryme.top

TS:   // 同 JS
来源：http://yqm.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://bvy.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yxw.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lrq.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://gpm.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://xtb.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://ncf.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ejt.mhx1999.top

JS:   async function f() { await g(); }
来源：http://suf.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ugd.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hzy.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oze.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://rnr.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://vsy.quarkkingdee.top

[O05] 并发执行并等待全部完成
来源：http://vbp.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://dwh.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oeh.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://tia.tarul.cn

TS:   await Promise.all(tasks)
来源：http://bym.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rco.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tga.fengsongda.top

Ruby: threads.map(&:join)
来源：http://cpd.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ayv.tian-w.cn

[O06] 使用进程池
来源：http://izx.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uyq.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ezw.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://pan.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://ftb.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mmz.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nkr.zdbjq.cn

Ruby: // fork 块
来源：http://rrf.jiagoushi.top

C#:   Parallel.For
来源：http://rwj.fehbvm.com

================================================================================
来源：http://eyj.gotoacloud.top

P. 常用工具函数
来源：http://glj.gaohongyu789.top

================================================================================
来源：http://qfk.yanxiufei.cn

[P01] 生成 UUID
来源：http://boo.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://kes.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mei.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://jlc.tarul.cn

TS:   crypto.randomUUID()
来源：http://isd.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://yay.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://tqi.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://dwd.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://ztt.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://nmu.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uyp.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yly.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pum.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ryz.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lhn.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hdg.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lxi.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://imb.fzhhl.top

[P03] 生成短随机字符串
来源：http://tzg.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xoi.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ddt.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bim.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gsw.hammf.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pbu.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aid.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wma.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ral.fehbvm.com

[P04] 求长度
来源：http://wqd.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jtu.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mza.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xhs.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rle.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://kur.cashguo.top

Go:   len(arr);  len(m)
来源：http://ojo.xinyue.icu

Ruby: x.length;  x.size
来源：http://tig.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vhh.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://xtq.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gfb.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sni.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gbz.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cqm.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nmw.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vvb.daxiang520.top

Ruby: a == b
来源：http://fob.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://obf.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sli.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://krz.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://fow.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mky.fzhhl.top

TS:   if (x == null) {}
来源：http://hdl.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hlf.fehbvm.com

Go:   if x == nil {}
来源：http://tmx.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uty.quarkkingdee.top

C#:   if (x is null) {}
来源：http://oop.jqgfzy.top

[P07] 防抖与节流
来源：http://amz.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jaf.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://hzs.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqn.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhc.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aby.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://foa.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rte.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://trg.xylfe.cn

[P08] 处理浮点精度问题
来源：http://cvt.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eau.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cxm.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dgh.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rcf.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pur.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nec.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://czu.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nky.zhongyouzk.top

================================================================================
来源：http://txc.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vie.316326.xyz

================================================================================
来源：http://oqo.guannengcc.top

[Q01] 创建表
来源：http://aip.svipenyu.cn

CREATE TABLE users (
来源：http://onf.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qzh.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://lfr.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://nqy.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lus.guowangkeji.top

);
来源：http://kme.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://zwn.aibaodan.cn

CREATE TABLE orders (
来源：http://fjr.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sit.hcnkem.com

user_id INT NOT NULL,
来源：http://dvq.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://scd.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ull.cashguo.top

);
来源：http://hor.jiagoushi.top

[Q03] 增加列
来源：http://smc.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xwn.zhengqikj.top

[Q04] 修改列类型
来源：http://nvg.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cwa.guowangkeji.top

[Q05] 重命名列
来源：http://yef.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wfg.haohaochexian.top

[Q06] 删除列
来源：http://xpv.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://cif.9152youxi.cn

[Q07] 删除表
来源：http://wjl.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://pkt.gotoacloud.top

[Q08] 创建普通索引
来源：http://yja.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hpp.jianghu66.top

[Q09] 创建唯一索引
来源：http://xrr.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nrf.gogol.net.cn

[Q10] 插入单行
来源：http://fct.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pqq.sufxvd.cn

[Q11] 一次插入多行
来源：http://syv.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jrm.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://jgs.jinqigufen.top


<!-- 参考信息 -->