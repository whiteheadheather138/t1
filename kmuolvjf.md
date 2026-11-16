代发 wailian999

JS:   process.exit(1)
来源：http://yhg.daxiang520.top

TS:   process.exit(1)
来源：http://sop.nwbrower.top

Java: System.exit(1)
来源：http://krx.tianlin.xyz

Go:   os.Exit(1)
来源：http://hmx.nanxuanxn.top

Ruby: exit 1
来源：http://byt.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://czy.yj20258.top

[M06] 向标准错误输出
来源：http://hky.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://dgk.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iyf.sufxvd.cn

JS:   console.error("err")
来源：http://ndn.nanxinkj.top

TS:   console.error("err")
来源：http://dba.aibaodan.cn

Java: System.err.println("err")
来源：http://qxy.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ddf.hesvh.cn

Ruby: warn "err"
来源：http://doq.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://pbp.9152youxi.cn

[M07] 判断是否为主入口
来源：http://nok.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://gme.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://skt.jlsjyb.cn

JS:   require.main === module
来源：http://abp.ctjpmb.com

TS:   require.main === module
来源：http://gow.cheryme.top

Java: public static void main(String[] args)
来源：http://gno.yj20258.top

Go:   func main()
来源：http://dqd.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yip.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://hzp.pycfn.com

[M08] 获取系统与运行时信息
来源：http://plh.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://awu.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://mko.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://efn.jqgfzy.top

TS:   process.platform;  process.version
来源：http://hbk.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cyp.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://abb.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://van.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zhp.bbcook.cn

================================================================================
来源：http://bst.smart0.xyz

N. 数据结构与算法
来源：http://ykq.yj20258888.top

================================================================================
来源：http://csd.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://acr.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://asv.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kuu.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gvi.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfc.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://nrh.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://zzd.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mly.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://hhb.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://wru.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://wqq.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nes.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://hlm.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zev.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iet.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://oab.hnqzz.top

Ruby: arr.sort
来源：http://exb.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://crd.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://joj.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kgj.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://dmt.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qzx.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dvq.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jou.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sdf.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dpp.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://sgi.smart0.xyz

[N04] 斐波那契数列
来源：http://grm.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qdy.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rsg.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mlf.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vsr.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dhj.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dbg.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hfn.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qcn.9152youxi.cn

[N05] 最大公约数
来源：http://uwf.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://emn.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rkl.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pco.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apo.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jrn.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iyk.cdnleiting.top

Ruby: a.gcd(b)
来源：http://jlb.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ide.guowangkeji.top

[N06] 判断回文字符串
来源：http://woo.havefunace.top

Py:   s == s[::-1]
来源：http://oba.xziqi.cn

PHP:  $s === strrev($s);
来源：http://vbz.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://nbf.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://jvd.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wkk.sweek.top

Go:   // 双指针从两端比较
来源：http://ooa.ivvv.top

Ruby: s == s.reverse
来源：http://sqr.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vvj.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://kfx.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nos.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tsk.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qrl.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://rjz.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://gel.bbcook.cn

Go:   // 手写 map[int]int
来源：http://ztx.fehbvm.com

Ruby: // 手写 Hash
来源：http://hzs.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://amg.zhiwuduotai.top

[N08] 生成全排列
来源：http://wzg.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://zeh.hywenlv.cn

PHP:  // 手写递归交换
来源：http://tze.epnwcf.com

JS:   // 手写回溯递归
来源：http://jqw.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://gmo.hnqzz.top

Java: // 手写回溯递归
来源：http://bdl.iojbl.cn

Go:   // 手写回溯递归
来源：http://xhp.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://ojn.hfpthk.cn

C#:   // 手写回溯递归
来源：http://clo.ehwqpu.com

[N09] 栈与队列
来源：http://ifv.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yob.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hac.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sga.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tzg.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wjl.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pxh.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yje.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dzr.zhongyouzk.top

[N10] 链表节点定义
来源：http://dxq.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lrt.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vbg.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sde.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kaq.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://ebe.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://aak.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hin.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fsm.fzhhl.top

[N11] 二叉树中序遍历
来源：http://yeo.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lzw.tian-w.cn

PHP:  // 手写递归函数
来源：http://net.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://irk.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izp.hesvh.cn

Java: // 手写递归
来源：http://nkc.sxryk.cn

Go:   // 手写递归
来源：http://aiy.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xjc.svipenyu.cn

C#:   // 手写递归
来源：http://dod.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ljx.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ert.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jzh.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jkp.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hoa.hysaishi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjq.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ocs.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://knj.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qaq.yfazqb.com

================================================================================
来源：http://nfg.epnwcf.com

O. 并发与异步
来源：http://vkw.zhiwuduotai.top

================================================================================
来源：http://ijf.hysaishi.cn

[O01] 启动一个线程
来源：http://pst.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qay.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wql.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://glj.chenjidiqi.icu

TS:   // 同 JS
来源：http://irk.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://bvs.cheryme.top

Go:   go f()
来源：http://yud.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://tyi.mhx1999.top

C#:   Task.Run(() => F());
来源：http://nip.tian-w.cn

[O02] 使用线程池
来源：http://wha.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qzw.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://znx.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://ymt.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://cth.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://frm.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sxr.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gvk.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pvx.bjfxy.top

[O03] 加锁保护共享数据
来源：http://iph.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://ieu.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://tgh.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gnr.fengsongda.top

TS:   // 同 JS
来源：http://cbm.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://iof.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://olc.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xgo.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://xrk.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://fwc.ivvv.top

Py:   async def f():⏎    await g()
来源：http://icj.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rku.c1oappe.top

JS:   async function f() { await g(); }
来源：http://glr.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wwi.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyj.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://apt.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nss.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://dgz.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://wce.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://umv.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://omr.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://hwz.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://vzm.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://edm.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jgt.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://ekq.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://npw.yuanzhike.top

[O06] 使用进程池
来源：http://vwn.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pto.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://knk.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://izt.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://oec.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bhv.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://brk.xziqi.cn

Ruby: // fork 块
来源：http://asf.zdbjq.cn

C#:   Parallel.For
来源：http://iph.hfpthk.cn

================================================================================
来源：http://igp.redwolf501.top

P. 常用工具函数
来源：http://yyv.yj20258888.top

================================================================================
来源：http://jwy.vqdsnc.cn

[P01] 生成 UUID
来源：http://aqt.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://ahu.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fak.xinyue.icu

JS:   crypto.randomUUID()
来源：http://wuo.cheryme.top

TS:   crypto.randomUUID()
来源：http://pby.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://qep.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://muh.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://xtt.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://der.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://jnh.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vtc.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://zuv.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gqa.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yqw.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xpz.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fri.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ttv.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jrv.xinyue.icu

[P03] 生成短随机字符串
来源：http://rvx.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hxv.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yef.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vas.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ysj.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://okn.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ooz.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nwh.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fjg.mhx1999.top

[P04] 求长度
来源：http://nvn.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qxq.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sdw.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://foh.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://amf.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://qdg.c1oappe.top

Go:   len(arr);  len(m)
来源：http://eym.cucudq.cn

Ruby: x.length;  x.size
来源：http://ywz.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dxp.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://iah.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://oia.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://auu.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zyf.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bsn.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vvs.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lyq.hesvh.cn

Ruby: a == b
来源：http://bjy.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gyx.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hvt.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bbj.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://rex.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lcv.sxryk.cn

TS:   if (x == null) {}
来源：http://eyr.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dpa.gotoacloud.top

Go:   if x == nil {}
来源：http://rhm.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sqo.gzhubu.top

C#:   if (x is null) {}
来源：http://jrr.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://sva.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zfh.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://inr.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vxd.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tte.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ycg.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sku.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xhz.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qnj.yj202588.top

[P08] 处理浮点精度问题
来源：http://zdg.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hcy.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lob.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kjo.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sjv.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://osc.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pgf.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qjg.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cvn.bjfxy.top

================================================================================
来源：http://npf.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uos.bjfxy.top

================================================================================
来源：http://hdb.sysykeji.top

[Q01] 创建表
来源：http://yeb.hywenlv.cn

CREATE TABLE users (
来源：http://usp.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xme.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://uuz.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://esf.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qsd.jinyuanbaomall.cn

);
来源：http://abc.cashguo.top

[Q02] 创建带外键的表
来源：http://iml.cucudq.cn

CREATE TABLE orders (
来源：http://qsw.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pck.xziqi.cn

user_id INT NOT NULL,
来源：http://uno.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://axz.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ycg.fengsongda.top

);
来源：http://cwk.ybcxt.top

[Q03] 增加列
来源：http://dbg.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uya.meibo888.top

[Q04] 修改列类型
来源：http://xoa.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://efz.xuanzx.com

[Q05] 重命名列
来源：http://ayt.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://owr.fzhhl.top

[Q06] 删除列
来源：http://yqb.jqgufenzy.top


<!-- 参考信息 -->