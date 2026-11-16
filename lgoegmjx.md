代发 wailian999

JS:   process.exit(1)
来源：http://mtw.fktsv.cn

TS:   process.exit(1)
来源：http://nda.jianghu66.top

Java: System.exit(1)
来源：http://xzq.hnxiangtu.top

Go:   os.Exit(1)
来源：http://dgx.jinqigufen.top

Ruby: exit 1
来源：http://ewm.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gwg.zdbjq.cn

[M06] 向标准错误输出
来源：http://kwi.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://rdp.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://kcj.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://jue.hnqzz.top

TS:   console.error("err")
来源：http://yqc.tian-w.cn

Java: System.err.println("err")
来源：http://xrl.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jaz.aibaodan.cn

Ruby: warn "err"
来源：http://ipi.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://wmz.wangdashe.top

[M07] 判断是否为主入口
来源：http://onl.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://geu.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfk.sweek.top

JS:   require.main === module
来源：http://rst.9152youxi.cn

TS:   require.main === module
来源：http://dtt.vehdjk.com

Java: public static void main(String[] args)
来源：http://urq.quarkkingdee.top

Go:   func main()
来源：http://dsx.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://liw.vehdjk.com

C#:   static void Main(string[] args)
来源：http://upe.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://ncb.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://npo.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://mkc.xuanzx.com

JS:   process.platform;  process.version
来源：http://txx.jiagoushi.top

TS:   process.platform;  process.version
来源：http://xwq.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kyp.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://olq.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://puu.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rkj.yuanzhike.top

================================================================================
来源：http://bbd.chenjidiqi.icu

N. 数据结构与算法
来源：http://luc.hnqzz.top

================================================================================
来源：http://rtg.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://hfb.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gvp.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://itp.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipc.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xtj.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://yfw.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://gsd.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ren.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cet.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://moa.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://knk.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sbb.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xhj.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bcv.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tdl.mhx1999.top

Go:   slices.Sort(arr)
来源：http://lod.ybcxt.top

Ruby: arr.sort
来源：http://kcv.haohaochexian.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ccf.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://hlg.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://duj.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://qgs.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://atj.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cob.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fqv.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xan.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dlj.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dsv.zhongyouzk.top

[N04] 斐波那契数列
来源：http://fqf.cdnleiting.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nrk.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nfu.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qtn.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rrh.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tuz.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dhk.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qmn.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bxy.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://ugx.yueranfly.top

Py:   math.gcd(a, b)
来源：http://cvk.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://azo.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zej.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fuy.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jjo.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://azp.zhixingplan.top

Ruby: a.gcd(b)
来源：http://arj.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hhv.tarul.cn

[N06] 判断回文字符串
来源：http://rga.xziqi.cn

Py:   s == s[::-1]
来源：http://nyh.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://sll.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://gsk.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://zgz.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cdw.nwbrower.top

Go:   // 双指针从两端比较
来源：http://yyd.nwbrower.top

Ruby: s == s.reverse
来源：http://oge.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ybp.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://mnu.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sjg.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jyi.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dqt.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://isd.dianchejie.cn

Java: // 手写 HashMap
来源：http://grs.hammf.cn

Go:   // 手写 map[int]int
来源：http://yym.ivvv.top

Ruby: // 手写 Hash
来源：http://ozf.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qjf.fanxiaobao.xyz

[N08] 生成全排列
来源：http://rjr.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://qbc.hysaishi.cn

PHP:  // 手写递归交换
来源：http://jyl.svipenyu.cn

JS:   // 手写回溯递归
来源：http://ktl.uphjek.com

TS:   // 手写回溯递归
来源：http://jik.dashuyun.cn

Java: // 手写回溯递归
来源：http://bpi.nanxinkj.top

Go:   // 手写回溯递归
来源：http://gyp.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://dwr.zdqjudy.top

C#:   // 手写回溯递归
来源：http://onk.jqgufenzy.top

[N09] 栈与队列
来源：http://dwa.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mea.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iyn.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hvm.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ihr.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wuu.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wmi.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dto.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jxv.tian-w.cn

[N10] 链表节点定义
来源：http://tit.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vqj.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qvp.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kem.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pkk.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://ksc.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iyr.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yze.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pxp.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://iav.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kxs.sysykeji.top

PHP:  // 手写递归函数
来源：http://rcy.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzk.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wto.zhixingplan.top

Java: // 手写递归
来源：http://szz.9152youxi.cn

Go:   // 手写递归
来源：http://tye.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://isg.xinyue.icu

C#:   // 手写递归
来源：http://wke.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://onc.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://erq.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cyf.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mvf.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ncr.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bon.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wdz.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rgw.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cxn.xinyue.icu

================================================================================
来源：http://gry.ivvv.top

O. 并发与异步
来源：http://drf.shanyushiyangtech.top

================================================================================
来源：http://sdw.gaohongyu789.top

[O01] 启动一个线程
来源：http://hyp.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vho.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xsj.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cer.andypj.xyz

TS:   // 同 JS
来源：http://qne.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://stq.yvedp.cn

Go:   go f()
来源：http://yfw.tian-w.cn

Ruby: Thread.new { f }
来源：http://gvl.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://eyl.sysykeji.top

[O02] 使用线程池
来源：http://sec.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sbw.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://syh.sxryk.cn

JS:   // worker_threads 线程池
来源：http://vtg.vehdjk.com

TS:   // worker_threads 线程池
来源：http://qlf.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uur.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zsr.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mnk.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ryo.xziqi.cn

[O03] 加锁保护共享数据
来源：http://xct.tarul.cn

Py:   with lock: shared += 1
来源：http://slr.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://gsl.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ydr.meibo888.top

TS:   // 同 JS
来源：http://jzk.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://jwl.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gyg.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fuu.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://nlv.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://lbr.ivvv.top

Py:   async def f():⏎    await g()
来源：http://pxa.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ytx.tanke756.top

JS:   async function f() { await g(); }
来源：http://kyp.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wor.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kpb.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zwx.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kon.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://xqr.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://ryf.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://mev.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nkv.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://ekj.yonumen.top

TS:   await Promise.all(tasks)
来源：http://zzk.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nif.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://moi.meibo888.top

Ruby: threads.map(&:join)
来源：http://ade.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bpm.zhoulong.xyz

[O06] 使用进程池
来源：http://ahf.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ues.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nmk.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://wvu.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://kmu.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hkq.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tzv.chenlongwang.top

Ruby: // fork 块
来源：http://njr.zhiwuduotai.top

C#:   Parallel.For
来源：http://woi.zhixingplan.top

================================================================================
来源：http://xfd.zdbjq.cn

P. 常用工具函数
来源：http://rjr.daxiang520.top

================================================================================
来源：http://uwi.pycfn.com

[P01] 生成 UUID
来源：http://crw.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://bjg.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jbv.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://xvs.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://jrg.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://oro.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://buj.316326.xyz

Ruby: SecureRandom.uuid
来源：http://hdj.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://iox.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://ixm.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oqf.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://myf.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qoh.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hxh.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zdc.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jip.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xuf.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kee.daxiang520.top

[P03] 生成短随机字符串
来源：http://hey.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jpy.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dat.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypr.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tyi.hammf.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gkz.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zrc.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wxr.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gkk.bjfxy.top

[P04] 求长度
来源：http://orw.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gld.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzh.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ksd.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yht.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://hjj.c1oappe.top

Go:   len(arr);  len(m)
来源：http://qqq.mhx1999.top

Ruby: x.length;  x.size
来源：http://dxv.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbe.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://ifr.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://zyr.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://azq.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://clm.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://joj.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://epv.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://yqr.cucudq.cn

Ruby: a == b
来源：http://hju.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://poj.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yxp.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://stf.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://ifn.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://abb.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://zey.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aug.yj20258.top

Go:   if x == nil {}
来源：http://jjt.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://evp.guannengcc.top

C#:   if (x is null) {}
来源：http://svw.shuidangran.top

[P07] 防抖与节流
来源：http://aaa.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gey.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://fyq.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcn.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfd.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dbj.svipenyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mlu.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hzq.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ede.tanke756.top

[P08] 处理浮点精度问题
来源：http://vhy.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mum.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lao.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rha.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rmw.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bol.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ptk.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hdg.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pot.birdmap.top

================================================================================
来源：http://ant.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zwy.iojbl.cn

================================================================================
来源：http://xvn.tian-w.cn

[Q01] 创建表
来源：http://drm.tarul.cn

CREATE TABLE users (
来源：http://zgs.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ltq.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://wdz.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://acp.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fdc.fanxiaobao.xyz

);
来源：http://czi.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://wuv.ydjk.org.cn

CREATE TABLE orders (
来源：http://exs.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkx.hywenlv.cn

user_id INT NOT NULL,
来源：http://keb.ivvv.top

amount DECIMAL(10, 2),
来源：http://dyz.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mdk.haohaochexian.top

);
来源：http://cwn.wangdashe.top

[Q03] 增加列
来源：http://luj.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zvx.yfazqb.com

[Q04] 修改列类型
来源：http://uqg.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://izc.zdqjudy.top

[Q05] 重命名列
来源：http://ays.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oqo.zhongyouzk.top

[Q06] 删除列
来源：http://tzd.yvedp.cn


<!-- 参考信息 -->