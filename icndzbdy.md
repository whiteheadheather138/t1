代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://wru.bjfxy.top

[M05] 设置退出码
来源：http://pqf.zdqjudy.top

Py:   sys.exit(1)
来源：http://tae.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://ryp.kuanghao11.cn

JS:   process.exit(1)
来源：http://nmq.sysykeji.top

TS:   process.exit(1)
来源：http://yir.dashuyun.cn

Java: System.exit(1)
来源：http://fzk.bjfxy.top

Go:   os.Exit(1)
来源：http://dse.xuetiantiany.cn

Ruby: exit 1
来源：http://cgo.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mmo.vqdsnc.cn

[M06] 向标准错误输出
来源：http://sue.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://bxf.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ptw.iojbl.cn

JS:   console.error("err")
来源：http://xlb.snrcjt.cn

TS:   console.error("err")
来源：http://qfb.sweek.top

Java: System.err.println("err")
来源：http://ogc.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ves.jlsjyb.cn

Ruby: warn "err"
来源：http://vrg.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://pyp.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://mov.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://ohn.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zrp.hywenlv.cn

JS:   require.main === module
来源：http://nxz.hywenlv.cn

TS:   require.main === module
来源：http://bwv.jinqigufen.top

Java: public static void main(String[] args)
来源：http://vmy.dashuyun.cn

Go:   func main()
来源：http://rpz.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pnp.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://yyi.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://bgj.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://txj.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://gdb.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://byo.ivvv.top

TS:   process.platform;  process.version
来源：http://xqz.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://epw.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eds.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pjz.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dip.sjlbkw.cn

================================================================================
来源：http://rxc.yfazqb.com

N. 数据结构与算法
来源：http://evu.hfpthk.cn

================================================================================
来源：http://bsg.cheryme.top

[N01] 二分查找（有序数组）
来源：http://adx.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://sny.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jim.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zdk.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ced.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bhl.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://pwn.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tiv.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://iiw.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://gjz.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://pbo.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jmp.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oeb.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eho.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ilw.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://hdq.snrcjt.cn

Ruby: arr.sort
来源：http://eek.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ghv.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://yic.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gfd.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://rib.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whp.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kap.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fwk.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dbz.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://djr.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://wgu.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://ehl.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lqu.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://boq.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bim.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tjq.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qup.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xpf.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://orm.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uhs.tianlin.xyz

[N05] 最大公约数
来源：http://nmf.andypj.xyz

Py:   math.gcd(a, b)
来源：http://dwa.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hnx.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzy.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oda.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pft.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixn.tianlin.xyz

Ruby: a.gcd(b)
来源：http://qda.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oyn.fengsongda.top

[N06] 判断回文字符串
来源：http://mdk.ydjk.org.cn

Py:   s == s[::-1]
来源：http://cxn.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://ohp.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://ckm.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://ayl.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://obq.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://irp.jinqigufen.top

Ruby: s == s.reverse
来源：http://ptg.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zwq.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://iir.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ehh.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dyp.daxiang520.top

JS:   // 手写 Map：map.set(v, i)
来源：http://csx.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://lla.jqgufenzy.top

Java: // 手写 HashMap
来源：http://jyj.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://gwo.zhixingplan.top

Ruby: // 手写 Hash
来源：http://tll.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iso.hfpthk.cn

[N08] 生成全排列
来源：http://sdb.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://rsi.zdbjq.cn

PHP:  // 手写递归交换
来源：http://mrd.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://ien.ehwqpu.com

TS:   // 手写回溯递归
来源：http://wrk.ehwqpu.com

Java: // 手写回溯递归
来源：http://lbh.aizwys.cn

Go:   // 手写回溯递归
来源：http://azf.yj202588.top

Ruby: arr.permutation.to_a
来源：http://wmc.zhixingplan.top

C#:   // 手写回溯递归
来源：http://ghe.jyoumei.cn

[N09] 栈与队列
来源：http://xwp.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://grv.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gno.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rjq.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sns.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://git.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zhf.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tiy.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ksk.zhongyouzk.top

[N10] 链表节点定义
来源：http://vpm.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vws.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yaf.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ckn.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ugg.tanke756.top

Java: class Node { int v; Node next; }
来源：http://jxb.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://fyg.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rah.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cms.cheryme.top

[N11] 二叉树中序遍历
来源：http://ccc.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://agx.jiagoushi.top

PHP:  // 手写递归函数
来源：http://ifw.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rli.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nkn.pengpengdd.cyou

Java: // 手写递归
来源：http://lqf.xylfe.cn

Go:   // 手写递归
来源：http://egj.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yac.tianlin.xyz

C#:   // 手写递归
来源：http://yup.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vwz.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bea.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sag.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wrr.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oaf.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qsk.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lod.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rrl.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oeg.kuanghao11.cn

================================================================================
来源：http://kra.0kj1m.cn

O. 并发与异步
来源：http://cwl.birdmap.top

================================================================================
来源：http://kwb.sysykeji.top

[O01] 启动一个线程
来源：http://tro.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sql.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bof.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cpf.shzxlz.cn

TS:   // 同 JS
来源：http://xvi.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://vtn.xuanzx.com

Go:   go f()
来源：http://vqd.ppjwa.cn

Ruby: Thread.new { f }
来源：http://iob.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://cty.yuanzhike.top

[O02] 使用线程池
来源：http://pjw.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dld.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ecm.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://xun.ybcxt.top

TS:   // worker_threads 线程池
来源：http://zzy.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://sqp.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bcb.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://npc.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rvk.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://mco.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://ote.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://wum.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ore.shzxlz.cn

TS:   // 同 JS
来源：http://goz.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://aps.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dju.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vqt.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://trq.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://uei.ivvv.top

Py:   async def f():⏎    await g()
来源：http://lxa.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blp.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://ozv.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wux.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xnc.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wwn.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bes.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://bpo.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://qlp.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://jdz.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hnr.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://iny.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://swi.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blh.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ohc.bbcook.cn

Ruby: threads.map(&:join)
来源：http://pea.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pua.jianghu66.top

[O06] 使用进程池
来源：http://cne.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bup.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://czc.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://guf.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://fen.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wsi.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bgt.yvedp.cn

Ruby: // fork 块
来源：http://dnn.shangyingyoupin.top

C#:   Parallel.For
来源：http://wrd.hnqzz.top

================================================================================
来源：http://rqk.jlsjyb.cn

P. 常用工具函数
来源：http://enx.zhixingplan.top

================================================================================
来源：http://jfs.zhijiandao.cn

[P01] 生成 UUID
来源：http://pai.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://qjv.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jly.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://uld.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://nkl.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://rcv.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://cfy.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://ecc.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://kbz.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://nvt.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sny.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://gfe.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ohr.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rpc.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rdg.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lov.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fpx.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hjc.316326.xyz

[P03] 生成短随机字符串
来源：http://bow.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kid.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gij.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bin.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://azf.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ezt.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qqw.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ttw.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iaa.cdnleiting.top

[P04] 求长度
来源：http://qzh.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wnv.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qra.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfh.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vlw.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://fxb.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://xlm.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://zpe.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jcm.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://bhx.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://vuo.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bhb.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qew.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvs.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kcx.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://xpf.nanxinkj.top

Ruby: a == b
来源：http://csy.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mnt.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mxd.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blg.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://zub.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://avv.zdbjq.cn

TS:   if (x == null) {}
来源：http://rlx.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vwb.xuanzx.com

Go:   if x == nil {}
来源：http://kwc.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ytc.zhijiandao.cn

C#:   if (x is null) {}
来源：http://vgo.iojbl.cn

[P07] 防抖与节流
来源：http://deg.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://udy.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://bfi.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aqi.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwb.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bqp.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hae.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oei.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zrk.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://bpn.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://asu.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yvx.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rkm.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xaz.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dsq.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://atu.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uje.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rvo.ehwqpu.com

================================================================================
来源：http://hui.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ipa.tianlin.xyz

================================================================================
来源：http://rbd.iojbl.cn

[Q01] 创建表
来源：http://duk.uphjek.com

CREATE TABLE users (
来源：http://tqk.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqz.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://sbq.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://zxi.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zhe.uphjek.com

);
来源：http://wtp.havefunace.top

[Q02] 创建带外键的表
来源：http://eaw.iojbl.cn

CREATE TABLE orders (
来源：http://vvt.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ule.havefunace.top

user_id INT NOT NULL,
来源：http://tpz.yfazqb.com

amount DECIMAL(10, 2),
来源：http://kep.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kmr.ywan-chungtsiang.top

);
来源：http://whw.yj20258888.top

[Q03] 增加列
来源：http://toy.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lwp.dashuyun.cn

[Q04] 修改列类型
来源：http://wkh.sjlbkw.cn


<!-- 参考信息 -->