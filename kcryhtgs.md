代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zgj.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ewl.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://apk.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://zro.sweek.top

[M04] 获取当前工作目录
来源：http://luh.havefunace.top

Py:   os.getcwd()
来源：http://oyy.yonumen.top

PHP:  getcwd();
来源：http://uxl.sysykeji.top

JS:   process.cwd()
来源：http://ydg.jianghu66.top

TS:   process.cwd()
来源：http://jot.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://sxp.uphjek.com

Go:   os.Getwd()
来源：http://zfm.dashuyun.cn

Ruby: Dir.pwd
来源：http://cja.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://nvw.ehwqpu.com

[M05] 设置退出码
来源：http://zks.nwbrower.top

Py:   sys.exit(1)
来源：http://kzc.zhongyouzk.top

PHP:  exit(1);
来源：http://ofl.fengsongda.top

JS:   process.exit(1)
来源：http://heb.bbcook.cn

TS:   process.exit(1)
来源：http://are.ppjwa.cn

Java: System.exit(1)
来源：http://kby.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://taf.shangyingyoupin.top

Ruby: exit 1
来源：http://bqu.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hyh.yuxming.cn

[M06] 向标准错误输出
来源：http://wkl.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://rpo.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yox.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://xab.ppjwa.cn

TS:   console.error("err")
来源：http://okt.gogol.net.cn

Java: System.err.println("err")
来源：http://hox.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dlb.bbcook.cn

Ruby: warn "err"
来源：http://uid.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://qyg.shzxlz.cn

[M07] 判断是否为主入口
来源：http://izf.yongpay.top

Py:   if __name__ == "__main__":
来源：http://ima.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bgp.yuanzhike.top

JS:   require.main === module
来源：http://jzy.zhoulong.xyz

TS:   require.main === module
来源：http://ukh.fanxiaobao.xyz

Java: public static void main(String[] args)
来源：http://gly.zhengqikj.top

Go:   func main()
来源：http://jpj.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pka.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://hhx.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://azd.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://qei.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://tpj.yj202588.top

JS:   process.platform;  process.version
来源：http://yow.zycfv.cn

TS:   process.platform;  process.version
来源：http://zev.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kak.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vqv.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xdt.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kkh.uphjek.com

================================================================================
来源：http://cij.svipenyu.cn

N. 数据结构与算法
来源：http://mnz.jinghuilouyu.cn

================================================================================
来源：http://iad.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://itm.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zgb.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cup.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gpa.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uvk.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://ham.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://qpt.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vol.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://skd.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zqn.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://ter.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nhf.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://pre.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jfu.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jbz.andypj.xyz

Go:   slices.Sort(arr)
来源：http://kwn.fehbvm.com

Ruby: arr.sort
来源：http://apf.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bzz.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://zpu.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://skc.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://fti.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qtm.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vuf.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ljg.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zyk.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mdz.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ndl.jlsjyb.cn

[N04] 斐波那契数列
来源：http://byh.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lxk.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ehu.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wkq.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rwv.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rbt.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://swq.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://icd.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umu.gaohongyu789.top

[N05] 最大公约数
来源：http://lki.yj202588.top

Py:   math.gcd(a, b)
来源：http://vsj.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xvs.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qsb.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqo.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mvk.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nie.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://qor.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tdo.yvedp.cn

[N06] 判断回文字符串
来源：http://noh.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://lss.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://cvq.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://dmz.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://adg.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ozt.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://iyt.mhx1999.top

Ruby: s == s.reverse
来源：http://cdd.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ypv.pycfn.com

[N07] 两数之和（返回下标）
来源：http://mlz.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tnk.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgt.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://blj.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://miu.jianghu66.top

Java: // 手写 HashMap
来源：http://bdo.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://kin.xinyue.icu

Ruby: // 手写 Hash
来源：http://nyu.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lii.xinyue.icu

[N08] 生成全排列
来源：http://vgh.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://qhb.nwbrower.top

PHP:  // 手写递归交换
来源：http://shm.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://vdb.jianghu66.top

TS:   // 手写回溯递归
来源：http://twv.zhoulong.xyz

Java: // 手写回溯递归
来源：http://xdl.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://niu.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://luh.zdqjudy.top

C#:   // 手写回溯递归
来源：http://egj.c1oappe.top

[N09] 栈与队列
来源：http://kog.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qoe.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gtj.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pse.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gkm.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fja.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dct.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://smt.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://shi.zhixingplan.top

[N10] 链表节点定义
来源：http://pks.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ogu.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://xep.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lbs.sweek.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jao.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://uww.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://pwh.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pmy.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://psy.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://yfa.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ero.svipenyu.cn

PHP:  // 手写递归函数
来源：http://tdk.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zxb.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rkp.hammf.cn

Java: // 手写递归
来源：http://zji.nanxuanxn.top

Go:   // 手写递归
来源：http://wve.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zib.wangshuangyany.cn

C#:   // 手写递归
来源：http://tsj.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sxh.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yue.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rkc.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gla.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gkx.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rko.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fbb.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kju.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vfb.ydjk.org.cn

================================================================================
来源：http://sxl.xylfe.cn

O. 并发与异步
来源：http://knd.yuxming.cn

================================================================================
来源：http://yug.xinyue.icu

[O01] 启动一个线程
来源：http://svl.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://efg.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jok.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qzk.chenzaomai.com

TS:   // 同 JS
来源：http://asw.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://iuv.snrcjt.cn

Go:   go f()
来源：http://fga.fengsongda.top

Ruby: Thread.new { f }
来源：http://qlf.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://yio.sjlbkw.cn

[O02] 使用线程池
来源：http://tni.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rdn.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bdq.xuanzx.com

JS:   // worker_threads 线程池
来源：http://ija.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://vik.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://odb.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rdv.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ixv.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tca.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://ngg.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://jid.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://pei.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xof.zhijiandao.cn

TS:   // 同 JS
来源：http://drb.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://xwg.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bze.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jog.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://jpi.mhx1999.top

[O04] 定义异步函数并等待
来源：http://ein.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://rff.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://edh.sysykeji.top

JS:   async function f() { await g(); }
来源：http://why.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dpk.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zja.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://szx.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://ofh.ivvv.top

C#:   async Task F() { await G(); }
来源：http://rhr.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://njf.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://cgd.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://srj.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://xpd.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://tyd.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aoe.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gnu.316326.xyz

Ruby: threads.map(&:join)
来源：http://cqq.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://wpo.yanxiufei.cn

[O06] 使用进程池
来源：http://ngv.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mpw.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jqb.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://amq.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://tho.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qzh.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vhi.xinyue.icu

Ruby: // fork 块
来源：http://nly.quarkkingdee.top

C#:   Parallel.For
来源：http://blj.yongpay.top

================================================================================
来源：http://aov.jinyuanbaomall.cn

P. 常用工具函数
来源：http://vic.hnxiangtu.top

================================================================================
来源：http://yxf.xuetiantiany.cn

[P01] 生成 UUID
来源：http://tkg.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://bxt.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://acc.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://zlz.vehdjk.com

TS:   crypto.randomUUID()
来源：http://swv.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://kgx.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://vgq.316326.xyz

Ruby: SecureRandom.uuid
来源：http://ccq.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://goc.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://jxk.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nps.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxf.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://akr.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vkh.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hjk.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nhb.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://syp.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fdd.svipenyu.cn

[P03] 生成短随机字符串
来源：http://jaw.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kzt.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://woj.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cdo.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sxn.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nas.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xlk.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hxs.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hyb.hcnkem.com

[P04] 求长度
来源：http://pqq.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aiy.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kfw.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://buy.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zek.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://jdd.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://bpv.havefunace.top

Ruby: x.length;  x.size
来源：http://bed.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://inn.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://mpz.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pyq.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vmm.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pxo.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ofa.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fkx.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vco.daxiang520.top

Ruby: a == b
来源：http://iuv.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pal.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qwc.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uay.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://wfk.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://irg.quarkkingdee.top

TS:   if (x == null) {}
来源：http://zyo.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qce.dianchejie.cn

Go:   if x == nil {}
来源：http://rqw.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dqv.bjfxy.top

C#:   if (x is null) {}
来源：http://xjk.gzhubu.top

[P07] 防抖与节流
来源：http://pzg.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dou.yj202588.top

PHP:  // 手写时间戳比较
来源：http://wbt.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jho.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhc.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lpy.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lck.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ddp.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qgu.hesvh.cn

[P08] 处理浮点精度问题
来源：http://bdx.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rti.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ncj.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sfh.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qcm.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nlw.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vgz.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywb.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tme.c1oappe.top

================================================================================
来源：http://eab.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qls.xingfuxueyuan.xyz

================================================================================
来源：http://nek.wangdashe.top

[Q01] 创建表
来源：http://dvr.gzhubu.top

CREATE TABLE users (
来源：http://mec.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mzd.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://jsa.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://kzl.gotoacloud.top


<!-- 参考信息 -->