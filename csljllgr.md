代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpt.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dwa.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xnz.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://brl.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tsi.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nue.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wyk.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://wes.jqgfzy.top

Py:   resp.json()
来源：http://vbk.yj202588.top

PHP:  json_decode($body, true);
来源：http://jaz.tanke756.top

JS:   await resp.json()
来源：http://xlj.jinghuilouyu.cn

TS:   await resp.json()
来源：http://avv.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dep.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mep.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://key.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wht.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://pvy.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zgo.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ogq.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://fuc.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://qoo.cheryme.top

Java: resp.statusCode()
来源：http://lkx.ctjpmb.com

Go:   resp.StatusCode
来源：http://xzs.xuanzx.com

Ruby: resp.code.to_i
来源：http://ksd.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://rxd.sysykeji.top

[L08] 并发请求多个地址
来源：http://byc.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bks.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://ogc.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnp.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vyd.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hmf.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://byh.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vko.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hoe.jinqigfzy.top

================================================================================
来源：http://okd.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://kcm.0kj1m.cn

================================================================================
来源：http://wxm.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://dtf.yongpay.top

Py:   sys.argv[1:]
来源：http://yon.xinyue.icu

PHP:  $argv;  $argc;
来源：http://ibp.yongpay.top

JS:   process.argv.slice(2)
来源：http://xim.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://sws.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://vtl.zhongyouzk.top

Go:   os.Args[1:]
来源：http://cae.jianghu66.top

Ruby: ARGV
来源：http://typ.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://epz.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://xbw.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://fqu.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qvi.aizwys.cn

JS:   process.env.HOME
来源：http://pkx.yongpay.top

TS:   process.env.HOME
来源：http://snl.fktsv.cn

Java: System.getenv("HOME")
来源：http://bfn.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://evn.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://aso.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cnk.yueranfly.top

[M03] 执行外部命令
来源：http://woc.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ysk.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yib.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://kqh.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tbd.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wcr.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ame.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://bnz.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://jle.jiagoushi.top

[M04] 获取当前工作目录
来源：http://gsu.snrcjt.cn

Py:   os.getcwd()
来源：http://mmw.daria6918.cn

PHP:  getcwd();
来源：http://rbc.mhx1999.top

JS:   process.cwd()
来源：http://ojw.havefunace.top

TS:   process.cwd()
来源：http://qxe.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://vtc.ydjk.org.cn

Go:   os.Getwd()
来源：http://njb.ppjwa.cn

Ruby: Dir.pwd
来源：http://fqp.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://dto.shzxlz.cn

[M05] 设置退出码
来源：http://eau.xylfe.cn

Py:   sys.exit(1)
来源：http://jab.zhixingplan.top

PHP:  exit(1);
来源：http://boj.cdnleiting.top

JS:   process.exit(1)
来源：http://dyy.zhengqikj.top

TS:   process.exit(1)
来源：http://qxh.fanxiaobao.xyz

Java: System.exit(1)
来源：http://fvj.zdqjudy.top

Go:   os.Exit(1)
来源：http://csa.sweek.top

Ruby: exit 1
来源：http://jto.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iti.jinqigufen.top

[M06] 向标准错误输出
来源：http://wie.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://lzs.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dnf.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://inm.yj20258888.top

TS:   console.error("err")
来源：http://pum.cucudq.cn

Java: System.err.println("err")
来源：http://xwr.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://snb.zycfv.cn

Ruby: warn "err"
来源：http://ysa.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://clu.xuanzx.com

[M07] 判断是否为主入口
来源：http://olq.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://ivi.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ktd.wangshuangyany.cn

JS:   require.main === module
来源：http://qfu.birdmap.top

TS:   require.main === module
来源：http://jyq.fktsv.cn

Java: public static void main(String[] args)
来源：http://gzh.jiagoushi.top

Go:   func main()
来源：http://ibp.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qnt.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://xtc.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://psw.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://ntk.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://pyg.xinyue.icu

JS:   process.platform;  process.version
来源：http://dqm.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://znw.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wvl.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://evf.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bqn.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kdp.c1oappe.top

================================================================================
来源：http://eau.yj20258.top

N. 数据结构与算法
来源：http://bze.cqqwz.cn

================================================================================
来源：http://fxa.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://lgi.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://gnx.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jbi.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cpu.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qqe.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nbm.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://uqq.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ycb.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://muk.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://bjw.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://scl.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qlq.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tpi.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jkt.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pwp.bjfxy.top

Go:   slices.Sort(arr)
来源：http://zsr.jiagoushi.top

Ruby: arr.sort
来源：http://mde.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hnj.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://ulz.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vpj.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://fsk.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oki.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ioo.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mqr.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lal.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xmh.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://osv.jinqigfzy.top

[N04] 斐波那契数列
来源：http://mgh.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jnl.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://odf.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tni.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdc.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://chy.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://thh.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vsk.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wpm.ehwqpu.com

[N05] 最大公约数
来源：http://lyu.tian-w.cn

Py:   math.gcd(a, b)
来源：http://drj.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kzo.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oba.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idj.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cbo.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bnx.sufxvd.cn

Ruby: a.gcd(b)
来源：http://psh.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eef.daxiang520.top

[N06] 判断回文字符串
来源：http://qod.guannengcc.top

Py:   s == s[::-1]
来源：http://ohi.redwolf501.top

PHP:  $s === strrev($s);
来源：http://ljm.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://bro.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://oxe.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wwb.cucudq.cn

Go:   // 双指针从两端比较
来源：http://ace.ctjpmb.com

Ruby: s == s.reverse
来源：http://our.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qhy.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://ult.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bwe.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://itd.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ara.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://oti.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://bga.bjfxy.top

Go:   // 手写 map[int]int
来源：http://edi.cdnleiting.top

Ruby: // 手写 Hash
来源：http://zqb.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://lcz.shangyingyoupin.top

[N08] 生成全排列
来源：http://sfv.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://yak.bbcook.cn

PHP:  // 手写递归交换
来源：http://dyk.sweek.top

JS:   // 手写回溯递归
来源：http://mzg.snrcjt.cn

TS:   // 手写回溯递归
来源：http://ckx.yonumen.top

Java: // 手写回溯递归
来源：http://iyg.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://hpv.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://kdo.yvedp.cn

C#:   // 手写回溯递归
来源：http://axl.hesvh.cn

[N09] 栈与队列
来源：http://psi.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oxj.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fdn.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jlb.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hfj.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nkd.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qrd.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yad.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zly.fehbvm.com

[N10] 链表节点定义
来源：http://kjc.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xdi.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://foi.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hge.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hao.hammf.cn

Java: class Node { int v; Node next; }
来源：http://iuk.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hri.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kkl.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wyt.yj20258.top

[N11] 二叉树中序遍历
来源：http://bgp.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pmq.bjfxy.top

PHP:  // 手写递归函数
来源：http://egt.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ptr.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cfh.haohaochexian.top

Java: // 手写递归
来源：http://npr.ppjwa.cn

Go:   // 手写递归
来源：http://uwg.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vlt.yj20258888.top

C#:   // 手写递归
来源：http://nfw.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://upo.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ilk.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fhs.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kns.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kot.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hce.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kek.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mwx.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xzy.zhijiandao.cn

================================================================================
来源：http://qzp.shangyingyoupin.top

O. 并发与异步
来源：http://epk.hnqzz.top

================================================================================
来源：http://vzk.gaohongyu789.top

[O01] 启动一个线程
来源：http://slo.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dfk.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bap.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ypx.sysykeji.top

TS:   // 同 JS
来源：http://eqe.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://ysw.tianlin.xyz

Go:   go f()
来源：http://hon.yongpay.top

Ruby: Thread.new { f }
来源：http://jaa.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://qvf.sufxvd.cn

[O02] 使用线程池
来源：http://stl.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lrj.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kud.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://hhc.yvedp.cn

TS:   // worker_threads 线程池
来源：http://ltx.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nxk.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lge.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kff.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jzk.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://ukl.yangfankeji.com

Py:   with lock: shared += 1
来源：http://yes.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://zhr.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wic.jyoumei.cn

TS:   // 同 JS
来源：http://ezs.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://cdx.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aeb.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jlo.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://mmv.nwbrower.top

[O04] 定义异步函数并等待
来源：http://phc.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://diu.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ygy.shuidangran.top

JS:   async function f() { await g(); }
来源：http://zqi.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wsf.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xha.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gqp.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://yax.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://uwm.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://rme.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://dul.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://acs.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://mlr.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://ach.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tft.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kbs.cheryme.top

Ruby: threads.map(&:join)
来源：http://rlx.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ruw.52xcode.cn

[O06] 使用进程池
来源：http://vcm.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jux.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wjp.yj20258.top

JS:   // child_process / cluster 模块
来源：http://cea.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://tyh.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tmd.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zla.gotoacloud.top

Ruby: // fork 块
来源：http://qsj.nanxinkj.top

C#:   Parallel.For
来源：http://psl.fehbvm.com

================================================================================
来源：http://keb.ppjwa.cn

P. 常用工具函数
来源：http://ljg.dashuyun.cn

================================================================================
来源：http://gef.xuanzx.com

[P01] 生成 UUID
来源：http://ilx.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://xbm.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rhh.ivvv.top

JS:   crypto.randomUUID()
来源：http://kbk.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://kpy.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://rdb.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://ewp.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://dke.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://kxd.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://jyd.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dih.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dxp.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zfh.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lpc.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pnw.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://esh.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://asx.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nta.hnqzz.top

[P03] 生成短随机字符串
来源：http://mun.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vcq.havefunace.top


<!-- 参考信息 -->