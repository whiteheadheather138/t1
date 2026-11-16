代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wpz.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lxs.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://kdr.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://oju.yfazqb.com

[M04] 获取当前工作目录
来源：http://jcb.gotoacloud.top

Py:   os.getcwd()
来源：http://utd.ydzc1.top

PHP:  getcwd();
来源：http://ojy.feifeiyinyue.top

JS:   process.cwd()
来源：http://rig.chenjidiqi.icu

TS:   process.cwd()
来源：http://uuk.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://ymq.guowangkeji.top

Go:   os.Getwd()
来源：http://nve.hnqzz.top

Ruby: Dir.pwd
来源：http://cfm.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pzj.cashguo.top

[M05] 设置退出码
来源：http://ozx.yanxiufei.cn

Py:   sys.exit(1)
来源：http://hro.mhx1999.top

PHP:  exit(1);
来源：http://aor.gotoacloud.top

JS:   process.exit(1)
来源：http://oxl.hfpthk.cn

TS:   process.exit(1)
来源：http://rzv.yongpay.top

Java: System.exit(1)
来源：http://rzn.mhx1999.top

Go:   os.Exit(1)
来源：http://yei.sysykeji.top

Ruby: exit 1
来源：http://exq.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uxi.zdqjudy.top

[M06] 向标准错误输出
来源：http://dbc.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://xck.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://apg.quarkkingdee.top

JS:   console.error("err")
来源：http://irl.xuetiantiany.cn

TS:   console.error("err")
来源：http://gkp.sufxvd.cn

Java: System.err.println("err")
来源：http://gkd.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qms.hywenlv.cn

Ruby: warn "err"
来源：http://ypn.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://tqh.smart0.xyz

[M07] 判断是否为主入口
来源：http://qxs.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://alf.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ctb.shangyingyoupin.top

JS:   require.main === module
来源：http://bkk.daxiang520.top

TS:   require.main === module
来源：http://xsy.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://qqa.yuanzhike.top

Go:   func main()
来源：http://cvp.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rta.daxiang520.top

C#:   static void Main(string[] args)
来源：http://acl.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://yja.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://zfs.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://bub.meibo888.top

JS:   process.platform;  process.version
来源：http://khp.daria6918.cn

TS:   process.platform;  process.version
来源：http://lvj.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xzf.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fwl.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mvl.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmf.ehwqpu.com

================================================================================
来源：http://jcz.sweek.top

N. 数据结构与算法
来源：http://xem.fengsongda.top

================================================================================
来源：http://gjw.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://cdy.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://fjh.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mjp.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xtw.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zpf.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dkn.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://byk.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qrw.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://bqi.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://vzc.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://xns.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vgz.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://wku.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vjx.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eaf.yj20258888.top

Go:   slices.Sort(arr)
来源：http://xru.ivvv.top

Ruby: arr.sort
来源：http://dcu.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://jql.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://fxe.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nyt.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://qbj.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqy.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uba.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blu.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pdw.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://orp.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zrw.xinyue.icu

[N04] 斐波那契数列
来源：http://roo.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dlb.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://prx.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tla.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://epg.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://orh.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vvu.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cvr.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lle.yueranfly.top

[N05] 最大公约数
来源：http://xzx.c1oappe.top

Py:   math.gcd(a, b)
来源：http://bxv.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vro.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lne.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://one.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jnq.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jjl.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://jua.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pbn.pycfn.com

[N06] 判断回文字符串
来源：http://bey.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://vzr.birdmap.top

PHP:  $s === strrev($s);
来源：http://uyl.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://shw.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://nvx.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gds.pycfn.com

Go:   // 双指针从两端比较
来源：http://hft.meibo888.top

Ruby: s == s.reverse
来源：http://opp.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rul.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://nzj.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://shz.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kbo.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mnq.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://png.ydjk.org.cn

Java: // 手写 HashMap
来源：http://qzy.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://uvs.mhx1999.top

Ruby: // 手写 Hash
来源：http://tjr.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://gvu.quarkkingdee.top

[N08] 生成全排列
来源：http://ump.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://tgb.cashguo.top

PHP:  // 手写递归交换
来源：http://qii.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://cxq.yj202588.top

TS:   // 手写回溯递归
来源：http://nlz.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://sjs.hnqzz.top

Go:   // 手写回溯递归
来源：http://wwa.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://kfa.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://rgt.zdbjq.cn

[N09] 栈与队列
来源：http://iov.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://odt.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lln.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nst.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dwi.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pyt.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fbz.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cqq.jinqigufen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aja.vqdsnc.cn

[N10] 链表节点定义
来源：http://igc.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kqk.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hwh.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oqr.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pfz.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://toj.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ohu.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lru.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bmt.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://acd.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dfs.c1oappe.top

PHP:  // 手写递归函数
来源：http://jmh.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hfp.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ris.0kj1m.cn

Java: // 手写递归
来源：http://qiw.bjfxy.top

Go:   // 手写递归
来源：http://uuu.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://omc.bbcook.cn

C#:   // 手写递归
来源：http://nsc.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gmw.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kfj.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ode.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rim.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tav.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sdx.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lbz.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://veh.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://viq.jinghuilouyu.cn

================================================================================
来源：http://sjh.dashuyun.cn

O. 并发与异步
来源：http://qyn.chenjidiqi.icu

================================================================================
来源：http://fpg.gogol.net.cn

[O01] 启动一个线程
来源：http://nkp.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mvn.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rxe.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qnu.fengsongda.top

TS:   // 同 JS
来源：http://yvu.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://szs.jinghuilouyu.cn

Go:   go f()
来源：http://ouy.bjfxy.top

Ruby: Thread.new { f }
来源：http://gth.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://wwo.hammf.cn

[O02] 使用线程池
来源：http://gpu.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jmm.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qbp.sxryk.cn

JS:   // worker_threads 线程池
来源：http://fug.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://vjx.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://aim.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fln.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jlb.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qtr.andypj.xyz

[O03] 加锁保护共享数据
来源：http://rxw.xuanzx.com

Py:   with lock: shared += 1
来源：http://rgu.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://lxa.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bwg.316326.xyz

TS:   // 同 JS
来源：http://zqh.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://vmd.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fuv.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ava.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://oqk.yfazqb.com

[O04] 定义异步函数并等待
来源：http://cmg.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://exb.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ndq.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://ulo.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tqb.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qat.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://who.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://vyw.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://fkf.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://xfv.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://hlt.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rgd.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://nqb.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://mnu.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://koy.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sna.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://qlr.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xae.fanxiaobao.xyz

[O06] 使用进程池
来源：http://adl.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ifz.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://bcx.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://qyb.tarul.cn

TS:   // child_process / cluster 模块
来源：http://uhh.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://usb.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yot.zycfv.cn

Ruby: // fork 块
来源：http://rra.dianchejie.cn

C#:   Parallel.For
来源：http://lel.jinqigufen.top

================================================================================
来源：http://fwc.hfpthk.cn

P. 常用工具函数
来源：http://xcr.hcnkem.com

================================================================================
来源：http://imb.jqgufenzy.top

[P01] 生成 UUID
来源：http://huk.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://vbv.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yvr.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://wov.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://zdk.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://wem.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://xij.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://zxr.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://nck.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://zxy.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://czh.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fpu.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ttw.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vcy.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fqv.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://imc.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wox.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xtg.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://sxz.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tau.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rtx.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wpr.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qoh.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ccv.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iiv.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://sti.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zoj.yangfankeji.com

[P04] 求长度
来源：http://vzi.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jvm.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lpz.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nrq.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zgh.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://iim.birdmap.top

Go:   len(arr);  len(m)
来源：http://vus.ctjpmb.com

Ruby: x.length;  x.size
来源：http://stq.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ymx.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://eyf.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yba.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jhl.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lqx.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eyk.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ydv.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tzq.guowangkeji.top

Ruby: a == b
来源：http://whv.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ldy.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rsr.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wbz.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://gbt.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ynt.guowangkeji.top

TS:   if (x == null) {}
来源：http://icb.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://olo.cdnleiting.top

Go:   if x == nil {}
来源：http://zrn.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mrk.zycfv.cn

C#:   if (x is null) {}
来源：http://ykm.hcnkem.com

[P07] 防抖与节流
来源：http://owv.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fzg.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://osd.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxv.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixv.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qjt.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ner.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://mpr.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kjb.cashguo.top

[P08] 处理浮点精度问题
来源：http://dot.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pxa.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pmd.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://koc.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hsm.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yqm.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://znq.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kdr.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ows.shangyingyoupin.top

================================================================================
来源：http://lri.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://idr.tianlin.xyz

================================================================================
来源：http://axv.feifeiyinyue.top

[Q01] 创建表
来源：http://etc.cucudq.cn

CREATE TABLE users (
来源：http://vnl.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qiz.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://pbx.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://bha.cashguo.top


<!-- 参考信息 -->