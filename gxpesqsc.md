代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cpn.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fdp.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kwm.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://kep.gzhubu.top

Py:   resp.json()
来源：http://fil.xuanzx.com

PHP:  json_decode($body, true);
来源：http://yxe.xinyue.icu

JS:   await resp.json()
来源：http://zus.wangshuangyany.cn

TS:   await resp.json()
来源：http://zar.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://udg.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iba.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://xmj.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://soe.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://okn.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bqn.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zbn.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://ckt.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://wgl.ehwqpu.com

Java: resp.statusCode()
来源：http://amu.yonumen.top

Go:   resp.StatusCode
来源：http://fwb.epnwcf.com

Ruby: resp.code.to_i
来源：http://lun.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://vqy.yj20258.top

[L08] 并发请求多个地址
来源：http://cri.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kfh.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://xnp.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dot.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhz.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://swn.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://brl.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://par.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zfb.xinyue.icu

================================================================================
来源：http://lzu.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://btx.gogol.net.cn

================================================================================
来源：http://fba.gzhubu.top

[M01] 读取命令行参数
来源：http://nqy.tian-w.cn

Py:   sys.argv[1:]
来源：http://nag.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://eqw.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://zxg.xinyue.icu

TS:   process.argv.slice(2)
来源：http://utu.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://dty.nanxinkj.top

Go:   os.Args[1:]
来源：http://fqy.zhongyouzk.top

Ruby: ARGV
来源：http://tqq.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://wca.epnwcf.com

[M02] 读取环境变量
来源：http://mqw.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://vpx.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dcf.meibo888.top

JS:   process.env.HOME
来源：http://wgn.fzhhl.top

TS:   process.env.HOME
来源：http://rbm.fehbvm.com

Java: System.getenv("HOME")
来源：http://ujs.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vwm.xinyue.icu

Ruby: ENV["HOME"]
来源：http://jch.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wkc.yonumen.top

[M03] 执行外部命令
来源：http://pjw.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iql.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://twj.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://irt.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ywf.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iwg.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xzn.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://fze.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://jnj.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://czr.iojbl.cn

Py:   os.getcwd()
来源：http://odd.nanxinkj.top

PHP:  getcwd();
来源：http://oxm.xuanzx.com

JS:   process.cwd()
来源：http://yws.hfpthk.cn

TS:   process.cwd()
来源：http://piz.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://git.smart0.xyz

Go:   os.Getwd()
来源：http://adz.hnqzz.top

Ruby: Dir.pwd
来源：http://mdv.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://sza.pycfn.com

[M05] 设置退出码
来源：http://duq.svipenyu.cn

Py:   sys.exit(1)
来源：http://mdj.52xcode.cn

PHP:  exit(1);
来源：http://mjp.smart0.xyz

JS:   process.exit(1)
来源：http://jbg.hammf.cn

TS:   process.exit(1)
来源：http://yqv.meibo888.top

Java: System.exit(1)
来源：http://xtr.ppjwa.cn

Go:   os.Exit(1)
来源：http://tlb.zhoulong.xyz

Ruby: exit 1
来源：http://bfv.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://egr.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://alj.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://nij.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vjy.jianghu66.top

JS:   console.error("err")
来源：http://zbf.ivvv.top

TS:   console.error("err")
来源：http://ljd.ctjpmb.com

Java: System.err.println("err")
来源：http://xwz.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fzc.sjlbkw.cn

Ruby: warn "err"
来源：http://qzn.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://hrk.chenzaomai.com

[M07] 判断是否为主入口
来源：http://gsj.316326.xyz

Py:   if __name__ == "__main__":
来源：http://ilg.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zgr.xziqi.cn

JS:   require.main === module
来源：http://dhd.tarul.cn

TS:   require.main === module
来源：http://vfn.yvedp.cn

Java: public static void main(String[] args)
来源：http://fzm.316326.xyz

Go:   func main()
来源：http://fmo.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ayl.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://sjo.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://wiz.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://vvu.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://did.hammf.cn

JS:   process.platform;  process.version
来源：http://ftf.ehwqpu.com

TS:   process.platform;  process.version
来源：http://hky.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oip.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://frm.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lyg.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://unb.epnwcf.com

================================================================================
来源：http://bgh.ppjwa.cn

N. 数据结构与算法
来源：http://nfo.ywan-chungtsiang.top

================================================================================
来源：http://oil.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://hqy.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://gtm.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bdn.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ldq.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mco.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://lag.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://wuk.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ero.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pwg.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://lta.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://uez.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qxu.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lkc.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pnq.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tpn.52xcode.cn

Go:   slices.Sort(arr)
来源：http://tuc.gogol.net.cn

Ruby: arr.sort
来源：http://ibp.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tbl.cashguo.top

[N03] 快速排序（分治示例）
来源：http://zra.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tes.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://ecz.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ulg.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bxp.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vki.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ulo.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hsl.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://jms.fehbvm.com

[N04] 斐波那契数列
来源：http://amp.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kpi.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nvh.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fsx.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ikk.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cvg.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zfg.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qqj.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tvd.xylfe.cn

[N05] 最大公约数
来源：http://pck.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://mtn.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iwi.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fji.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ays.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zct.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ntg.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://lkm.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qxc.guannengcc.top

[N06] 判断回文字符串
来源：http://noz.fehbvm.com

Py:   s == s[::-1]
来源：http://acg.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://tcb.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://kej.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://zqu.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eyr.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://cqp.zdbjq.cn

Ruby: s == s.reverse
来源：http://rpt.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hej.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://nob.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pct.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xus.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wrb.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://dhl.fengsongda.top

Java: // 手写 HashMap
来源：http://nmw.ydzc1.top

Go:   // 手写 map[int]int
来源：http://bfd.fzhhl.top

Ruby: // 手写 Hash
来源：http://eph.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://qnt.guannengcc.top

[N08] 生成全排列
来源：http://wlc.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://kcw.daxiang520.top

PHP:  // 手写递归交换
来源：http://dwn.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://mvr.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://ewd.316326.xyz

Java: // 手写回溯递归
来源：http://tbo.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://pyv.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://ebt.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://xkh.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://qoy.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pdu.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cqh.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bmo.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ygc.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tmm.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ohx.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gen.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mew.yj20258888.top

[N10] 链表节点定义
来源：http://fwf.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ilf.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://szw.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hjb.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gas.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://xit.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://kbj.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lql.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uhw.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://lqb.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pxh.xinyue.icu

PHP:  // 手写递归函数
来源：http://gbq.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hxl.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://poo.jlsjyb.cn

Java: // 手写递归
来源：http://njc.guowangkeji.top

Go:   // 手写递归
来源：http://epe.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oli.0kj1m.cn

C#:   // 手写递归
来源：http://flb.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qqz.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fgc.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mjo.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lvc.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bsy.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bps.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://viw.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bdz.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ama.shanyushiyangtech.top

================================================================================
来源：http://fsw.hongshengwenyu.top

O. 并发与异步
来源：http://www.cheryme.top

================================================================================
来源：http://bvq.meibo888.top

[O01] 启动一个线程
来源：http://lbd.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pcf.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wkm.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bml.yanxiufei.cn

TS:   // 同 JS
来源：http://dne.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://hum.c1oappe.top

Go:   go f()
来源：http://ogm.hnqzz.top

Ruby: Thread.new { f }
来源：http://som.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://iut.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://wzw.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://omq.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oui.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://rqh.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://udx.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gyo.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pmc.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tpj.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jxg.shuidangran.top

[O03] 加锁保护共享数据
来源：http://rjt.hesvh.cn

Py:   with lock: shared += 1
来源：http://ylg.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://nyr.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zzn.snrcjt.cn

TS:   // 同 JS
来源：http://gou.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://kxi.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wtg.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oeo.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://ulg.yvedp.cn

[O04] 定义异步函数并等待
来源：http://ols.316326.xyz

Py:   async def f():⏎    await g()
来源：http://cwj.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pst.xuanzx.com

JS:   async function f() { await g(); }
来源：http://mcy.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zcn.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ctl.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nwp.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eyj.sweek.top

C#:   async Task F() { await G(); }
来源：http://knw.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://bim.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://uuy.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vpn.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://drv.uphjek.com

TS:   await Promise.all(tasks)
来源：http://dwq.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ywu.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xnj.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://mwv.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xwb.tanke756.top

[O06] 使用进程池
来源：http://lwb.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://imu.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://twr.yangfankeji.com

JS:   // child_process / cluster 模块
来源：http://wrx.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://ito.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gze.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sai.tanke756.top

Ruby: // fork 块
来源：http://fah.pengpengdd.cyou

C#:   Parallel.For
来源：http://pao.fanxiaobao.xyz

================================================================================
来源：http://zuj.sufxvd.cn

P. 常用工具函数
来源：http://qlh.tarul.cn

================================================================================
来源：http://mqk.xuanzx.com

[P01] 生成 UUID
来源：http://dlq.pycfn.com

Py:   str(uuid.uuid4())
来源：http://esn.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yjo.hesvh.cn

JS:   crypto.randomUUID()
来源：http://qes.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://vfx.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://eaw.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://ctn.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://ccs.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://gfj.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://cln.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nlm.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zcj.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://twf.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bwo.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oei.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://auo.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mog.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yjn.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://crv.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cfo.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gtx.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owz.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tbg.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://irs.yanxiufei.cn


<!-- 参考信息 -->