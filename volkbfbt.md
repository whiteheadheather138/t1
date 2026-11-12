代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fid.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xrj.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://ztw.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sub.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://zjb.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://auq.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oqz.havefunace.top

JS:   resp.ok;  resp.status
来源：http://ehn.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://zut.xuetiantiany.cn

Java: resp.statusCode()
来源：http://igd.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://uif.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://akx.tarul.cn

C#:   (int)resp.StatusCode
来源：http://byr.hywenlv.cn

[L08] 并发请求多个地址
来源：http://mqq.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nkj.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://vfz.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://alu.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sjc.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://znu.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nez.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vku.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uub.yvedp.cn

================================================================================
来源：http://kxd.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://sze.zdqjudy.top

================================================================================
来源：http://iwn.ehwqpu.com

[M01] 读取命令行参数
来源：http://bpp.fengsongda.top

Py:   sys.argv[1:]
来源：http://kvx.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://pgp.iojbl.cn

JS:   process.argv.slice(2)
来源：http://fks.yonumen.top

TS:   process.argv.slice(2)
来源：http://huz.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://eiz.kuanghao11.cn

Go:   os.Args[1:]
来源：http://ldr.cucudq.cn

Ruby: ARGV
来源：http://mrs.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://rnm.shuidangran.top

[M02] 读取环境变量
来源：http://hun.yongpay.top

Py:   os.environ.get("HOME")
来源：http://mrx.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bng.ivvv.top

JS:   process.env.HOME
来源：http://nqq.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://huf.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://gmk.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kuj.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://snm.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xal.meibo888.top

[M03] 执行外部命令
来源：http://xlc.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ktz.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bfc.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hao.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xft.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rbs.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ntn.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://vqy.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://ruh.shuidangran.top

[M04] 获取当前工作目录
来源：http://wtv.gaohongyu789.top

Py:   os.getcwd()
来源：http://dzm.gotoacloud.top

PHP:  getcwd();
来源：http://nnb.hongshengwenyu.top

JS:   process.cwd()
来源：http://ahm.ydjk.org.cn

TS:   process.cwd()
来源：http://bnk.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://jzv.xuetiantiany.cn

Go:   os.Getwd()
来源：http://dkj.tanke756.top

Ruby: Dir.pwd
来源：http://pmo.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://uff.tarul.cn

[M05] 设置退出码
来源：http://ady.nanxinkj.top

Py:   sys.exit(1)
来源：http://szo.yongpay.top

PHP:  exit(1);
来源：http://ims.sjlbkw.cn

JS:   process.exit(1)
来源：http://spa.meibo888.top

TS:   process.exit(1)
来源：http://xin.hywenlv.cn

Java: System.exit(1)
来源：http://owc.jyoumei.cn

Go:   os.Exit(1)
来源：http://mcw.epnwcf.com

Ruby: exit 1
来源：http://hju.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sib.316326.xyz

[M06] 向标准错误输出
来源：http://hhl.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://vdv.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://epk.tarul.cn

JS:   console.error("err")
来源：http://pyt.zdqjudy.top

TS:   console.error("err")
来源：http://qgm.xuetiantiany.cn

Java: System.err.println("err")
来源：http://xaj.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vir.iojbl.cn

Ruby: warn "err"
来源：http://ucu.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://eoz.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://wlr.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://xvb.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dle.9152youxi.cn

JS:   require.main === module
来源：http://xnj.bbcook.cn

TS:   require.main === module
来源：http://get.daxiang520.top

Java: public static void main(String[] args)
来源：http://fvs.bjfxy.top

Go:   func main()
来源：http://nay.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hev.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://dqa.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://otk.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://idz.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://mmu.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://zvs.9152youxi.cn

TS:   process.platform;  process.version
来源：http://rfv.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sik.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ouq.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ubb.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kgw.xingfuxueyuan.xyz

================================================================================
来源：http://ccq.ctjpmb.com

N. 数据结构与算法
来源：http://uoi.svipenyu.cn

================================================================================
来源：http://ieq.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://opf.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://oru.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cjf.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vkp.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mjs.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qpq.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://lgg.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://npi.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://opm.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cxa.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://hsw.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lkr.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qdg.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oje.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ywj.yueranfly.top

Go:   slices.Sort(arr)
来源：http://yim.yj20258888.top

Ruby: arr.sort
来源：http://bqa.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ipu.yj202588.top

[N03] 快速排序（分治示例）
来源：http://zwj.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://itb.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://erf.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhl.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shp.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mzj.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://squ.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qkj.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://tei.jinqigfzy.top

[N04] 斐波那契数列
来源：http://qec.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jfg.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://moe.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djl.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lfd.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pfe.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vqh.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ery.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ikc.cdnleiting.top

[N05] 最大公约数
来源：http://dsw.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://sqb.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jkg.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rgi.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjy.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ocj.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lzv.fengsongda.top

Ruby: a.gcd(b)
来源：http://wbh.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://skq.dianchejie.cn

[N06] 判断回文字符串
来源：http://otg.uphjek.com

Py:   s == s[::-1]
来源：http://klf.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://oir.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://obk.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://qjt.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://czo.tarul.cn

Go:   // 双指针从两端比较
来源：http://xgk.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://muq.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://zyj.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://ggn.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jkn.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://joe.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://apu.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://pqb.ydjk.org.cn

Java: // 手写 HashMap
来源：http://rxr.shuidangran.top

Go:   // 手写 map[int]int
来源：http://wwi.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://ymd.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://tzw.jyoumei.cn

[N08] 生成全排列
来源：http://ude.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://zcc.hammf.cn

PHP:  // 手写递归交换
来源：http://zok.xylfe.cn

JS:   // 手写回溯递归
来源：http://fao.ctjpmb.com

TS:   // 手写回溯递归
来源：http://mse.chenzaomai.com

Java: // 手写回溯递归
来源：http://nto.jiagoushi.top

Go:   // 手写回溯递归
来源：http://zvh.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://rkn.yongpay.top

C#:   // 手写回溯递归
来源：http://was.yvedp.cn

[N09] 栈与队列
来源：http://sbh.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vos.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shp.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://svm.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://soy.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rlt.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xvy.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aik.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://haz.pengpengdd.cyou

[N10] 链表节点定义
来源：http://rky.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aye.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sxi.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://raa.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yqa.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://zcg.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mat.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://nah.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://eml.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://yex.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gbf.wangdashe.top

PHP:  // 手写递归函数
来源：http://scv.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aux.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mzt.xuanzx.com

Java: // 手写递归
来源：http://pnz.tarul.cn

Go:   // 手写递归
来源：http://dza.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qeq.zycfv.cn

C#:   // 手写递归
来源：http://iqw.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qyo.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zzr.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://apx.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lkz.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ifl.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dkw.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dhg.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qah.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ixh.iojbl.cn

================================================================================
来源：http://kmg.0kj1m.cn

O. 并发与异步
来源：http://uzi.hongshengwenyu.top

================================================================================
来源：http://zgb.snrcjt.cn

[O01] 启动一个线程
来源：http://hiu.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qvz.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mdm.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bdu.ehwqpu.com

TS:   // 同 JS
来源：http://rsn.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://esw.zhijiandao.cn

Go:   go f()
来源：http://tlv.havefunace.top

Ruby: Thread.new { f }
来源：http://mnx.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://ths.yongpay.top

[O02] 使用线程池
来源：http://fep.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qca.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bwe.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://ass.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://ixy.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://una.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pmr.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uhw.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rlt.nwbrower.top

[O03] 加锁保护共享数据
来源：http://kbj.zdbjq.cn

Py:   with lock: shared += 1
来源：http://bja.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://oih.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aus.jinghuilouyu.cn

TS:   // 同 JS
来源：http://yai.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://sgv.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tef.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fvc.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://wma.316326.xyz

[O04] 定义异步函数并等待
来源：http://xfd.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://rdz.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zek.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://bxf.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gdu.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ctm.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://coc.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://hdg.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://zpq.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://vha.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://cjq.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pnb.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://erk.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://mqa.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xic.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhk.tanke756.top

Ruby: threads.map(&:join)
来源：http://ewz.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://anj.shangyingyoupin.top

[O06] 使用进程池
来源：http://vsj.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yax.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://siy.pycfn.com

JS:   // child_process / cluster 模块
来源：http://uwm.cheryme.top

TS:   // child_process / cluster 模块
来源：http://pqn.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tkj.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yky.xinyue.icu

Ruby: // fork 块
来源：http://bkp.yanxiufei.cn

C#:   Parallel.For
来源：http://hoy.mhx1999.top

================================================================================
来源：http://xzo.smart0.xyz

P. 常用工具函数
来源：http://rgx.zhijiandao.cn

================================================================================
来源：http://zvg.redwolf501.top

[P01] 生成 UUID
来源：http://ttx.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://mqv.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eyg.tanke756.top

JS:   crypto.randomUUID()
来源：http://sob.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://yna.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://bqp.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://zlc.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://xzy.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://vhg.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://adc.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://viw.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xhs.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eyg.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://obl.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yod.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bba.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tbb.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rdg.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://tnx.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://poe.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hql.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwb.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mgz.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kgi.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hea.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wxh.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lzq.yvedp.cn

[P04] 求长度
来源：http://mjd.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ihv.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fwq.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xug.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xny.316326.xyz


<!-- 参考信息 -->