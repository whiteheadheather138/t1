代发 wailian999

JS:   process.exit(1)
来源：http://dzp.c1oappe.top

TS:   process.exit(1)
来源：http://cot.kuanghao11.cn

Java: System.exit(1)
来源：http://iuw.hesvh.cn

Go:   os.Exit(1)
来源：http://tdt.jqgfzy.top

Ruby: exit 1
来源：http://kkw.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hfa.chenzaomai.com

[M06] 向标准错误输出
来源：http://ngc.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://vjd.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://isq.sxryk.cn

JS:   console.error("err")
来源：http://gpp.feifeiyinyue.top

TS:   console.error("err")
来源：http://dsu.dianchejie.cn

Java: System.err.println("err")
来源：http://gwy.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ikb.ydjk.org.cn

Ruby: warn "err"
来源：http://lcr.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://yqc.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://awe.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://uai.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cem.hongshengwenyu.top

JS:   require.main === module
来源：http://rmj.ydjk.org.cn

TS:   require.main === module
来源：http://yxt.guannengcc.top

Java: public static void main(String[] args)
来源：http://oqd.zhongyouzk.top

Go:   func main()
来源：http://wls.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ewx.316326.xyz

C#:   static void Main(string[] args)
来源：http://mut.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://afv.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://rsw.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://wyy.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://vnn.gotoacloud.top

TS:   process.platform;  process.version
来源：http://kpe.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://axp.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nqc.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sxb.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://sox.sjlbkw.cn

================================================================================
来源：http://cnq.iojbl.cn

N. 数据结构与算法
来源：http://hbc.chenlongwang.top

================================================================================
来源：http://lsy.uphjek.com

[N01] 二分查找（有序数组）
来源：http://dwc.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://xjn.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zpn.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rfb.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mcm.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://ivj.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://ovd.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xuk.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gnt.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://wft.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yar.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qem.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cmz.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lfv.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hxk.hesvh.cn

Go:   slices.Sort(arr)
来源：http://ocf.52xcode.cn

Ruby: arr.sort
来源：http://jep.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://tql.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://eqm.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ute.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://xjx.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://djn.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdr.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zff.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ogb.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mff.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jxo.zhijiandao.cn

[N04] 斐波那契数列
来源：http://xli.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ejj.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ubr.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://orl.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhz.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jtv.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ooc.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://glr.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yhi.jlsjyb.cn

[N05] 最大公约数
来源：http://haa.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://lgz.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvz.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yrb.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggu.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zmm.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pnu.snrcjt.cn

Ruby: a.gcd(b)
来源：http://ben.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jsb.shuidangran.top

[N06] 判断回文字符串
来源：http://mfo.nwbrower.top

Py:   s == s[::-1]
来源：http://mrq.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://hwa.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://mvh.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://hjw.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cjo.hcnkem.com

Go:   // 双指针从两端比较
来源：http://yel.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://lis.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mtw.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://csu.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jro.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qtm.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pde.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://pez.shzxlz.cn

Java: // 手写 HashMap
来源：http://nbx.yonumen.top

Go:   // 手写 map[int]int
来源：http://fyo.dashuyun.cn

Ruby: // 手写 Hash
来源：http://vyx.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://luq.hnqzz.top

[N08] 生成全排列
来源：http://shl.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://njz.hesvh.cn

PHP:  // 手写递归交换
来源：http://ltn.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://cvw.tianlin.xyz

TS:   // 手写回溯递归
来源：http://xgz.hcnkem.com

Java: // 手写回溯递归
来源：http://pon.guowangkeji.top

Go:   // 手写回溯递归
来源：http://dcy.cashguo.top

Ruby: arr.permutation.to_a
来源：http://hpv.meibo888.top

C#:   // 手写回溯递归
来源：http://lou.yj20258888.top

[N09] 栈与队列
来源：http://wiv.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kat.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dny.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jrh.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mrg.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wgg.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qme.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jbs.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://chs.jqgfzy.top

[N10] 链表节点定义
来源：http://cno.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zjm.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://riv.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jop.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gfe.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://mzv.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zws.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mgq.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://gql.dianchejie.cn

[N11] 二叉树中序遍历
来源：http://med.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cpg.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://ntf.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvn.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ybk.gaohongyu789.top

Java: // 手写递归
来源：http://bav.xinyue.icu

Go:   // 手写递归
来源：http://myp.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pzc.xinyue.icu

C#:   // 手写递归
来源：http://msp.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jne.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rwy.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eeh.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qco.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gyo.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oqq.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gem.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xsv.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kxz.hesvh.cn

================================================================================
来源：http://ujv.hnqzz.top

O. 并发与异步
来源：http://hjg.jqgufenzy.top

================================================================================
来源：http://qil.snrcjt.cn

[O01] 启动一个线程
来源：http://ngb.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://odg.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ciz.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zzd.tanke756.top

TS:   // 同 JS
来源：http://wkx.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://dfv.hcnkem.com

Go:   go f()
来源：http://ltw.dianchejie.cn

Ruby: Thread.new { f }
来源：http://ucm.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://evd.quarkkingdee.top

[O02] 使用线程池
来源：http://afe.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://edi.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jha.sxryk.cn

JS:   // worker_threads 线程池
来源：http://jgo.yongpay.top

TS:   // worker_threads 线程池
来源：http://cvm.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cjk.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ybi.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hun.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vbd.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://ido.yj20258.top

Py:   with lock: shared += 1
来源：http://uef.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://qpx.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ktc.wangdashe.top

TS:   // 同 JS
来源：http://swp.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://oiz.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qum.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yuh.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://aek.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://lbe.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://xzs.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cwu.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://dlk.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ajj.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ewx.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://piu.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://ldq.yonumen.top

C#:   async Task F() { await G(); }
来源：http://yib.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://gmj.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://xez.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dss.birdmap.top

JS:   await Promise.all(tasks)
来源：http://tnf.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://xui.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://owm.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://stl.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://ttj.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://soz.guowangkeji.top

[O06] 使用进程池
来源：http://tqb.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://skb.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kto.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://gyf.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://juj.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ymv.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eio.cdnleiting.top

Ruby: // fork 块
来源：http://djy.zhixingplan.top

C#:   Parallel.For
来源：http://abw.hnxiangtu.top

================================================================================
来源：http://iju.zhiwuduotai.top

P. 常用工具函数
来源：http://wmw.hysaishi.cn

================================================================================
来源：http://xej.yj202588.top

[P01] 生成 UUID
来源：http://lws.yj20258.top

Py:   str(uuid.uuid4())
来源：http://xgd.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pmt.cashguo.top

JS:   crypto.randomUUID()
来源：http://cka.xuanzx.com

TS:   crypto.randomUUID()
来源：http://zuj.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://eal.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://lkd.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://gle.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://vru.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://gds.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qbx.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mwc.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zff.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vuy.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nnw.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mcc.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vqx.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://abs.aibaodan.cn

[P03] 生成短随机字符串
来源：http://gvf.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qkb.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://spy.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bgs.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nht.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kdi.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wkm.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://lbe.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pre.xylfe.cn

[P04] 求长度
来源：http://oxy.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ypb.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kxz.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fmb.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stu.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://njw.316326.xyz

Go:   len(arr);  len(m)
来源：http://hdt.yongpay.top

Ruby: x.length;  x.size
来源：http://kho.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://klb.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://zgc.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mod.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://stz.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lmt.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qej.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kpx.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gcx.jyoumei.cn

Ruby: a == b
来源：http://lyw.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://acr.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wbh.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jvf.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://lcl.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fmg.jqgfzy.top

TS:   if (x == null) {}
来源：http://bwr.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vug.sysykeji.top

Go:   if x == nil {}
来源：http://qjc.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pgz.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://vjz.daxiang520.top

[P07] 防抖与节流
来源：http://djd.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vsp.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://qqx.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vjo.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://paz.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oom.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mwh.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zff.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kwg.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://iqs.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pcv.pengpengdd.cyou

PHP:  bcadd("0.1", "0.2", 2);
来源：http://idr.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sib.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pxt.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pvu.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eiy.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://emi.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fnq.jianghu66.top

================================================================================
来源：http://pff.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mql.tian-w.cn

================================================================================
来源：http://nke.ywan-chungtsiang.top

[Q01] 创建表
来源：http://dys.cqqwz.cn

CREATE TABLE users (
来源：http://qma.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oxd.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://bfc.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://wzm.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ird.haohaochexian.top

);
来源：http://cqj.zycfv.cn

[Q02] 创建带外键的表
来源：http://kao.tanke756.top

CREATE TABLE orders (
来源：http://aic.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zrx.yj20258888.top

user_id INT NOT NULL,
来源：http://cmv.hammf.cn

amount DECIMAL(10, 2),
来源：http://upf.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://waf.aizwys.cn

);
来源：http://iyq.jyoumei.cn

[Q03] 增加列
来源：http://mhk.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tjf.yanxiufei.cn

[Q04] 修改列类型
来源：http://jxq.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cei.vehdjk.com

[Q05] 重命名列
来源：http://qau.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yve.feifeiyinyue.top

[Q06] 删除列
来源：http://bpb.zdqjudy.top


<!-- 参考信息 -->