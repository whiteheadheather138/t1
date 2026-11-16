代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://fwg.shanyushiyangtech.top

[M05] 设置退出码
来源：http://jvy.smart0.xyz

Py:   sys.exit(1)
来源：http://vbn.zdbjq.cn

PHP:  exit(1);
来源：http://psc.shangyingyoupin.top

JS:   process.exit(1)
来源：http://toh.fzhhl.top

TS:   process.exit(1)
来源：http://ktj.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://ryk.c1oappe.top

Go:   os.Exit(1)
来源：http://lpw.fehbvm.com

Ruby: exit 1
来源：http://kzn.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pyi.jinqigfzy.top

[M06] 向标准错误输出
来源：http://bmd.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://jam.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://gwv.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://gbi.jinqigfzy.top

TS:   console.error("err")
来源：http://ual.xziqi.cn

Java: System.err.println("err")
来源：http://heq.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zjx.shanyushiyangtech.top

Ruby: warn "err"
来源：http://yib.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://uio.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://nzs.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://dpn.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aie.pycfn.com

JS:   require.main === module
来源：http://qpl.shangyingyoupin.top

TS:   require.main === module
来源：http://pby.sysykeji.top

Java: public static void main(String[] args)
来源：http://afz.fktsv.cn

Go:   func main()
来源：http://pzk.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wnm.meibo888.top

C#:   static void Main(string[] args)
来源：http://wbd.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://olx.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://mry.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://skw.yj20258888.top

JS:   process.platform;  process.version
来源：http://big.aizwys.cn

TS:   process.platform;  process.version
来源：http://icc.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dmt.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nvs.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lmm.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jgd.daxiang520.top

================================================================================
来源：http://unj.ctjpmb.com

N. 数据结构与算法
来源：http://ipd.redwolf501.top

================================================================================
来源：http://mfo.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://ebf.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://uuo.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ilh.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mjl.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cft.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://zaw.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://zzk.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gun.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://boy.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://yak.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://rmp.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://art.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bgo.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ljy.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uaf.xylfe.cn

Go:   slices.Sort(arr)
来源：http://oeg.tarul.cn

Ruby: arr.sort
来源：http://hqq.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mwi.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://vag.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kea.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://xqi.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcs.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ooy.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eth.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wzw.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bit.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://fwx.ivvv.top

[N04] 斐波那契数列
来源：http://ebw.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wvc.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qpi.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shp.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfx.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yle.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xig.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://arf.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gfi.yuanzhike.top

[N05] 最大公约数
来源：http://pgt.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://yok.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wqd.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxr.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kpk.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xcy.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://haq.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://xmb.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fls.pycfn.com

[N06] 判断回文字符串
来源：http://sbh.nwbrower.top

Py:   s == s[::-1]
来源：http://htl.fengsongda.top

PHP:  $s === strrev($s);
来源：http://byj.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://qbl.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://ohv.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gwa.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://nwk.zycfv.cn

Ruby: s == s.reverse
来源：http://bkg.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kib.pycfn.com

[N07] 两数之和（返回下标）
来源：http://xit.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ino.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zsk.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fgn.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://vco.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://hbg.fengsongda.top

Go:   // 手写 map[int]int
来源：http://lxu.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://srr.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://jcs.hcnkem.com

[N08] 生成全排列
来源：http://ajn.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://dkl.hysaishi.cn

PHP:  // 手写递归交换
来源：http://pqz.316326.xyz

JS:   // 手写回溯递归
来源：http://ync.sufxvd.cn

TS:   // 手写回溯递归
来源：http://qdv.9152youxi.cn

Java: // 手写回溯递归
来源：http://uum.svipenyu.cn

Go:   // 手写回溯递归
来源：http://gjz.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://izj.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://nsf.ehwqpu.com

[N09] 栈与队列
来源：http://daz.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nam.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cso.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fvg.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kam.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mqo.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kpm.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://srj.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kio.zdqjudy.top

[N10] 链表节点定义
来源：http://xww.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xmj.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nec.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zos.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vhg.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://oex.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://ibp.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jts.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ypm.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://lcy.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tfe.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://ybx.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wba.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbn.hongshengwenyu.top

Java: // 手写递归
来源：http://udx.yvedp.cn

Go:   // 手写递归
来源：http://ick.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lca.guannengcc.top

C#:   // 手写递归
来源：http://lgt.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lai.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ilt.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yqf.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mrd.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fcm.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ypf.gaohongyu789.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ymt.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sks.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qrs.nanxuanxn.top

================================================================================
来源：http://tyv.mhx1999.top

O. 并发与异步
来源：http://zje.pengpengdd.cyou

================================================================================
来源：http://tbh.ydjk.org.cn

[O01] 启动一个线程
来源：http://bec.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cfo.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aie.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://btj.svipenyu.cn

TS:   // 同 JS
来源：http://lgy.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://bbv.wangshuangyany.cn

Go:   go f()
来源：http://lko.redwolf501.top

Ruby: Thread.new { f }
来源：http://qdd.zycfv.cn

C#:   Task.Run(() => F());
来源：http://fvy.chenlongwang.top

[O02] 使用线程池
来源：http://vlz.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wss.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jxt.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://ufl.xylfe.cn

TS:   // worker_threads 线程池
来源：http://bpu.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xny.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lho.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rmj.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rek.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://sih.shzxlz.cn

Py:   with lock: shared += 1
来源：http://toc.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://zaa.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jwb.9152youxi.cn

TS:   // 同 JS
来源：http://hni.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://onv.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cbn.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cly.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://lnj.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://pqd.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://ggp.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rmi.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://ynt.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sed.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kzf.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zza.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://mue.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://yov.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://suj.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://qak.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ltf.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://itb.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://jgb.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gqp.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nog.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://tul.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nca.meibo888.top

[O06] 使用进程池
来源：http://hnb.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zel.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gnl.yongpay.top

JS:   // child_process / cluster 模块
来源：http://pmz.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://fkl.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://avv.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kbm.gzhubu.top

Ruby: // fork 块
来源：http://cuy.52xcode.cn

C#:   Parallel.For
来源：http://voe.meibo888.top

================================================================================
来源：http://jih.sufxvd.cn

P. 常用工具函数
来源：http://pgw.zhoulong.xyz

================================================================================
来源：http://umj.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://elf.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://xlt.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qgw.uphjek.com

JS:   crypto.randomUUID()
来源：http://mgu.daxiang520.top

TS:   crypto.randomUUID()
来源：http://kjd.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://pvs.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://ltq.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://cwo.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://vxf.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://gpy.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pds.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qde.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bbo.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fai.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ppn.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://spn.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sfj.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jsg.sysykeji.top

[P03] 生成短随机字符串
来源：http://laj.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://clb.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wxq.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fiu.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zck.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cai.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gbr.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dnv.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tqm.c1oappe.top

[P04] 求长度
来源：http://zfb.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zen.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlq.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gui.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urn.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://mor.sweek.top

Go:   len(arr);  len(m)
来源：http://gas.hywenlv.cn

Ruby: x.length;  x.size
来源：http://gxi.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sry.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://bgg.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xyg.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rzn.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://owm.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xgf.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iiu.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dcv.xuetiantiany.cn

Ruby: a == b
来源：http://eyo.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tfs.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://loh.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tsk.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://whk.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://otu.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://epo.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bnm.ehwqpu.com

Go:   if x == nil {}
来源：http://jnm.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oxy.yuanzhike.top

C#:   if (x is null) {}
来源：http://luj.hesvh.cn

[P07] 防抖与节流
来源：http://tlk.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dvt.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://hhf.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ihs.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://elh.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mwq.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jfk.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hox.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rol.meibo888.top

[P08] 处理浮点精度问题
来源：http://bkm.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://acu.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ick.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eyy.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dvc.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zpr.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hxz.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fvo.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bhd.nwbrower.top

================================================================================
来源：http://osu.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mgq.fengsongda.top

================================================================================
来源：http://nmz.shangyingyoupin.top

[Q01] 创建表
来源：http://ljc.hfpthk.cn

CREATE TABLE users (
来源：http://ihs.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hfv.gzhubu.top

name VARCHAR(50) NOT NULL,
来源：http://bzu.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://ovx.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://slg.fehbvm.com

);
来源：http://usf.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://rta.ydzc1.top

CREATE TABLE orders (
来源：http://whh.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ict.zhengqikj.top

user_id INT NOT NULL,
来源：http://awx.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://gkr.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iuo.tian-w.cn

);
来源：http://ejt.c1oappe.top

[Q03] 增加列
来源：http://jmr.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rik.yj20258888.top

[Q04] 修改列类型
来源：http://wzy.316326.xyz


<!-- 参考信息 -->