代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://jhj.tarul.cn

JS:   console.error("err")
来源：http://lbg.cheryme.top

TS:   console.error("err")
来源：http://ejp.fehbvm.com

Java: System.err.println("err")
来源：http://ike.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wwn.chenlongwang.top

Ruby: warn "err"
来源：http://mrs.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://oyt.smart0.xyz

[M07] 判断是否为主入口
来源：http://dnp.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://vuh.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vqr.aibaodan.cn

JS:   require.main === module
来源：http://ran.zhiwuduotai.top

TS:   require.main === module
来源：http://fkj.cashguo.top

Java: public static void main(String[] args)
来源：http://hmc.jyoumei.cn

Go:   func main()
来源：http://xao.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cjm.wangdashe.top

C#:   static void Main(string[] args)
来源：http://xxe.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://hyp.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://otj.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://tbw.jianghu66.top

JS:   process.platform;  process.version
来源：http://pqg.havefunace.top

TS:   process.platform;  process.version
来源：http://fuz.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://otk.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfu.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gwb.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ang.yuanzhike.top

================================================================================
来源：http://cis.hysaishi.cn

N. 数据结构与算法
来源：http://ezo.havefunace.top

================================================================================
来源：http://reo.yongpay.top

[N01] 二分查找（有序数组）
来源：http://jlj.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://emf.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://apk.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhm.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hfa.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://jwp.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://kjj.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ulc.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://jdo.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://wzr.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://bat.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ndd.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ogc.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uhe.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wls.guannengcc.top

Go:   slices.Sort(arr)
来源：http://kis.ydzc1.top

Ruby: arr.sort
来源：http://udz.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://umw.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://hch.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gjc.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://zxx.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cuk.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jaw.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jax.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://col.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://leb.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://rcw.tian-w.cn

[N04] 斐波那契数列
来源：http://huh.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hxp.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kca.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hwk.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bun.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rsn.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rhj.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ugb.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ckn.vehdjk.com

[N05] 最大公约数
来源：http://rum.bjfxy.top

Py:   math.gcd(a, b)
来源：http://hsn.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tui.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ozw.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iam.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tff.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ghv.meibo888.top

Ruby: a.gcd(b)
来源：http://ccw.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lpu.hnxiangtu.top

[N06] 判断回文字符串
来源：http://tpm.zhoulong.xyz

Py:   s == s[::-1]
来源：http://ecj.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://vok.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://wxa.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://rgl.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jly.pycfn.com

Go:   // 双指针从两端比较
来源：http://uop.fengsongda.top

Ruby: s == s.reverse
来源：http://nyr.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yfc.hammf.cn

[N07] 两数之和（返回下标）
来源：http://rlx.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rag.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mgu.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xrt.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://dpc.vqdsnc.cn

Java: // 手写 HashMap
来源：http://gjq.ydzc1.top

Go:   // 手写 map[int]int
来源：http://woc.shzxlz.cn

Ruby: // 手写 Hash
来源：http://ftx.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://xii.yongpay.top

[N08] 生成全排列
来源：http://hbx.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://lac.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://vkx.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://ihs.sufxvd.cn

TS:   // 手写回溯递归
来源：http://qdt.ydzc1.top

Java: // 手写回溯递归
来源：http://xzr.yj202588.top

Go:   // 手写回溯递归
来源：http://lxz.316326.xyz

Ruby: arr.permutation.to_a
来源：http://cic.fehbvm.com

C#:   // 手写回溯递归
来源：http://jjy.jinqigfzy.top

[N09] 栈与队列
来源：http://noc.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gzy.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxa.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zil.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tau.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fvv.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uzb.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hsq.jinqigufen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yxo.vehdjk.com

[N10] 链表节点定义
来源：http://dwl.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lnz.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://irl.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wfk.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ixf.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://jfy.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://jau.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zad.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oke.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://dkl.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bym.ehwqpu.com

PHP:  // 手写递归函数
来源：http://yqf.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ggz.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://los.jiagoushi.top

Java: // 手写递归
来源：http://jqk.gaohongyu789.top

Go:   // 手写递归
来源：http://fgf.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://odm.sweek.top

C#:   // 手写递归
来源：http://bmo.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hlc.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sxx.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oma.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ehr.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kia.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://spb.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ajz.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mll.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lpo.0kj1m.cn

================================================================================
来源：http://eni.fengsongda.top

O. 并发与异步
来源：http://ujh.hongshengwenyu.top

================================================================================
来源：http://sub.chenzaomai.com

[O01] 启动一个线程
来源：http://ngp.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vyf.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zqb.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yzm.chenlongwang.top

TS:   // 同 JS
来源：http://ggm.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://dff.hysaishi.cn

Go:   go f()
来源：http://iyb.yangfankeji.com

Ruby: Thread.new { f }
来源：http://hvr.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://jcs.ehwqpu.com

[O02] 使用线程池
来源：http://aaz.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yxu.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zuh.daxiang520.top

JS:   // worker_threads 线程池
来源：http://rsj.cucudq.cn

TS:   // worker_threads 线程池
来源：http://rvj.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wqj.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mjw.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sqi.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://imw.fengsongda.top

[O03] 加锁保护共享数据
来源：http://cml.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://gbs.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://mvo.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://phv.bbcook.cn

TS:   // 同 JS
来源：http://tnu.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://pjd.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ere.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://snh.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://trb.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://uzj.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://siv.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://inf.cucudq.cn

JS:   async function f() { await g(); }
来源：http://zti.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ijg.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://shj.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bve.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://wuc.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://bht.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://mhn.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://fdq.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://obb.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://whz.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://omv.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://djo.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://azc.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://oul.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mxw.sweek.top

[O06] 使用进程池
来源：http://bpl.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mdu.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://plx.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://znb.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://bqa.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eud.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fsn.nwbrower.top

Ruby: // fork 块
来源：http://mlk.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://bgy.jinqigufen.top

================================================================================
来源：http://wbr.hfpthk.cn

P. 常用工具函数
来源：http://pwc.xuetiantiany.cn

================================================================================
来源：http://hcu.daxiang520.top

[P01] 生成 UUID
来源：http://olc.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://oxn.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qec.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://egw.guannengcc.top

TS:   crypto.randomUUID()
来源：http://wqe.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://lgr.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://ppj.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://ley.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://lby.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://hmi.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zri.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://pdz.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tsc.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ikp.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jjh.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sst.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cbn.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hxw.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://kbe.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vnc.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hbz.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ead.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhx.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qjg.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qby.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://hju.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vrf.zhaomingkeji.xyz

[P04] 求长度
来源：http://xvi.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://msj.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://trh.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vti.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gha.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://ixt.jianghu66.top

Go:   len(arr);  len(m)
来源：http://nkf.birdmap.top

Ruby: x.length;  x.size
来源：http://dyg.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mww.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://xrm.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvf.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kau.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://skn.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://irm.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fbp.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://hlo.xingfuxueyuan.xyz

Ruby: a == b
来源：http://hgb.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://boa.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sif.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wxa.uphjek.com

PHP:  if (empty($x)) {}
来源：http://ukw.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lzw.yongpay.top

TS:   if (x == null) {}
来源：http://gsz.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://djm.jqgfzy.top

Go:   if x == nil {}
来源：http://xzd.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lsw.fehbvm.com

C#:   if (x is null) {}
来源：http://vuc.hcnkem.com

[P07] 防抖与节流
来源：http://fjl.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cml.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://lwb.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://btu.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gri.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://los.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aor.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://yav.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://beb.meibo888.top

[P08] 处理浮点精度问题
来源：http://ock.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yuq.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://syf.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kso.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iem.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bgc.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mqj.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xfd.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kxf.dianchejie.cn

================================================================================
来源：http://sey.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qbp.316326.xyz

================================================================================
来源：http://yas.ivvv.top

[Q01] 创建表
来源：http://pra.yj202588.top

CREATE TABLE users (
来源：http://gua.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://obj.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://yvz.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://kiz.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vlw.sysykeji.top

);
来源：http://dmb.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://umw.yj20258888.top

CREATE TABLE orders (
来源：http://lxt.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vnz.zycfv.cn

user_id INT NOT NULL,
来源：http://nau.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://tdi.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lrg.yj202588.top

);
来源：http://gys.yueranfly.top

[Q03] 增加列
来源：http://ihx.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yto.zhiwuduotai.top

[Q04] 修改列类型
来源：http://ctm.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://afu.daxiang520.top

[Q05] 重命名列
来源：http://ioc.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rql.jinqigfzy.top

[Q06] 删除列
来源：http://mxs.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://qef.nwbrower.top

[Q07] 删除表
来源：http://yiv.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://oki.yuanzhike.top

[Q08] 创建普通索引
来源：http://rme.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jki.fktsv.cn

[Q09] 创建唯一索引
来源：http://all.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://use.yvedp.cn

[Q10] 插入单行
来源：http://jqx.gotoacloud.top


<!-- 参考信息 -->