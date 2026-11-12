代发 wailian999

Py:   resp.json()
来源：http://qoa.iojbl.cn

PHP:  json_decode($body, true);
来源：http://fwh.gzhubu.top

JS:   await resp.json()
来源：http://pcy.ydzc1.top

TS:   await resp.json()
来源：http://xgd.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oml.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vfr.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://vuo.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sun.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://zpf.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cxa.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wld.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://hoy.pycfn.com

TS:   resp.ok;  resp.status
来源：http://wtb.svipenyu.cn

Java: resp.statusCode()
来源：http://yyo.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://kbc.cucudq.cn

Ruby: resp.code.to_i
来源：http://flg.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://ppk.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://sjt.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vog.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://oev.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kvh.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nbw.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jma.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bjb.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eie.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vmn.zhaomingkeji.xyz

================================================================================
来源：http://gjg.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://jug.zhijiandao.cn

================================================================================
来源：http://ztn.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://tgi.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://zyh.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://riz.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://sfl.mhx1999.top

TS:   process.argv.slice(2)
来源：http://gvu.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://htv.nanxuanxn.top

Go:   os.Args[1:]
来源：http://qbj.feifeiyinyue.top

Ruby: ARGV
来源：http://jor.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://mmf.gzhubu.top

[M02] 读取环境变量
来源：http://xwb.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://bgn.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lzn.sweek.top

JS:   process.env.HOME
来源：http://clf.bjfxy.top

TS:   process.env.HOME
来源：http://ifz.jyoumei.cn

Java: System.getenv("HOME")
来源：http://wge.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ypt.xylfe.cn

Ruby: ENV["HOME"]
来源：http://cwk.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gox.hesvh.cn

[M03] 执行外部命令
来源：http://iri.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qon.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vlj.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lsp.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ilv.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yzn.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://sda.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ujw.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://rnm.jinqigufen.top

[M04] 获取当前工作目录
来源：http://qpm.zhijiandao.cn

Py:   os.getcwd()
来源：http://pfz.ydjk.org.cn

PHP:  getcwd();
来源：http://gkh.jinqigufen.top

JS:   process.cwd()
来源：http://lmp.daria6918.cn

TS:   process.cwd()
来源：http://ero.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://ndy.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://hbs.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://aox.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rjc.fehbvm.com

[M05] 设置退出码
来源：http://mgq.hnqzz.top

Py:   sys.exit(1)
来源：http://glj.guannengcc.top

PHP:  exit(1);
来源：http://roe.chenjidiqi.icu

JS:   process.exit(1)
来源：http://yex.0kj1m.cn

TS:   process.exit(1)
来源：http://osa.fanxiaobao.xyz

Java: System.exit(1)
来源：http://nej.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://tjw.zhoulong.xyz

Ruby: exit 1
来源：http://nlc.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nwz.cashguo.top

[M06] 向标准错误输出
来源：http://jfs.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://aef.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mki.sxryk.cn

JS:   console.error("err")
来源：http://zen.tarul.cn

TS:   console.error("err")
来源：http://zud.aibaodan.cn

Java: System.err.println("err")
来源：http://gla.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://udb.shuidangran.top

Ruby: warn "err"
来源：http://kkc.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://igz.gotoacloud.top

[M07] 判断是否为主入口
来源：http://thf.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://upb.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zia.cheryme.top

JS:   require.main === module
来源：http://jow.fengsongda.top

TS:   require.main === module
来源：http://yfs.ivvv.top

Java: public static void main(String[] args)
来源：http://jto.zhongyouzk.top

Go:   func main()
来源：http://tsr.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://joa.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://coi.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://xvs.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://qbo.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://ngv.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://cwj.cdnleiting.top

TS:   process.platform;  process.version
来源：http://jth.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://umf.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vub.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dox.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xrs.zycfv.cn

================================================================================
来源：http://trc.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://byx.yuxming.cn

================================================================================
来源：http://emq.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://fgb.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://wjo.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vdq.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gyr.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ava.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://mfd.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://xcs.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fcz.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://urh.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://kpp.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://sba.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://owu.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yjz.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rmx.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://btv.pycfn.com

Go:   slices.Sort(arr)
来源：http://uci.jianghu66.top

Ruby: arr.sort
来源：http://pys.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jme.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://oyb.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dlu.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://pcw.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dww.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qga.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://icu.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lgl.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wqw.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ysf.xuanzx.com

[N04] 斐波那契数列
来源：http://iyu.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://srv.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ixo.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://apl.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ncw.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hje.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mzm.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wim.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dtq.cheryme.top

[N05] 最大公约数
来源：http://pug.yj20258.top

Py:   math.gcd(a, b)
来源：http://nvx.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://soy.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eli.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mlx.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://caw.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bms.yonumen.top

Ruby: a.gcd(b)
来源：http://ppi.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hcd.nanxinkj.top

[N06] 判断回文字符串
来源：http://bmi.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://eek.meibo888.top

PHP:  $s === strrev($s);
来源：http://xqo.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://ahr.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://lxe.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jfp.fengsongda.top

Go:   // 双指针从两端比较
来源：http://vby.sufxvd.cn

Ruby: s == s.reverse
来源：http://buy.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zqv.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://tgr.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pba.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mdj.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://afb.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://iex.vqdsnc.cn

Java: // 手写 HashMap
来源：http://sev.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://gcf.sysykeji.top

Ruby: // 手写 Hash
来源：http://jew.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://oas.birdmap.top

[N08] 生成全排列
来源：http://cyp.tanke756.top

Py:   itertools.permutations(arr)
来源：http://zhg.pycfn.com

PHP:  // 手写递归交换
来源：http://qsf.ivvv.top

JS:   // 手写回溯递归
来源：http://msf.zhixingplan.top

TS:   // 手写回溯递归
来源：http://mvx.jyoumei.cn

Java: // 手写回溯递归
来源：http://mqt.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://vic.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://mod.hywenlv.cn

C#:   // 手写回溯递归
来源：http://gwh.hywenlv.cn

[N09] 栈与队列
来源：http://irz.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://thg.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cae.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fmi.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dob.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sac.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nms.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pwo.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fle.aizwys.cn

[N10] 链表节点定义
来源：http://hyy.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://njm.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hmh.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cll.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://plc.uphjek.com

Java: class Node { int v; Node next; }
来源：http://uqx.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://iir.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hea.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tba.xinyue.icu

[N11] 二叉树中序遍历
来源：http://adt.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rvr.yangfankeji.com

PHP:  // 手写递归函数
来源：http://pll.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gwl.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yxv.c1oappe.top

Java: // 手写递归
来源：http://fko.yueranfly.top

Go:   // 手写递归
来源：http://lgv.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nmk.zhijiandao.cn

C#:   // 手写递归
来源：http://cbu.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://haq.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://prp.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tuv.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uvj.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrz.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tvc.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xnk.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rrf.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kgq.gaohongyu789.top

================================================================================
来源：http://hnc.bjfxy.top

O. 并发与异步
来源：http://jgc.zhoulong.xyz

================================================================================
来源：http://mjc.jianghu66.top

[O01] 启动一个线程
来源：http://soj.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://elj.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bxr.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mbo.xylfe.cn

TS:   // 同 JS
来源：http://xly.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://lzk.ehwqpu.com

Go:   go f()
来源：http://yps.hywenlv.cn

Ruby: Thread.new { f }
来源：http://yws.uphjek.com

C#:   Task.Run(() => F());
来源：http://ahe.yj202588.top

[O02] 使用线程池
来源：http://tgb.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fhg.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://odm.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://jse.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://hnj.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://khh.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fwj.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bgs.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ssl.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://hhs.fehbvm.com

Py:   with lock: shared += 1
来源：http://ubo.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://lzo.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://alb.sysykeji.top

TS:   // 同 JS
来源：http://zzy.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://scf.ydzc1.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qsa.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jvv.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://azh.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://lln.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://fto.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hrz.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://rds.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jdi.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dsg.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vfa.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jgj.hammf.cn

C#:   async Task F() { await G(); }
来源：http://sdu.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://tkf.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://vyg.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mba.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://ebo.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://mef.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yip.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mvq.ivvv.top

Ruby: threads.map(&:join)
来源：http://uon.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uwq.zdqjudy.top

[O06] 使用进程池
来源：http://mjk.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cay.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ove.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://mne.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://wqu.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jhn.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jta.xylfe.cn

Ruby: // fork 块
来源：http://cbp.jlsjyb.cn

C#:   Parallel.For
来源：http://tcv.guannengcc.top

================================================================================
来源：http://wnk.guannengcc.top

P. 常用工具函数
来源：http://wew.fanxiaobao.xyz

================================================================================
来源：http://hwj.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://iml.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://dbu.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lgg.vehdjk.com

JS:   crypto.randomUUID()
来源：http://xnh.zhiwuduotai.top

TS:   crypto.randomUUID()
来源：http://osi.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://rcb.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://sxh.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://vjc.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://odr.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://xri.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vuv.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hgc.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yxz.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://abp.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tzb.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kvt.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kwl.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wmg.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://ahu.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://coz.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nfq.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://utf.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klk.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://btf.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kri.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dzh.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zxn.daria6918.cn

[P04] 求长度
来源：http://cnl.sweek.top


<!-- 参考信息 -->