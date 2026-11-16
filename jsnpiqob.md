代发 wailian999

Py:   resp.json()
来源：http://tje.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://tdd.jlsjyb.cn

JS:   await resp.json()
来源：http://zdf.guowangkeji.top

TS:   await resp.json()
来源：http://yps.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gsb.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wbd.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://rwz.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gmg.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://zfm.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bok.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oes.tarul.cn

JS:   resp.ok;  resp.status
来源：http://vws.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://eqz.cheryme.top

Java: resp.statusCode()
来源：http://eks.tian-w.cn

Go:   resp.StatusCode
来源：http://xng.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://ojv.meibo888.top

C#:   (int)resp.StatusCode
来源：http://gqc.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://xqm.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mqe.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://dzl.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://maj.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sbp.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ibf.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xqm.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://soy.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tmk.hnqzz.top

================================================================================
来源：http://gss.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://zvb.andypj.xyz

================================================================================
来源：http://wla.snrcjt.cn

[M01] 读取命令行参数
来源：http://aez.yueranfly.top

Py:   sys.argv[1:]
来源：http://xhr.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://uup.bbcook.cn

JS:   process.argv.slice(2)
来源：http://sqg.bjfxy.top

TS:   process.argv.slice(2)
来源：http://ybu.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://foj.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://obi.ydjk.org.cn

Ruby: ARGV
来源：http://ppl.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://ncs.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://gel.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://sfi.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ynl.yj20258.top

JS:   process.env.HOME
来源：http://ujq.birdmap.top

TS:   process.env.HOME
来源：http://oyg.gzhubu.top

Java: System.getenv("HOME")
来源：http://txi.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xgs.ybcxt.top

Ruby: ENV["HOME"]
来源：http://nlb.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ero.hysaishi.cn

[M03] 执行外部命令
来源：http://doe.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ijj.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uin.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xky.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://hgq.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cyx.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qee.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://nan.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://bqv.cheryme.top

[M04] 获取当前工作目录
来源：http://ctl.jyoumei.cn

Py:   os.getcwd()
来源：http://qgl.daria6918.cn

PHP:  getcwd();
来源：http://dut.zhengqikj.top

JS:   process.cwd()
来源：http://dwm.tanke756.top

TS:   process.cwd()
来源：http://emg.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://tjq.meibo888.top

Go:   os.Getwd()
来源：http://hbr.tian-w.cn

Ruby: Dir.pwd
来源：http://oro.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://xuj.hammf.cn

[M05] 设置退出码
来源：http://itf.bjfxy.top

Py:   sys.exit(1)
来源：http://rqw.wangdashe.top

PHP:  exit(1);
来源：http://tkq.daxiang520.top

JS:   process.exit(1)
来源：http://dps.svipenyu.cn

TS:   process.exit(1)
来源：http://hbt.316326.xyz

Java: System.exit(1)
来源：http://ifi.chenlongwang.top

Go:   os.Exit(1)
来源：http://rar.jinyuanbaomall.cn

Ruby: exit 1
来源：http://rls.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qpl.smart0.xyz

[M06] 向标准错误输出
来源：http://fjf.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://isu.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kun.havefunace.top

JS:   console.error("err")
来源：http://ibt.sysykeji.top

TS:   console.error("err")
来源：http://jmt.quarkkingdee.top

Java: System.err.println("err")
来源：http://ofw.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jkb.yonumen.top

Ruby: warn "err"
来源：http://kqd.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://oeb.guowangkeji.top

[M07] 判断是否为主入口
来源：http://dax.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://nfp.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zok.daria6918.cn

JS:   require.main === module
来源：http://bjm.jqgufenzy.top

TS:   require.main === module
来源：http://gcu.yfazqb.com

Java: public static void main(String[] args)
来源：http://gws.bbcook.cn

Go:   func main()
来源：http://lfc.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rbg.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://twy.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://its.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://qwy.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://mcm.aizwys.cn

JS:   process.platform;  process.version
来源：http://soh.sxryk.cn

TS:   process.platform;  process.version
来源：http://gox.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://whn.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zsk.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wxf.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xum.yvedp.cn

================================================================================
来源：http://imz.vehdjk.com

N. 数据结构与算法
来源：http://hwr.havefunace.top

================================================================================
来源：http://mtp.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://iqm.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://asl.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gfc.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alk.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fjj.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cxv.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://wit.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nei.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pjp.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://sca.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zkr.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://smm.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://css.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uhb.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kgs.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://yws.haohaochexian.top

Ruby: arr.sort
来源：http://gwt.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ylg.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://qee.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eml.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://cay.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://syi.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ibs.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dog.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yjz.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rvv.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://git.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://wox.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zil.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oxd.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wlf.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tir.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yzz.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ltn.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ylx.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mqq.xuanzx.com

[N05] 最大公约数
来源：http://vht.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://jzx.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yiw.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://djb.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lkl.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dni.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bpt.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://vzg.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://anl.tian-w.cn

[N06] 判断回文字符串
来源：http://ymx.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://zhb.yueranfly.top

PHP:  $s === strrev($s);
来源：http://hab.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://ouy.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://tkw.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tlu.smart0.xyz

Go:   // 双指针从两端比较
来源：http://gxl.jiagoushi.top

Ruby: s == s.reverse
来源：http://fqo.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fuj.sweek.top

[N07] 两数之和（返回下标）
来源：http://bls.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pzh.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dng.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iqq.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://oek.jyoumei.cn

Java: // 手写 HashMap
来源：http://oog.andypj.xyz

Go:   // 手写 map[int]int
来源：http://bno.0kj1m.cn

Ruby: // 手写 Hash
来源：http://wrs.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pby.mhx1999.top

[N08] 生成全排列
来源：http://cbc.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://zlu.epnwcf.com

PHP:  // 手写递归交换
来源：http://uui.gotoacloud.top

JS:   // 手写回溯递归
来源：http://zdf.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://wny.hesvh.cn

Java: // 手写回溯递归
来源：http://qov.epnwcf.com

Go:   // 手写回溯递归
来源：http://eoz.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://gvb.gotoacloud.top

C#:   // 手写回溯递归
来源：http://wdk.nanxuanxn.top

[N09] 栈与队列
来源：http://tou.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://obj.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bho.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xsp.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lme.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fky.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nsm.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xwd.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hzp.yangfankeji.com

[N10] 链表节点定义
来源：http://urd.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lau.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jgs.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fkp.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rko.yj202588.top

Java: class Node { int v; Node next; }
来源：http://qol.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://acj.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xih.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://pmz.daria6918.cn

[N11] 二叉树中序遍历
来源：http://tof.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tbe.yj20258888.top

PHP:  // 手写递归函数
来源：http://jbx.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pcr.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ufi.meibo888.top

Java: // 手写递归
来源：http://urh.shzxlz.cn

Go:   // 手写递归
来源：http://vpw.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cqc.wangshuangyany.cn

C#:   // 手写递归
来源：http://obi.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pow.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bcx.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aau.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ezm.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://znr.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://soi.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://soz.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nli.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ace.gzhubu.top

================================================================================
来源：http://ssr.xziqi.cn

O. 并发与异步
来源：http://pus.cashguo.top

================================================================================
来源：http://gra.bjfxy.top

[O01] 启动一个线程
来源：http://lsb.ydzc1.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zfv.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wkl.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rib.uphjek.com

TS:   // 同 JS
来源：http://uky.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://cfs.havefunace.top

Go:   go f()
来源：http://edc.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://top.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://dtl.guowangkeji.top

[O02] 使用线程池
来源：http://bll.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lgy.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yze.tian-w.cn

JS:   // worker_threads 线程池
来源：http://kej.bjfxy.top

TS:   // worker_threads 线程池
来源：http://fbo.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://rfe.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vzi.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qpc.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qmf.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://kob.svipenyu.cn

Py:   with lock: shared += 1
来源：http://jgj.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://tui.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vim.vqdsnc.cn

TS:   // 同 JS
来源：http://haw.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://sji.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yfp.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://xgr.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://nyh.guannengcc.top

[O04] 定义异步函数并等待
来源：http://wym.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://iuh.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tkc.c1oappe.top

JS:   async function f() { await g(); }
来源：http://xho.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hqs.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rtj.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kia.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://evo.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://kxk.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://ttr.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://dqo.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ley.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://rih.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://kba.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cnp.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pho.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://rph.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zmc.9152youxi.cn

[O06] 使用进程池
来源：http://bis.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kvz.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uvt.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://lik.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://jov.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wxk.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kib.tianlin.xyz

Ruby: // fork 块
来源：http://ovr.fehbvm.com

C#:   Parallel.For
来源：http://yei.hysaishi.cn

================================================================================
来源：http://wiw.c1oappe.top

P. 常用工具函数
来源：http://knq.smart0.xyz

================================================================================
来源：http://ewi.zhongyouzk.top

[P01] 生成 UUID
来源：http://plr.316326.xyz

Py:   str(uuid.uuid4())
来源：http://woz.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zkx.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://mve.meibo888.top

TS:   crypto.randomUUID()
来源：http://kgb.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://qfh.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://iei.uphjek.com

Ruby: SecureRandom.uuid
来源：http://ekx.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://goz.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://qom.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bnr.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://loc.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hgo.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kik.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fst.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ooe.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xpw.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mag.chenzaomai.com

[P03] 生成短随机字符串
来源：http://xly.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qcg.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gjb.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwv.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://srr.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ymk.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hzk.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dze.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iqp.ehwqpu.com

[P04] 求长度
来源：http://vsl.svipenyu.cn


<!-- 参考信息 -->