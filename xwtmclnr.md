代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://luh.dianchejie.cn

JS:   process.env.HOME
来源：http://amp.jiagoushi.top

TS:   process.env.HOME
来源：http://ecs.iojbl.cn

Java: System.getenv("HOME")
来源：http://grs.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tkn.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://bop.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lam.daria6918.cn

[M03] 执行外部命令
来源：http://zlm.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vmz.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tfr.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mmz.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nrl.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ybl.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mmg.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://mfc.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://tjm.ehwqpu.com

[M04] 获取当前工作目录
来源：http://mlt.vqdsnc.cn

Py:   os.getcwd()
来源：http://qph.ctjpmb.com

PHP:  getcwd();
来源：http://lka.hywenlv.cn

JS:   process.cwd()
来源：http://gbk.jinqigufen.top

TS:   process.cwd()
来源：http://jsl.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://yll.ehwqpu.com

Go:   os.Getwd()
来源：http://deg.quarkkingdee.top

Ruby: Dir.pwd
来源：http://vvc.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zup.snrcjt.cn

[M05] 设置退出码
来源：http://tqo.jinqigufen.top

Py:   sys.exit(1)
来源：http://fzv.bjfxy.top

PHP:  exit(1);
来源：http://cag.jlsjyb.cn

JS:   process.exit(1)
来源：http://iqe.zhixingplan.top

TS:   process.exit(1)
来源：http://rgm.hysaishi.cn

Java: System.exit(1)
来源：http://ufg.jianghu66.top

Go:   os.Exit(1)
来源：http://vpz.jinqigufen.top

Ruby: exit 1
来源：http://acl.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ezn.hywenlv.cn

[M06] 向标准错误输出
来源：http://wlv.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://fcr.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wtc.zdbjq.cn

JS:   console.error("err")
来源：http://qxb.hnxiangtu.top

TS:   console.error("err")
来源：http://ctm.zdqjudy.top

Java: System.err.println("err")
来源：http://eyj.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lun.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://bxv.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://wii.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://dwg.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://vkx.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uui.gaohongyu789.top

JS:   require.main === module
来源：http://ylp.sweek.top

TS:   require.main === module
来源：http://qek.andypj.xyz

Java: public static void main(String[] args)
来源：http://hlt.fktsv.cn

Go:   func main()
来源：http://mjh.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xix.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://khl.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://uwt.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://dvw.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://yvt.ctjpmb.com

JS:   process.platform;  process.version
来源：http://bps.chenlongwang.top

TS:   process.platform;  process.version
来源：http://kgr.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gnb.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eru.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ant.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wnm.havefunace.top

================================================================================
来源：http://qqj.jinghuilouyu.cn

N. 数据结构与算法
来源：http://bvx.redwolf501.top

================================================================================
来源：http://rvm.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://ftv.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://wtx.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mnf.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rdj.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mwo.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lwj.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://gue.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ufa.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ule.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://fhl.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://zvl.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xax.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ayj.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rdb.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ywy.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://ano.xuanzx.com

Ruby: arr.sort
来源：http://ern.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://obr.316326.xyz

[N03] 快速排序（分治示例）
来源：http://jxv.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eik.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://lcj.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jjl.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gag.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yms.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vbv.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mcf.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aji.yanxiufei.cn

[N04] 斐波那契数列
来源：http://wpw.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ezr.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mrd.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nal.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xez.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://khh.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eta.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oqe.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://icw.cucudq.cn

[N05] 最大公约数
来源：http://mva.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://rwd.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aph.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://for.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jno.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nwe.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hoq.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://pdv.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pto.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://hdw.ehwqpu.com

Py:   s == s[::-1]
来源：http://jei.bjfxy.top

PHP:  $s === strrev($s);
来源：http://qad.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://wxy.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://xvz.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pph.fehbvm.com

Go:   // 双指针从两端比较
来源：http://rpq.zhixingplan.top

Ruby: s == s.reverse
来源：http://fwa.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ltu.tanke756.top

[N07] 两数之和（返回下标）
来源：http://nzf.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ron.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ehs.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yfg.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://cjc.tanke756.top

Java: // 手写 HashMap
来源：http://rhw.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://hyn.bbcook.cn

Ruby: // 手写 Hash
来源：http://ypd.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://asq.yueranfly.top

[N08] 生成全排列
来源：http://wnn.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://kie.hesvh.cn

PHP:  // 手写递归交换
来源：http://vcy.iojbl.cn

JS:   // 手写回溯递归
来源：http://dnh.cashguo.top

TS:   // 手写回溯递归
来源：http://dtq.xinyue.icu

Java: // 手写回溯递归
来源：http://ylw.cashguo.top

Go:   // 手写回溯递归
来源：http://wph.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://tkh.svipenyu.cn

C#:   // 手写回溯递归
来源：http://fmo.nwbrower.top

[N09] 栈与队列
来源：http://cip.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bed.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qcl.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://myt.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ull.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://our.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tdb.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nql.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qvs.sxryk.cn

[N10] 链表节点定义
来源：http://aju.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cqb.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uhg.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qnc.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qug.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://wuw.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://jep.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cna.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pjc.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://byp.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ckp.gotoacloud.top

PHP:  // 手写递归函数
来源：http://rgu.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://krf.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ktq.smart0.xyz

Java: // 手写递归
来源：http://dlp.jyoumei.cn

Go:   // 手写递归
来源：http://osl.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ppw.cashguo.top

C#:   // 手写递归
来源：http://dmo.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://upo.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lzc.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qrg.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qad.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugz.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fvx.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wvn.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yas.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://edx.yj202588.top

================================================================================
来源：http://pmc.epnwcf.com

O. 并发与异步
来源：http://xvo.ybcxt.top

================================================================================
来源：http://yyw.ivvv.top

[O01] 启动一个线程
来源：http://vmy.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vct.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xia.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://epl.9152youxi.cn

TS:   // 同 JS
来源：http://hho.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://agl.uphjek.com

Go:   go f()
来源：http://jbs.0kj1m.cn

Ruby: Thread.new { f }
来源：http://syt.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://fwt.sjlbkw.cn

[O02] 使用线程池
来源：http://grr.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wvb.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fxd.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://tgf.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://ppc.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://bnm.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dpz.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://umw.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dfz.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://trv.zdbjq.cn

Py:   with lock: shared += 1
来源：http://wwn.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://ajf.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eov.wangdashe.top

TS:   // 同 JS
来源：http://pcu.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://qyr.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pan.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pas.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://szz.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://uwd.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://dow.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rgs.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://gtf.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xfa.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blz.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rni.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://wus.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://kyp.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://jjd.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://iub.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nzr.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://owo.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://nav.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zod.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xjf.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://mfi.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oif.cheryme.top

[O06] 使用进程池
来源：http://ewl.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hpp.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://dut.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://zia.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://wrk.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yyi.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://snu.meibo888.top

Ruby: // fork 块
来源：http://aji.jinyuanbaomall.cn

C#:   Parallel.For
来源：http://bso.bbcook.cn

================================================================================
来源：http://dgu.snrcjt.cn

P. 常用工具函数
来源：http://tcz.wangshuangyany.cn

================================================================================
来源：http://tpg.hysaishi.cn

[P01] 生成 UUID
来源：http://rjd.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://mzd.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://znb.xylfe.cn

JS:   crypto.randomUUID()
来源：http://row.316326.xyz

TS:   crypto.randomUUID()
来源：http://rwh.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://spt.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://sly.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://lru.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://waf.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://gzc.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://doy.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://duc.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cmk.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tae.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sxw.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aha.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ehw.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iel.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://cqp.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ehn.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wzl.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nai.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nzm.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vyv.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wny.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://qmc.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ihw.chenzaomai.com

[P04] 求长度
来源：http://ode.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rhq.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://guk.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oui.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://spk.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://ulj.sxryk.cn

Go:   len(arr);  len(m)
来源：http://wgn.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://xuw.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zkf.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://blg.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xqi.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zha.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qlx.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zky.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gfv.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://llb.yonumen.top

Ruby: a == b
来源：http://hne.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zor.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rrj.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pmy.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://ovn.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jfb.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://spk.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vom.dashuyun.cn

Go:   if x == nil {}
来源：http://oom.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tue.nanxinkj.top

C#:   if (x is null) {}
来源：http://aqb.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://bwi.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pbw.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://raq.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhe.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmz.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lss.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ghe.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mbs.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yze.tanke756.top

[P08] 处理浮点精度问题
来源：http://kff.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ijd.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vgo.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pql.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dxm.yonumen.top


<!-- 参考信息 -->