代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sda.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mui.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bus.aizwys.cn

[L06] 解析响应为 JSON
来源：http://rbv.shzxlz.cn

Py:   resp.json()
来源：http://jxb.yonumen.top

PHP:  json_decode($body, true);
来源：http://fzg.zhongyouzk.top

JS:   await resp.json()
来源：http://huj.yanxiufei.cn

TS:   await resp.json()
来源：http://kch.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wdy.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dyk.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://gbl.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gkk.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://grk.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://imi.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txk.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://xpt.cashguo.top

TS:   resp.ok;  resp.status
来源：http://irs.cdnleiting.top

Java: resp.statusCode()
来源：http://aos.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://nxj.mhx1999.top

Ruby: resp.code.to_i
来源：http://qdn.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://zkj.jqgfzy.top

[L08] 并发请求多个地址
来源：http://saq.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qao.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://jyj.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ggm.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nqc.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tzo.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zwc.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fam.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ifv.chenlongwang.top

================================================================================
来源：http://rig.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://pgc.cdnleiting.top

================================================================================
来源：http://fok.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://ewa.vehdjk.com

Py:   sys.argv[1:]
来源：http://huj.sysykeji.top

PHP:  $argv;  $argc;
来源：http://gam.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://uqi.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://nxz.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://lrz.gotoacloud.top

Go:   os.Args[1:]
来源：http://waj.meibo888.top

Ruby: ARGV
来源：http://bnp.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://okn.hcnkem.com

[M02] 读取环境变量
来源：http://ccz.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://czj.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://avp.jiagoushi.top

JS:   process.env.HOME
来源：http://hby.316326.xyz

TS:   process.env.HOME
来源：http://fur.ybcxt.top

Java: System.getenv("HOME")
来源：http://cvl.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ufx.yj20258888.top

Ruby: ENV["HOME"]
来源：http://ypq.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zgf.svipenyu.cn

[M03] 执行外部命令
来源：http://guc.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ilh.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ihz.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kps.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zug.xziqi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sxw.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://irx.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://pad.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://ile.cheryme.top

[M04] 获取当前工作目录
来源：http://eqq.kuanghao11.cn

Py:   os.getcwd()
来源：http://lkr.chenlongwang.top

PHP:  getcwd();
来源：http://tti.shangyingyoupin.top

JS:   process.cwd()
来源：http://bzv.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://xxa.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://vec.pycfn.com

Go:   os.Getwd()
来源：http://cmo.cdnleiting.top

Ruby: Dir.pwd
来源：http://yeh.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://exn.ydjk.org.cn

[M05] 设置退出码
来源：http://nia.guannengcc.top

Py:   sys.exit(1)
来源：http://rej.shanyushiyangtech.top

PHP:  exit(1);
来源：http://nkj.fengsongda.top

JS:   process.exit(1)
来源：http://pzr.kuanghao11.cn

TS:   process.exit(1)
来源：http://iej.hnqzz.top

Java: System.exit(1)
来源：http://udr.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://ojd.xziqi.cn

Ruby: exit 1
来源：http://rgi.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://crn.ctjpmb.com

[M06] 向标准错误输出
来源：http://zcq.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://gvs.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eqb.guowangkeji.top

JS:   console.error("err")
来源：http://bab.gogol.net.cn

TS:   console.error("err")
来源：http://cpv.gzhubu.top

Java: System.err.println("err")
来源：http://gur.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vwh.fehbvm.com

Ruby: warn "err"
来源：http://tdk.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://wch.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://lji.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://biw.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gpv.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://whp.jinqigufen.top

TS:   require.main === module
来源：http://nzl.yonumen.top

Java: public static void main(String[] args)
来源：http://ucq.52xcode.cn

Go:   func main()
来源：http://zme.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qdy.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://jbr.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://uzc.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://nxx.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://szh.jianghu66.top

JS:   process.platform;  process.version
来源：http://gds.iojbl.cn

TS:   process.platform;  process.version
来源：http://lev.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pbx.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ztq.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://smm.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wiq.ybcxt.top

================================================================================
来源：http://vyr.yangfankeji.com

N. 数据结构与算法
来源：http://kfk.ydjk.org.cn

================================================================================
来源：http://gqy.sweek.top

[N01] 二分查找（有序数组）
来源：http://ikn.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://gwb.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xaq.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tvx.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ynp.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nnb.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://kvu.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://opq.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://lbf.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://xvw.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://sei.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xdj.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fdz.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mkb.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mjs.smart0.xyz

Go:   slices.Sort(arr)
来源：http://sfr.zhixingplan.top

Ruby: arr.sort
来源：http://oca.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tjq.birdmap.top

[N03] 快速排序（分治示例）
来源：http://odh.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://agj.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://gkz.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sdy.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dce.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://him.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cas.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tpu.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dhm.ctjpmb.com

[N04] 斐波那契数列
来源：http://lzb.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://stw.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bom.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jef.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozw.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qdg.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ydz.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nrv.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kpd.vehdjk.com

[N05] 最大公约数
来源：http://obl.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://yfd.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zek.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ftm.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fhj.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tta.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nci.ybcxt.top

Ruby: a.gcd(b)
来源：http://epl.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ram.ehwqpu.com

[N06] 判断回文字符串
来源：http://slm.zdbjq.cn

Py:   s == s[::-1]
来源：http://ogs.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://ykz.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://peu.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://dva.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aox.tian-w.cn

Go:   // 双指针从两端比较
来源：http://dye.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://eth.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xpe.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://btk.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fck.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://phi.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cxo.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://zel.yj20258.top

Java: // 手写 HashMap
来源：http://cje.xinyue.icu

Go:   // 手写 map[int]int
来源：http://ocl.zdbjq.cn

Ruby: // 手写 Hash
来源：http://mhl.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://fxx.svipenyu.cn

[N08] 生成全排列
来源：http://efa.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://boo.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://dxh.hesvh.cn

JS:   // 手写回溯递归
来源：http://qtd.cashguo.top

TS:   // 手写回溯递归
来源：http://ryx.yj20258888.top

Java: // 手写回溯递归
来源：http://gwp.sysykeji.top

Go:   // 手写回溯递归
来源：http://jxf.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://jha.havefunace.top

C#:   // 手写回溯递归
来源：http://dus.aibaodan.cn

[N09] 栈与队列
来源：http://miv.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bah.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gbo.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://owy.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vxy.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://erk.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xev.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pnr.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zix.quarkkingdee.top

[N10] 链表节点定义
来源：http://dkf.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cnb.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rjh.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rwv.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fmn.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://diz.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://jmy.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://czm.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qld.sweek.top

[N11] 二叉树中序遍历
来源：http://zpb.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ooe.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://ilr.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://whn.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ece.jinghuilouyu.cn

Java: // 手写递归
来源：http://xkl.zhixingplan.top

Go:   // 手写递归
来源：http://xyn.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jrf.hfpthk.cn

C#:   // 手写递归
来源：http://tyr.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xpe.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugg.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wtg.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zuf.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://clp.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tbd.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pob.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dhi.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cyn.ybcxt.top

================================================================================
来源：http://hyn.bjfxy.top

O. 并发与异步
来源：http://zhu.cheryme.top

================================================================================
来源：http://kte.hnqzz.top

[O01] 启动一个线程
来源：http://lji.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ovj.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lsw.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qjy.fktsv.cn

TS:   // 同 JS
来源：http://qar.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://rem.chenlongwang.top

Go:   go f()
来源：http://ssw.gogol.net.cn

Ruby: Thread.new { f }
来源：http://ocd.yfazqb.com

C#:   Task.Run(() => F());
来源：http://ysb.dianchejie.cn

[O02] 使用线程池
来源：http://yvw.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lqh.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qhj.xuanzx.com

JS:   // worker_threads 线程池
来源：http://qtv.fktsv.cn

TS:   // worker_threads 线程池
来源：http://ult.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://ixj.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bqm.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kda.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dmn.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://lum.fehbvm.com

Py:   with lock: shared += 1
来源：http://svk.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://qnr.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://adb.zhongyouzk.top

TS:   // 同 JS
来源：http://jqd.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://ptz.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kbj.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zqe.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://juz.bbcook.cn

[O04] 定义异步函数并等待
来源：http://exj.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://niz.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://djl.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://woa.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cfg.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aqb.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dhi.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://bpd.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://ejx.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://xzv.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://ptu.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jnt.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://hvt.uphjek.com

TS:   await Promise.all(tasks)
来源：http://uhi.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eiy.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ngx.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://ygw.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://cyb.sxryk.cn

[O06] 使用进程池
来源：http://khj.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xte.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xfo.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://slw.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://qgy.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aza.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gxi.shzxlz.cn

Ruby: // fork 块
来源：http://lne.jqgufenzy.top

C#:   Parallel.For
来源：http://hqb.c1oappe.top

================================================================================
来源：http://ayx.52xcode.cn

P. 常用工具函数
来源：http://lzz.cucudq.cn

================================================================================
来源：http://pbx.snrcjt.cn

[P01] 生成 UUID
来源：http://zgf.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://kcy.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jqg.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://bcu.meibo888.top

TS:   crypto.randomUUID()
来源：http://wkw.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://vcq.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://fcn.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://nia.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://jhv.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://vci.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mll.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zup.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mkj.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yqf.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ogi.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lov.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ecf.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wgk.guannengcc.top

[P03] 生成短随机字符串
来源：http://qvs.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cjs.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ogo.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwy.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://izu.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://seh.vqdsnc.cn


<!-- 参考信息 -->