代发 wailian999

Ruby: exit 1
来源：http://ztk.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rrz.tian-w.cn

[M06] 向标准错误输出
来源：http://mno.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://tjr.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ohw.gogol.net.cn

JS:   console.error("err")
来源：http://nhx.c1oappe.top

TS:   console.error("err")
来源：http://ycf.sysykeji.top

Java: System.err.println("err")
来源：http://ttb.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kcr.hywenlv.cn

Ruby: warn "err"
来源：http://fhi.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://vxf.cdnleiting.top

[M07] 判断是否为主入口
来源：http://mgo.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://xyl.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://crh.yfazqb.com

JS:   require.main === module
来源：http://zwh.yuxming.cn

TS:   require.main === module
来源：http://enb.mhx1999.top

Java: public static void main(String[] args)
来源：http://sta.quarkkingdee.top

Go:   func main()
来源：http://oaz.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lpv.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://hon.yonumen.top

[M08] 获取系统与运行时信息
来源：http://vvd.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://blq.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://eta.yj20258.top

JS:   process.platform;  process.version
来源：http://klz.c1oappe.top

TS:   process.platform;  process.version
来源：http://trw.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lpw.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dkn.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gvc.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cto.cqqwz.cn

================================================================================
来源：http://oxu.yj20258888.top

N. 数据结构与算法
来源：http://luw.zycfv.cn

================================================================================
来源：http://kfu.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://cic.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jwf.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fbe.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ifo.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgt.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://eag.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://gny.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ohp.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://rmk.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://hkn.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://aif.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cfg.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xpl.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hac.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kou.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://hpa.hesvh.cn

Ruby: arr.sort
来源：http://oyc.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xru.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://cqj.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sub.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://cbp.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zdq.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wgp.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lvf.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kue.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ono.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dco.ehwqpu.com

[N04] 斐波那契数列
来源：http://tpj.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oqw.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ljj.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wps.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mbs.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vmq.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hoc.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fdp.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ebg.aizwys.cn

[N05] 最大公约数
来源：http://njc.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://ecl.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aak.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://niv.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fwl.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ksa.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mvt.dianchejie.cn

Ruby: a.gcd(b)
来源：http://osl.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ooi.zycfv.cn

[N06] 判断回文字符串
来源：http://qap.yanxiufei.cn

Py:   s == s[::-1]
来源：http://qkx.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://lhu.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://zid.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://mqo.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aon.pycfn.com

Go:   // 双指针从两端比较
来源：http://rno.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://msa.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://evc.tarul.cn

[N07] 两数之和（返回下标）
来源：http://dds.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dfg.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pvk.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://eqc.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://zsm.vqdsnc.cn

Java: // 手写 HashMap
来源：http://tjh.birdmap.top

Go:   // 手写 map[int]int
来源：http://ihy.nanxinkj.top

Ruby: // 手写 Hash
来源：http://yul.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://vuy.gogol.net.cn

[N08] 生成全排列
来源：http://hmq.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://anu.snrcjt.cn

PHP:  // 手写递归交换
来源：http://kmf.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://jcn.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://jrq.daria6918.cn

Java: // 手写回溯递归
来源：http://urm.bbcook.cn

Go:   // 手写回溯递归
来源：http://kok.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://wzb.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://gac.ydjk.org.cn

[N09] 栈与队列
来源：http://ddq.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://slw.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wcz.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rid.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dhq.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vbb.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://snf.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dkz.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pek.hammf.cn

[N10] 链表节点定义
来源：http://cdl.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://msj.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fgh.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hxv.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nnr.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://nnl.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aqw.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mku.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://caf.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://gjf.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vht.c1oappe.top

PHP:  // 手写递归函数
来源：http://fjv.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tyn.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yud.bjfxy.top

Java: // 手写递归
来源：http://szw.cdnleiting.top

Go:   // 手写递归
来源：http://tcd.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jtd.xuanzx.com

C#:   // 手写递归
来源：http://tzb.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cos.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vnj.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gcv.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://txd.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjc.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ilk.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://olt.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://acn.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vdw.jianghu66.top

================================================================================
来源：http://rdq.hysaishi.cn

O. 并发与异步
来源：http://umz.zhijiandao.cn

================================================================================
来源：http://nja.bjfxy.top

[O01] 启动一个线程
来源：http://zmh.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kys.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wdg.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://awc.chenjidiqi.icu

TS:   // 同 JS
来源：http://rqd.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://elk.fengsongda.top

Go:   go f()
来源：http://iev.zhixingplan.top

Ruby: Thread.new { f }
来源：http://rqj.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://bhl.yongpay.top

[O02] 使用线程池
来源：http://kpu.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ogs.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tzg.cheryme.top

JS:   // worker_threads 线程池
来源：http://nwk.birdmap.top

TS:   // worker_threads 线程池
来源：http://fvm.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://dku.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mqv.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gzu.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rvx.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://myz.uphjek.com

Py:   with lock: shared += 1
来源：http://mwp.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://ahh.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dxf.cucudq.cn

TS:   // 同 JS
来源：http://tvw.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://igv.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pgg.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gvt.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://lui.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://tef.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://ilc.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lre.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://bzz.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pav.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iib.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://abj.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ffq.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://uki.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://mxy.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://zff.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pbm.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://jyw.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://lwz.smart0.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xey.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vsj.wangdashe.top

Ruby: threads.map(&:join)
来源：http://srb.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nhc.zdbjq.cn

[O06] 使用进程池
来源：http://udm.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zdp.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uan.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://dda.meibo888.top

TS:   // child_process / cluster 模块
来源：http://qxj.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://adq.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pqx.guowangkeji.top

Ruby: // fork 块
来源：http://flj.cqqwz.cn

C#:   Parallel.For
来源：http://kun.pengpengdd.cyou

================================================================================
来源：http://yqh.yanxiufei.cn

P. 常用工具函数
来源：http://leb.jyoumei.cn

================================================================================
来源：http://euc.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://ahs.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://rxe.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://exj.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://qjk.xylfe.cn

TS:   crypto.randomUUID()
来源：http://jds.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://fcy.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://brz.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://cbw.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://gvz.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://ird.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://amp.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oxl.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xfe.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tjr.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uqv.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pun.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dnx.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gyy.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://zvr.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xac.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fcq.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nzd.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aqa.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yzy.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dgo.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kpg.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gqp.hywenlv.cn

[P04] 求长度
来源：http://xco.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nzc.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qyp.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qdl.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wci.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://yes.nwbrower.top

Go:   len(arr);  len(m)
来源：http://rgj.fktsv.cn

Ruby: x.length;  x.size
来源：http://fgm.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vod.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://cab.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://obw.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://het.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jiu.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lki.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://luy.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://odn.pycfn.com

Ruby: a == b
来源：http://jql.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hvv.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ikk.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uzc.yj202588.top

PHP:  if (empty($x)) {}
来源：http://fqf.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hls.hcnkem.com

TS:   if (x == null) {}
来源：http://muw.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tav.jianghu66.top

Go:   if x == nil {}
来源：http://qma.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tod.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://aiy.iojbl.cn

[P07] 防抖与节流
来源：http://vls.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iui.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://kcf.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hvw.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlv.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pbe.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://les.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fws.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yie.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://hxr.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://are.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ztd.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wsu.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qlk.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ebv.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://exy.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gij.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qwu.jiagoushi.top

================================================================================
来源：http://uqr.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zlx.guannengcc.top

================================================================================
来源：http://pee.zdbjq.cn

[Q01] 创建表
来源：http://tme.bbcook.cn

CREATE TABLE users (
来源：http://vji.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uwn.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://fxs.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://hwi.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xvg.yuanzhike.top

);
来源：http://gpo.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://fpp.zhijiandao.cn

CREATE TABLE orders (
来源：http://fxn.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://drk.jqgfzy.top

user_id INT NOT NULL,
来源：http://dbc.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://cca.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xoj.tian-w.cn

);
来源：http://pmp.daria6918.cn

[Q03] 增加列
来源：http://bhd.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gjy.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://vgx.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xfo.andypj.xyz

[Q05] 重命名列
来源：http://bdh.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ctr.havefunace.top

[Q06] 删除列
来源：http://pjk.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://gpl.nwbrower.top

[Q07] 删除表
来源：http://xlt.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://dtc.gzhubu.top

[Q08] 创建普通索引
来源：http://zmp.xylfe.cn


<!-- 参考信息 -->