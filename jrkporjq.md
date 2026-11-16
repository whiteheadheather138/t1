代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yed.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zbk.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zkq.andypj.xyz

[L06] 解析响应为 JSON
来源：http://gsq.zhongyouzk.top

Py:   resp.json()
来源：http://ban.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://duj.iojbl.cn

JS:   await resp.json()
来源：http://phk.zdqjudy.top

TS:   await resp.json()
来源：http://ctn.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yrg.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nrf.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://pcg.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sid.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://abi.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://acu.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nkr.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://gdo.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://lya.ydjk.org.cn

Java: resp.statusCode()
来源：http://afr.ehwqpu.com

Go:   resp.StatusCode
来源：http://bvz.aibaodan.cn

Ruby: resp.code.to_i
来源：http://lxn.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://nhh.dianchejie.cn

[L08] 并发请求多个地址
来源：http://rib.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://llz.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://eyn.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rne.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rtb.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ilp.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gnh.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lry.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wwe.zhongyouzk.top

================================================================================
来源：http://hev.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://tvy.hammf.cn

================================================================================
来源：http://vke.guowangkeji.top

[M01] 读取命令行参数
来源：http://qeq.yueranfly.top

Py:   sys.argv[1:]
来源：http://ohm.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://eye.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://yad.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://xmv.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://tsy.yfazqb.com

Go:   os.Args[1:]
来源：http://glc.jinyuanbaomall.cn

Ruby: ARGV
来源：http://tkg.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://fee.zhengqikj.top

[M02] 读取环境变量
来源：http://jzl.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://jmj.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xfk.yangfankeji.com

JS:   process.env.HOME
来源：http://zui.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://hai.shuidangran.top

Java: System.getenv("HOME")
来源：http://ndx.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qlp.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://bqv.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://spr.jinqigfzy.top

[M03] 执行外部命令
来源：http://edp.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://moe.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gdb.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jau.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ryf.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uul.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wih.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://bcn.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://nvb.dianchejie.cn

[M04] 获取当前工作目录
来源：http://ada.xziqi.cn

Py:   os.getcwd()
来源：http://zts.sysykeji.top

PHP:  getcwd();
来源：http://ift.jyoumei.cn

JS:   process.cwd()
来源：http://shy.hywenlv.cn

TS:   process.cwd()
来源：http://bcj.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://ods.birdmap.top

Go:   os.Getwd()
来源：http://exv.cucudq.cn

Ruby: Dir.pwd
来源：http://vgt.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://elo.zdbjq.cn

[M05] 设置退出码
来源：http://itm.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://why.cqqwz.cn

PHP:  exit(1);
来源：http://aex.316326.xyz

JS:   process.exit(1)
来源：http://tpd.hammf.cn

TS:   process.exit(1)
来源：http://gbx.dianchejie.cn

Java: System.exit(1)
来源：http://qju.jqgufenzy.top

Go:   os.Exit(1)
来源：http://aoo.xinyue.icu

Ruby: exit 1
来源：http://ljz.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wuw.xinyue.icu

[M06] 向标准错误输出
来源：http://dxn.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://vji.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vvl.gzhubu.top

JS:   console.error("err")
来源：http://dlj.xziqi.cn

TS:   console.error("err")
来源：http://iva.zhixingplan.top

Java: System.err.println("err")
来源：http://qcz.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ntr.cheryme.top

Ruby: warn "err"
来源：http://rmm.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://bod.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://ngb.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://heh.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nvx.havefunace.top

JS:   require.main === module
来源：http://mqy.nanxuanxn.top

TS:   require.main === module
来源：http://mih.guannengcc.top

Java: public static void main(String[] args)
来源：http://yzl.jinghuilouyu.cn

Go:   func main()
来源：http://plh.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pzq.ivvv.top

C#:   static void Main(string[] args)
来源：http://loo.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://qix.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://ugu.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://hwz.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://brz.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://eiw.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zbh.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jdj.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://amj.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://kib.xuanzx.com

================================================================================
来源：http://han.havefunace.top

N. 数据结构与算法
来源：http://mfe.jinqigfzy.top

================================================================================
来源：http://dch.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://dff.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://gro.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hnb.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjj.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xem.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eaq.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://fwl.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ldw.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://ajb.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://amk.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://mpn.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ive.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qau.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vpo.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mqi.hesvh.cn

Go:   slices.Sort(arr)
来源：http://dcv.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://gdr.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yci.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://rvt.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pjr.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://njm.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://puh.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://prw.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://clz.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lgv.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qpl.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ixf.haohaochexian.top

[N04] 斐波那契数列
来源：http://kww.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://djj.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vpe.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zhn.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://myk.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qkg.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hmx.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mya.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://out.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://usi.pycfn.com

Py:   math.gcd(a, b)
来源：http://bqc.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tha.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rgw.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pjc.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://isx.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hcm.yangfankeji.com

Ruby: a.gcd(b)
来源：http://tcb.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dti.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://clr.hfpthk.cn

Py:   s == s[::-1]
来源：http://gwg.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://qpb.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://rhh.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://kak.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vea.hnqzz.top

Go:   // 双指针从两端比较
来源：http://kgp.jianghu66.top

Ruby: s == s.reverse
来源：http://fct.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bks.birdmap.top

[N07] 两数之和（返回下标）
来源：http://fny.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zvf.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://unb.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xgm.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://enl.cheryme.top

Java: // 手写 HashMap
来源：http://yve.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://tcd.gotoacloud.top

Ruby: // 手写 Hash
来源：http://frb.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jbm.sufxvd.cn

[N08] 生成全排列
来源：http://gjp.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://gxu.hesvh.cn

PHP:  // 手写递归交换
来源：http://giv.yangfankeji.com

JS:   // 手写回溯递归
来源：http://kss.pycfn.com

TS:   // 手写回溯递归
来源：http://gzi.yangfankeji.com

Java: // 手写回溯递归
来源：http://otw.jianghu66.top

Go:   // 手写回溯递归
来源：http://lsl.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://qpb.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://ngb.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://sne.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ivz.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fzu.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dif.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wmc.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kfq.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kqi.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ywi.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vcu.aizwys.cn

[N10] 链表节点定义
来源：http://sbu.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhe.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rpm.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hnf.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fsu.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://hcf.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://uff.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mhr.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jot.tarul.cn

[N11] 二叉树中序遍历
来源：http://xxd.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rif.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://ffs.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bvi.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfz.wangshuangyany.cn

Java: // 手写递归
来源：http://zky.jqgufenzy.top

Go:   // 手写递归
来源：http://bmx.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nsp.9152youxi.cn

C#:   // 手写递归
来源：http://amx.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uiz.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hzk.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gfa.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eyo.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qnu.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dqr.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eue.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bsy.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://amv.kuanghao11.cn

================================================================================
来源：http://gsc.c1oappe.top

O. 并发与异步
来源：http://pto.kuanghao11.cn

================================================================================
来源：http://frc.ctjpmb.com

[O01] 启动一个线程
来源：http://zxt.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dsf.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sxq.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wbz.yuanzhike.top

TS:   // 同 JS
来源：http://orn.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://kch.birdmap.top

Go:   go f()
来源：http://dte.dashuyun.cn

Ruby: Thread.new { f }
来源：http://tnh.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://vlu.yj20258888.top

[O02] 使用线程池
来源：http://hrw.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mlg.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vyx.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://igz.shuidangran.top

TS:   // worker_threads 线程池
来源：http://osu.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tns.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tmt.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oxq.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wlm.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://ltg.fengsongda.top

Py:   with lock: shared += 1
来源：http://wti.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://jsn.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kzv.yuxming.cn

TS:   // 同 JS
来源：http://gcs.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://kzb.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ojw.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zdp.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://gac.nanxuanxn.top

[O04] 定义异步函数并等待
来源：http://jbb.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://sky.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nci.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://csb.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pla.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bum.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xie.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://owp.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://che.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://pdr.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://clj.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tck.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://wkk.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://zon.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qro.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yve.tarul.cn

Ruby: threads.map(&:join)
来源：http://mwx.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vpc.andypj.xyz

[O06] 使用进程池
来源：http://wip.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rxw.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://miy.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://nad.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://ggs.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bns.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqp.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://ygm.tianlin.xyz

C#:   Parallel.For
来源：http://gfx.zhengqikj.top

================================================================================
来源：http://bjd.hcnkem.com

P. 常用工具函数
来源：http://kqu.iojbl.cn

================================================================================
来源：http://lxp.nanxinkj.top

[P01] 生成 UUID
来源：http://cpl.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://taz.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rsz.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://aee.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://dkr.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://gxi.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://qwz.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://zdh.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://mgp.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://dsm.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cel.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gya.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://laz.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bzc.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tvj.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xnd.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oxg.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xlu.meibo888.top

[P03] 生成短随机字符串
来源：http://yjt.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zqp.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xep.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hpr.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fjs.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pmp.meibo888.top


<!-- 参考信息 -->