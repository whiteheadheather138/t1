代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jrl.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iph.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://uqq.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zuz.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://wvx.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hoy.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jss.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://pcn.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://bdr.yangfankeji.com

Java: resp.statusCode()
来源：http://yag.smart0.xyz

Go:   resp.StatusCode
来源：http://svs.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://vdu.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://aoa.shuidangran.top

[L08] 并发请求多个地址
来源：http://irg.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zgh.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://jko.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://noa.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jef.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wke.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ufm.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yli.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wsq.hammf.cn

================================================================================
来源：http://xpi.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://myn.dianchejie.cn

================================================================================
来源：http://pky.zycfv.cn

[M01] 读取命令行参数
来源：http://ade.meibo888.top

Py:   sys.argv[1:]
来源：http://gec.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://jut.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://mto.bjfxy.top

TS:   process.argv.slice(2)
来源：http://izn.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://pjw.hnqzz.top

Go:   os.Args[1:]
来源：http://ria.yuxming.cn

Ruby: ARGV
来源：http://lxk.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://klc.uphjek.com

[M02] 读取环境变量
来源：http://tim.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://npo.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mdv.iojbl.cn

JS:   process.env.HOME
来源：http://kyc.wangdashe.top

TS:   process.env.HOME
来源：http://cwe.sxryk.cn

Java: System.getenv("HOME")
来源：http://uwo.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xll.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://gne.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uyu.aibaodan.cn

[M03] 执行外部命令
来源：http://qjj.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vnc.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://owv.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iho.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://geh.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vos.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rnu.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cob.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://ymb.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://eir.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://jag.yangfankeji.com

PHP:  getcwd();
来源：http://ajs.ehwqpu.com

JS:   process.cwd()
来源：http://xsa.yj202588.top

TS:   process.cwd()
来源：http://tll.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://tch.hnqzz.top

Go:   os.Getwd()
来源：http://ojv.ybcxt.top

Ruby: Dir.pwd
来源：http://cpy.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://wce.yfazqb.com

[M05] 设置退出码
来源：http://xpa.xuanzx.com

Py:   sys.exit(1)
来源：http://jnl.tarul.cn

PHP:  exit(1);
来源：http://vhu.tian-w.cn

JS:   process.exit(1)
来源：http://nay.bjfxy.top

TS:   process.exit(1)
来源：http://rci.xinyue.icu

Java: System.exit(1)
来源：http://lmp.yfazqb.com

Go:   os.Exit(1)
来源：http://zzi.xylfe.cn

Ruby: exit 1
来源：http://yrr.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lmg.smart0.xyz

[M06] 向标准错误输出
来源：http://ara.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://rrm.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://upd.gogol.net.cn

JS:   console.error("err")
来源：http://tnv.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://ito.hfpthk.cn

Java: System.err.println("err")
来源：http://xsf.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vbd.ehwqpu.com

Ruby: warn "err"
来源：http://zut.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://rrc.yj20258888.top

[M07] 判断是否为主入口
来源：http://fig.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://jtf.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vey.cheryme.top

JS:   require.main === module
来源：http://wgx.shzxlz.cn

TS:   require.main === module
来源：http://hnz.guowangkeji.top

Java: public static void main(String[] args)
来源：http://htj.jiagoushi.top

Go:   func main()
来源：http://atb.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yke.hesvh.cn

C#:   static void Main(string[] args)
来源：http://bbn.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://aao.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://qkb.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://gro.havefunace.top

JS:   process.platform;  process.version
来源：http://byn.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://vcn.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gmn.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ezw.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iih.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://msk.dianchejie.cn

================================================================================
来源：http://vgl.meibo888.top

N. 数据结构与算法
来源：http://tii.zdbjq.cn

================================================================================
来源：http://wir.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://izi.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://pwd.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fne.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://amz.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wev.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://zuk.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://zxh.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wum.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ojl.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://ubk.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://ioe.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ajv.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xqj.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://upm.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jlo.316326.xyz

Go:   slices.Sort(arr)
来源：http://qno.jinghuilouyu.cn

Ruby: arr.sort
来源：http://yxw.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sjh.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://pnn.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wzu.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://qpd.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mup.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dhg.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bld.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hwf.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whf.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://hfw.yuxming.cn

[N04] 斐波那契数列
来源：http://aoy.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ofa.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mfw.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rfk.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nqs.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ffp.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://goy.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pbz.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cco.hysaishi.cn

[N05] 最大公约数
来源：http://mhv.aizwys.cn

Py:   math.gcd(a, b)
来源：http://nng.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lhc.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gzc.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmt.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://piu.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dek.cdnleiting.top

Ruby: a.gcd(b)
来源：http://kcl.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lqg.zhengqikj.top

[N06] 判断回文字符串
来源：http://zfc.yfazqb.com

Py:   s == s[::-1]
来源：http://fxx.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://ylq.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://kku.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://ufx.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://epl.vehdjk.com

Go:   // 双指针从两端比较
来源：http://iqz.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://qrr.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://prb.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://yjg.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://opi.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tvi.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wyi.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://qku.ydzc1.top

Java: // 手写 HashMap
来源：http://exj.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://fea.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://zqj.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://fkf.zdqjudy.top

[N08] 生成全排列
来源：http://tgu.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://xeh.aibaodan.cn

PHP:  // 手写递归交换
来源：http://nkg.vehdjk.com

JS:   // 手写回溯递归
来源：http://lju.tarul.cn

TS:   // 手写回溯递归
来源：http://fku.guowangkeji.top

Java: // 手写回溯递归
来源：http://vat.haohaochexian.top

Go:   // 手写回溯递归
来源：http://gjl.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://mmb.52xcode.cn

C#:   // 手写回溯递归
来源：http://klr.yj202588.top

[N09] 栈与队列
来源：http://uag.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ybq.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://plp.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wvp.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://scc.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lvl.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oub.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qqm.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dau.gzhubu.top

[N10] 链表节点定义
来源：http://dvw.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pcg.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yet.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bpa.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://csp.birdmap.top

Java: class Node { int v; Node next; }
来源：http://jqv.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://toh.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://hrl.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nvc.bbcook.cn

[N11] 二叉树中序遍历
来源：http://gik.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ihr.aibaodan.cn

PHP:  // 手写递归函数
来源：http://rmu.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvf.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://odc.meibo888.top

Java: // 手写递归
来源：http://gre.chenjidiqi.icu

Go:   // 手写递归
来源：http://xtb.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uqo.kuanghao11.cn

C#:   // 手写递归
来源：http://wdo.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tbh.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yws.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://moo.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bjf.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gzw.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sty.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xxl.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ocp.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ugz.zdbjq.cn

================================================================================
来源：http://ijj.quarkkingdee.top

O. 并发与异步
来源：http://cva.yueranfly.top

================================================================================
来源：http://fzd.316326.xyz

[O01] 启动一个线程
来源：http://mxc.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mwr.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fsu.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yny.bbcook.cn

TS:   // 同 JS
来源：http://yms.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://aee.yj202588.top

Go:   go f()
来源：http://qzo.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://niu.fzhhl.top

C#:   Task.Run(() => F());
来源：http://zka.haohaochexian.top

[O02] 使用线程池
来源：http://vmo.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wfy.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hzt.cucudq.cn

JS:   // worker_threads 线程池
来源：http://fpz.smart0.xyz

TS:   // worker_threads 线程池
来源：http://jae.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://ylx.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bei.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dxz.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nzm.sysykeji.top

[O03] 加锁保护共享数据
来源：http://mnt.snrcjt.cn

Py:   with lock: shared += 1
来源：http://kvr.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://xra.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kob.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://oyn.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://rea.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tdt.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ypj.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://tiv.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://tez.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://sac.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eli.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://ejq.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yuo.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ayc.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tno.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://qle.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://cmx.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://prq.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://cvm.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dcn.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://kqv.yonumen.top

TS:   await Promise.all(tasks)
来源：http://wfx.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ucx.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bce.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://rrp.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://upl.jinqigfzy.top

[O06] 使用进程池
来源：http://mxl.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tcg.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qne.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://okn.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://ofy.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://auh.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://snt.xziqi.cn

Ruby: // fork 块
来源：http://qwn.tian-w.cn

C#:   Parallel.For
来源：http://gus.shangyingyoupin.top

================================================================================
来源：http://ycj.zhongyouzk.top

P. 常用工具函数
来源：http://adg.jlsjyb.cn

================================================================================
来源：http://neo.birdmap.top

[P01] 生成 UUID
来源：http://cnf.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://ckd.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xbe.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://jyl.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://sdr.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://uzp.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://trq.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://zfp.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://mpq.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://wkj.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xyb.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://lrt.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wzr.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fxb.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ico.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tfw.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wqr.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bdl.shzxlz.cn

[P03] 生成短随机字符串
来源：http://zym.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lib.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mhu.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://puz.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hjp.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cbr.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jtb.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gzm.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://acz.guannengcc.top

[P04] 求长度
来源：http://tfs.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nvu.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lgc.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ide.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://czo.yuanzhike.top


<!-- 参考信息 -->