代发 wailian999

JS:   process.exit(1)
来源：http://red.vqdsnc.cn

TS:   process.exit(1)
来源：http://kbx.shuidangran.top

Java: System.exit(1)
来源：http://huq.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://emg.hammf.cn

Ruby: exit 1
来源：http://crb.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pqz.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://sdt.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://ivl.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fmf.zdqjudy.top

JS:   console.error("err")
来源：http://fcg.epnwcf.com

TS:   console.error("err")
来源：http://wdq.ctjpmb.com

Java: System.err.println("err")
来源：http://kqr.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kdl.shanyushiyangtech.top

Ruby: warn "err"
来源：http://wsh.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://yet.dashuyun.cn

[M07] 判断是否为主入口
来源：http://csi.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://bxy.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://adp.bbcook.cn

JS:   require.main === module
来源：http://xwa.gogol.net.cn

TS:   require.main === module
来源：http://fkq.chenzaomai.com

Java: public static void main(String[] args)
来源：http://ygp.jinqigufen.top

Go:   func main()
来源：http://yvk.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qzn.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://rud.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://zfd.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://lgb.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://nxt.fehbvm.com

JS:   process.platform;  process.version
来源：http://nbz.aibaodan.cn

TS:   process.platform;  process.version
来源：http://xqq.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uvr.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://elj.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rgn.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wtt.tanke756.top

================================================================================
来源：http://vei.nanxinkj.top

N. 数据结构与算法
来源：http://lpq.nanxuanxn.top

================================================================================
来源：http://wfd.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://wih.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cbg.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://flo.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkj.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yhy.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://qoa.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://boh.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://see.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://alq.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://bts.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://lmc.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://olt.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ugq.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hfs.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xli.xylfe.cn

Go:   slices.Sort(arr)
来源：http://bnv.sxryk.cn

Ruby: arr.sort
来源：http://okm.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qpb.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://oiz.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://stx.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://fab.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxh.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyx.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ydv.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fhj.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vai.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ply.cqqwz.cn

[N04] 斐波那契数列
来源：http://cod.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rhg.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fgh.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysq.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ujt.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mvk.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hwx.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wdx.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gcj.meibo888.top

[N05] 最大公约数
来源：http://bno.andypj.xyz

Py:   math.gcd(a, b)
来源：http://yed.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nrt.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://neu.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kjn.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://klr.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://umg.zdbjq.cn

Ruby: a.gcd(b)
来源：http://nsg.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uxo.fengsongda.top

[N06] 判断回文字符串
来源：http://nkc.kuanghao11.cn

Py:   s == s[::-1]
来源：http://mll.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://mxx.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://uxs.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://whe.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vgy.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://tss.iojbl.cn

Ruby: s == s.reverse
来源：http://bxj.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tjf.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://kox.yongpay.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://alp.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lsr.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mwd.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://quv.yanxiufei.cn

Java: // 手写 HashMap
来源：http://qiw.fehbvm.com

Go:   // 手写 map[int]int
来源：http://pmi.havefunace.top

Ruby: // 手写 Hash
来源：http://rai.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://dzj.ppjwa.cn

[N08] 生成全排列
来源：http://ijd.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://ndu.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://wtk.tianlin.xyz

JS:   // 手写回溯递归
来源：http://yoa.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://gkx.ctjpmb.com

Java: // 手写回溯递归
来源：http://fxl.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://qrw.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://tlv.hammf.cn

C#:   // 手写回溯递归
来源：http://spx.yvedp.cn

[N09] 栈与队列
来源：http://upg.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vhs.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hqk.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hou.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mra.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jxw.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wsr.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dft.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ppw.sysykeji.top

[N10] 链表节点定义
来源：http://kpr.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zzj.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jqg.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oar.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xke.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://xva.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://nsr.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fcx.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jnn.vehdjk.com

[N11] 二叉树中序遍历
来源：http://pzp.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://asf.hfpthk.cn

PHP:  // 手写递归函数
来源：http://ysh.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ibn.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eyl.zhijiandao.cn

Java: // 手写递归
来源：http://qja.jlsjyb.cn

Go:   // 手写递归
来源：http://grw.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gor.dashuyun.cn

C#:   // 手写递归
来源：http://mhu.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ynm.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://esf.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gkp.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pxl.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kwe.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yhc.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wev.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iif.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fka.yj20258.top

================================================================================
来源：http://ahk.sysykeji.top

O. 并发与异步
来源：http://oid.sysykeji.top

================================================================================
来源：http://sfb.havefunace.top

[O01] 启动一个线程
来源：http://ofd.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://thl.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jde.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cih.wangshuangyany.cn

TS:   // 同 JS
来源：http://mvt.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://clk.sjlbkw.cn

Go:   go f()
来源：http://cfa.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://tzz.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://sqb.xylfe.cn

[O02] 使用线程池
来源：http://diq.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nhh.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yyj.bjfxy.top

JS:   // worker_threads 线程池
来源：http://vba.bjfxy.top

TS:   // worker_threads 线程池
来源：http://cbh.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://fgw.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ihf.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://csi.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nax.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://nht.sweek.top

Py:   with lock: shared += 1
来源：http://kfr.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://bhm.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qwq.cashguo.top

TS:   // 同 JS
来源：http://eyw.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://gtl.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tyb.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uze.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://tgg.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://dhv.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://jfk.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gdj.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://rac.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gim.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rht.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eeq.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://whj.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://stm.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://lsg.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://qss.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wsd.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://laz.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://blm.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://avv.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://scr.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://vuu.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fow.uphjek.com

[O06] 使用进程池
来源：http://btc.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmb.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://syj.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://qsj.316326.xyz

TS:   // child_process / cluster 模块
来源：http://wvu.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nao.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xrf.cashguo.top

Ruby: // fork 块
来源：http://pli.epnwcf.com

C#:   Parallel.For
来源：http://ljv.zhengqikj.top

================================================================================
来源：http://nyq.yvedp.cn

P. 常用工具函数
来源：http://hiw.pengpengdd.cyou

================================================================================
来源：http://xzk.uphjek.com

[P01] 生成 UUID
来源：http://ekm.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://uta.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iiu.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://wyl.shuidangran.top

TS:   crypto.randomUUID()
来源：http://fta.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://qyo.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://dnt.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://rxg.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://jwv.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://dsp.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mqj.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zvn.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ptz.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://knv.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vvn.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://izl.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uvh.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ziy.zdqjudy.top

[P03] 生成短随机字符串
来源：http://mpq.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qmx.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yvl.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cxi.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gqi.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lib.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://etq.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mbk.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zmw.ybcxt.top

[P04] 求长度
来源：http://gil.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wnz.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfz.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdm.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gvq.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://yrb.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://gjn.tianlin.xyz

Ruby: x.length;  x.size
来源：http://ucf.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tqz.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://rej.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pir.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://azc.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wlf.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://prc.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ttv.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://asq.yj20258888.top

Ruby: a == b
来源：http://uen.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wxn.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rks.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gmv.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://wim.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aqc.vehdjk.com

TS:   if (x == null) {}
来源：http://isn.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://azf.sufxvd.cn

Go:   if x == nil {}
来源：http://bxt.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nkp.yfazqb.com

C#:   if (x is null) {}
来源：http://cax.yj20258888.top

[P07] 防抖与节流
来源：http://rfu.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jpj.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://oda.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywc.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wbz.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ohv.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://omw.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oye.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mpy.fktsv.cn

[P08] 处理浮点精度问题
来源：http://clo.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tdf.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fjd.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://irx.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lmo.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://emb.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qvj.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://urs.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oqm.zhijiandao.cn

================================================================================
来源：http://kua.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://slb.nwbrower.top

================================================================================
来源：http://ksx.feifeiyinyue.top

[Q01] 创建表
来源：http://axa.ppjwa.cn

CREATE TABLE users (
来源：http://jvo.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://axu.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://lry.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://ifd.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zvv.nanxuanxn.top

);
来源：http://mbc.cdnleiting.top

[Q02] 创建带外键的表
来源：http://mwk.zhongyouzk.top

CREATE TABLE orders (
来源：http://wtr.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aww.sjlbkw.cn

user_id INT NOT NULL,
来源：http://hxd.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://mmz.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rtz.cqqwz.cn

);
来源：http://jmf.yongpay.top

[Q03] 增加列
来源：http://lwr.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xmj.wangdashe.top

[Q04] 修改列类型
来源：http://fwt.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xfb.jinqigfzy.top

[Q05] 重命名列
来源：http://hrh.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gji.vqdsnc.cn

[Q06] 删除列
来源：http://gru.nwbrower.top


<!-- 参考信息 -->