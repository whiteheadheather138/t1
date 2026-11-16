代发 wailian999

Py:   resp.json()
来源：http://jwi.mhx1999.top

PHP:  json_decode($body, true);
来源：http://szq.hcnkem.com

JS:   await resp.json()
来源：http://hsf.zhengqikj.top

TS:   await resp.json()
来源：http://eeb.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://utq.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bwp.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://hlh.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://riu.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://lif.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kxy.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gzy.tanke756.top

JS:   resp.ok;  resp.status
来源：http://skn.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://ejw.kuanghao11.cn

Java: resp.statusCode()
来源：http://wpd.fengsongda.top

Go:   resp.StatusCode
来源：http://cvj.mhx1999.top

Ruby: resp.code.to_i
来源：http://gmb.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://gar.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://csr.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ald.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://zts.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fuo.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nvb.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ppd.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bph.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kws.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cme.shangyingyoupin.top

================================================================================
来源：http://fgx.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://zei.yj202588.top

================================================================================
来源：http://ohs.gzhubu.top

[M01] 读取命令行参数
来源：http://vbn.hfpthk.cn

Py:   sys.argv[1:]
来源：http://aqt.xinyue.icu

PHP:  $argv;  $argc;
来源：http://bbg.hesvh.cn

JS:   process.argv.slice(2)
来源：http://vvm.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://pij.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://pfr.guowangkeji.top

Go:   os.Args[1:]
来源：http://ljt.yanxiufei.cn

Ruby: ARGV
来源：http://wbr.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://sge.havefunace.top

[M02] 读取环境变量
来源：http://fnj.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://ndc.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vau.yvedp.cn

JS:   process.env.HOME
来源：http://ktf.xziqi.cn

TS:   process.env.HOME
来源：http://wlu.dianchejie.cn

Java: System.getenv("HOME")
来源：http://yua.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cvp.yj20258888.top

Ruby: ENV["HOME"]
来源：http://tcm.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sdz.yj202588.top

[M03] 执行外部命令
来源：http://fiz.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xcj.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xch.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uit.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fjq.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hoe.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nxx.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://poo.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://elk.tianlin.xyz

[M04] 获取当前工作目录
来源：http://epz.zycfv.cn

Py:   os.getcwd()
来源：http://ypf.vehdjk.com

PHP:  getcwd();
来源：http://oya.cqqwz.cn

JS:   process.cwd()
来源：http://cln.gaohongyu789.top

TS:   process.cwd()
来源：http://ord.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://jye.jinqigufen.top

Go:   os.Getwd()
来源：http://fmm.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://jya.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yfx.52xcode.cn

[M05] 设置退出码
来源：http://krn.316326.xyz

Py:   sys.exit(1)
来源：http://ofw.zycfv.cn

PHP:  exit(1);
来源：http://slw.zhixingplan.top

JS:   process.exit(1)
来源：http://gwl.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://xsm.ehwqpu.com

Java: System.exit(1)
来源：http://mqb.zdqjudy.top

Go:   os.Exit(1)
来源：http://dhe.tanke756.top

Ruby: exit 1
来源：http://bta.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dqb.tian-w.cn

[M06] 向标准错误输出
来源：http://zxw.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://wmh.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gtk.sufxvd.cn

JS:   console.error("err")
来源：http://oal.bbcook.cn

TS:   console.error("err")
来源：http://mcs.yuanzhike.top

Java: System.err.println("err")
来源：http://anq.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qmc.iojbl.cn

Ruby: warn "err"
来源：http://csp.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://rtw.redwolf501.top

[M07] 判断是否为主入口
来源：http://uuv.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://vpg.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wlt.yangfankeji.com

JS:   require.main === module
来源：http://nqt.fzhhl.top

TS:   require.main === module
来源：http://xwy.jqgfzy.top

Java: public static void main(String[] args)
来源：http://gcw.tianlin.xyz

Go:   func main()
来源：http://ejr.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fxe.aizwys.cn

C#:   static void Main(string[] args)
来源：http://dbj.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://hbr.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://ofe.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://jut.9152youxi.cn

JS:   process.platform;  process.version
来源：http://pdr.zdbjq.cn

TS:   process.platform;  process.version
来源：http://vgj.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://skb.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wwb.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hrj.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wgq.bjfxy.top

================================================================================
来源：http://jxl.svipenyu.cn

N. 数据结构与算法
来源：http://sqc.c1oappe.top

================================================================================
来源：http://qvz.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://mmd.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://tfw.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qyz.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfa.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ayt.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://mxf.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://rkq.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ugc.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://baz.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://gpb.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://gxs.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kcu.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://plr.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vng.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zpn.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://vcs.jianghu66.top

Ruby: arr.sort
来源：http://aci.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vtr.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://qld.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hjm.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://fzd.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esj.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fka.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://twc.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jud.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ydx.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://pdn.ehwqpu.com

[N04] 斐波那契数列
来源：http://cqa.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ucj.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gbv.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hge.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nta.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://beo.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://inw.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xcy.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rrq.meibo888.top

[N05] 最大公约数
来源：http://hkw.sxryk.cn

Py:   math.gcd(a, b)
来源：http://yxt.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fbi.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://erg.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzm.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oeb.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nzn.snrcjt.cn

Ruby: a.gcd(b)
来源：http://scf.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lhy.yonumen.top

[N06] 判断回文字符串
来源：http://mnz.tarul.cn

Py:   s == s[::-1]
来源：http://frd.cucudq.cn

PHP:  $s === strrev($s);
来源：http://rgh.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://gpk.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://kjd.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yug.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://njd.ehwqpu.com

Ruby: s == s.reverse
来源：http://awm.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uwm.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://zzp.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mqo.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ykf.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oaw.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://lrf.zdbjq.cn

Java: // 手写 HashMap
来源：http://yyt.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://llo.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://cxf.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://lvl.shangyingyoupin.top

[N08] 生成全排列
来源：http://hta.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://krs.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://oru.c1oappe.top

JS:   // 手写回溯递归
来源：http://mho.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://uxa.guowangkeji.top

Java: // 手写回溯递归
来源：http://uxs.wangdashe.top

Go:   // 手写回溯递归
来源：http://dep.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://ljk.cheryme.top

C#:   // 手写回溯递归
来源：http://ifh.hnxiangtu.top

[N09] 栈与队列
来源：http://pbr.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://htd.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://imd.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tak.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ngc.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hzl.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rya.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tde.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sok.uphjek.com

[N10] 链表节点定义
来源：http://nxl.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://szt.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mdx.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ikm.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lbm.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://jvw.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://ghl.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jwj.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vzu.aizwys.cn

[N11] 二叉树中序遍历
来源：http://dsr.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dly.chenzaomai.com

PHP:  // 手写递归函数
来源：http://ssw.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlz.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpp.yueranfly.top

Java: // 手写递归
来源：http://vee.zhongyouzk.top

Go:   // 手写递归
来源：http://moq.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rnx.xuetiantiany.cn

C#:   // 手写递归
来源：http://cys.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zfs.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vdo.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygn.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jgr.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kcq.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yiy.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iec.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gde.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://auo.yj20258.top

================================================================================
来源：http://lgz.birdmap.top

O. 并发与异步
来源：http://hgt.jiagoushi.top

================================================================================
来源：http://jaz.52xcode.cn

[O01] 启动一个线程
来源：http://zzr.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://imj.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fan.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dqq.yuxming.cn

TS:   // 同 JS
来源：http://ltr.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://due.yfazqb.com

Go:   go f()
来源：http://zyx.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://ady.yonumen.top

C#:   Task.Run(() => F());
来源：http://edi.sxryk.cn

[O02] 使用线程池
来源：http://avp.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://guo.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sug.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://mbx.yueranfly.top

TS:   // worker_threads 线程池
来源：http://mos.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://ckc.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://upl.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xtp.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gpv.zycfv.cn

[O03] 加锁保护共享数据
来源：http://egu.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://ygq.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://vhg.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pcr.smart0.xyz

TS:   // 同 JS
来源：http://fuc.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://hxx.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jsb.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uvh.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://fsk.redwolf501.top

[O04] 定义异步函数并等待
来源：http://yib.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://bhf.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bpw.fzhhl.top

JS:   async function f() { await g(); }
来源：http://gdo.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tgq.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://avf.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vvj.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://nft.yonumen.top

C#:   async Task F() { await G(); }
来源：http://axd.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://qgv.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://udo.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://skn.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://isc.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://nba.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jho.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lbm.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://okv.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ciz.9152youxi.cn

[O06] 使用进程池
来源：http://ycl.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://umb.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://mzt.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://ygs.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://ozy.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qjq.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zch.hnxiangtu.top

Ruby: // fork 块
来源：http://spp.havefunace.top

C#:   Parallel.For
来源：http://lng.yvedp.cn

================================================================================
来源：http://nzv.gotoacloud.top

P. 常用工具函数
来源：http://lpk.zdqjudy.top

================================================================================
来源：http://uve.tian-w.cn

[P01] 生成 UUID
来源：http://rqf.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://xih.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eym.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://juj.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://jbq.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://suh.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://ogw.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://fqd.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://kbg.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://zfq.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zyq.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yer.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qub.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jdp.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nvb.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ige.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ano.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asa.cdnleiting.top

[P03] 生成短随机字符串
来源：http://uve.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqg.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bmr.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwk.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pyk.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nzx.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xtb.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uwz.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fpt.gogol.net.cn

[P04] 求长度
来源：http://rck.jiagoushi.top


<!-- 参考信息 -->