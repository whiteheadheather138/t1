代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ymy.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hds.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hym.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nzp.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rrm.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ojp.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aqc.hesvh.cn

[L06] 解析响应为 JSON
来源：http://dul.gogol.net.cn

Py:   resp.json()
来源：http://qzt.hnqzz.top

PHP:  json_decode($body, true);
来源：http://dba.zdbjq.cn

JS:   await resp.json()
来源：http://cgf.jqgfzy.top

TS:   await resp.json()
来源：http://qnz.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://isu.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wgq.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://jnz.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbu.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://dpl.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iot.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://avr.yj202588.top

JS:   resp.ok;  resp.status
来源：http://hws.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://zsl.fktsv.cn

Java: resp.statusCode()
来源：http://fgj.bbcook.cn

Go:   resp.StatusCode
来源：http://ziy.bjfxy.top

Ruby: resp.code.to_i
来源：http://glz.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://hog.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://zbw.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rxh.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://yiy.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nrt.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vju.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mba.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dtk.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://peg.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://axn.shangyingyoupin.top

================================================================================
来源：http://qtp.sweek.top

M. 命令行 / 进程 / 环境
来源：http://dxq.ppjwa.cn

================================================================================
来源：http://lkv.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://qfk.yueranfly.top

Py:   sys.argv[1:]
来源：http://zmq.hnqzz.top

PHP:  $argv;  $argc;
来源：http://oxk.daxiang520.top

JS:   process.argv.slice(2)
来源：http://jfx.pycfn.com

TS:   process.argv.slice(2)
来源：http://mra.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://yva.epnwcf.com

Go:   os.Args[1:]
来源：http://urc.hcnkem.com

Ruby: ARGV
来源：http://bqn.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://rcu.nanxuanxn.top

[M02] 读取环境变量
来源：http://xsw.hammf.cn

Py:   os.environ.get("HOME")
来源：http://lul.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rzp.daria6918.cn

JS:   process.env.HOME
来源：http://jvf.nanxinkj.top

TS:   process.env.HOME
来源：http://ton.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://wwi.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yey.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://lsx.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wzi.cdnleiting.top

[M03] 执行外部命令
来源：http://phj.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://stj.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://geq.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qso.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://doi.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ntw.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xzy.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://pon.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://xxc.dashuyun.cn

[M04] 获取当前工作目录
来源：http://etp.hfpthk.cn

Py:   os.getcwd()
来源：http://lxq.dianchejie.cn

PHP:  getcwd();
来源：http://zns.jqgfzy.top

JS:   process.cwd()
来源：http://sin.cucudq.cn

TS:   process.cwd()
来源：http://lgg.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://uvf.jinqigufen.top

Go:   os.Getwd()
来源：http://xuw.zdqjudy.top

Ruby: Dir.pwd
来源：http://ljs.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://fcz.shzxlz.cn

[M05] 设置退出码
来源：http://wmh.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://kyk.cdnleiting.top

PHP:  exit(1);
来源：http://okx.jinqigufen.top

JS:   process.exit(1)
来源：http://uoz.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://obd.hfpthk.cn

Java: System.exit(1)
来源：http://gyg.mhx1999.top

Go:   os.Exit(1)
来源：http://mgm.jyoumei.cn

Ruby: exit 1
来源：http://moy.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sxn.yj202588.top

[M06] 向标准错误输出
来源：http://nkp.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://hos.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://blv.kuanghao11.cn

JS:   console.error("err")
来源：http://wsu.yueranfly.top

TS:   console.error("err")
来源：http://nqr.nanxinkj.top

Java: System.err.println("err")
来源：http://qoe.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rae.hnqzz.top

Ruby: warn "err"
来源：http://clx.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://knf.yj20258.top

[M07] 判断是否为主入口
来源：http://klu.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://zwq.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fea.sxryk.cn

JS:   require.main === module
来源：http://sqn.fktsv.cn

TS:   require.main === module
来源：http://wss.ehwqpu.com

Java: public static void main(String[] args)
来源：http://dhj.jqgufenzy.top

Go:   func main()
来源：http://ckt.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ryz.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://uzg.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://ime.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://myn.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://uiz.dianchejie.cn

JS:   process.platform;  process.version
来源：http://mtn.dashuyun.cn

TS:   process.platform;  process.version
来源：http://ghd.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lka.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pmi.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nqj.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dkp.epnwcf.com

================================================================================
来源：http://aqi.ivvv.top

N. 数据结构与算法
来源：http://cyl.zdqjudy.top

================================================================================
来源：http://ydz.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://eur.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://hzx.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://way.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://unp.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fcy.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://zxe.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://hxc.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bcj.quarkkingdee.top

C#:   Array.BinarySearch(arr, x)
来源：http://lfa.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://dmy.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://gkr.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jqu.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pme.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ooz.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qff.316326.xyz

Go:   slices.Sort(arr)
来源：http://oaf.hcnkem.com

Ruby: arr.sort
来源：http://ybx.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wvw.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://nrs.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oxf.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://hkf.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yyj.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zln.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zhf.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yit.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://naj.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://obz.zhengqikj.top

[N04] 斐波那契数列
来源：http://idd.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gmq.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://suo.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vxl.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wpy.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fts.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ala.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://piq.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aeh.jianghu66.top

[N05] 最大公约数
来源：http://bzy.xinyue.icu

Py:   math.gcd(a, b)
来源：http://mgn.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kqe.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iep.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jpr.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gwg.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tqv.vehdjk.com

Ruby: a.gcd(b)
来源：http://hbw.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ufi.meibo888.top

[N06] 判断回文字符串
来源：http://qkm.cheryme.top

Py:   s == s[::-1]
来源：http://nec.bbcook.cn

PHP:  $s === strrev($s);
来源：http://ops.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://ejh.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://tyo.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xaw.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://zeg.jianghu66.top

Ruby: s == s.reverse
来源：http://cpa.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rlr.cheryme.top

[N07] 两数之和（返回下标）
来源：http://kxw.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wzr.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wsa.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ull.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://mmz.sweek.top

Java: // 手写 HashMap
来源：http://ffz.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://dii.xinyue.icu

Ruby: // 手写 Hash
来源：http://cgd.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://cor.quarkkingdee.top

[N08] 生成全排列
来源：http://eix.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://qhh.yueranfly.top

PHP:  // 手写递归交换
来源：http://qxv.vehdjk.com

JS:   // 手写回溯递归
来源：http://fxo.fktsv.cn

TS:   // 手写回溯递归
来源：http://jws.jyoumei.cn

Java: // 手写回溯递归
来源：http://qqu.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://xlb.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://qiv.hammf.cn

C#:   // 手写回溯递归
来源：http://cwh.wangshuangyany.cn

[N09] 栈与队列
来源：http://luj.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://apo.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sph.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ybw.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uuc.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xky.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kya.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uig.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oek.jyoumei.cn

[N10] 链表节点定义
来源：http://hhw.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gbh.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gwx.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dix.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bpz.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://fhz.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://olf.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xfl.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://euf.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://ebt.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ily.xuanzx.com

PHP:  // 手写递归函数
来源：http://qbz.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gyn.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qnq.gzhubu.top

Java: // 手写递归
来源：http://yvr.jlsjyb.cn

Go:   // 手写递归
来源：http://wls.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gjv.daria6918.cn

C#:   // 手写递归
来源：http://mpf.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nwt.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xjq.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jnv.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rnz.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lxu.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rzq.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cid.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mgm.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jhr.fengsongda.top

================================================================================
来源：http://wgg.tarul.cn

O. 并发与异步
来源：http://xwm.ywan-chungtsiang.top

================================================================================
来源：http://luc.xziqi.cn

[O01] 启动一个线程
来源：http://otx.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gxw.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lyf.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mpx.nanxuanxn.top

TS:   // 同 JS
来源：http://seu.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://gpm.fktsv.cn

Go:   go f()
来源：http://ajf.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://nyo.yfazqb.com

C#:   Task.Run(() => F());
来源：http://sgg.wangshuangyany.cn

[O02] 使用线程池
来源：http://btc.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bbx.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wed.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://gra.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://mes.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tdi.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://itg.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lhc.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cdt.tian-w.cn

[O03] 加锁保护共享数据
来源：http://yew.yuxming.cn

Py:   with lock: shared += 1
来源：http://qbs.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://omh.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fco.dashuyun.cn

TS:   // 同 JS
来源：http://kiw.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://khi.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jvv.hysaishi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bsd.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://agd.yfazqb.com

[O04] 定义异步函数并等待
来源：http://tql.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://yqm.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yeb.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://yqv.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yzm.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tdk.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yqs.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://nhk.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://qaq.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://mus.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://vmp.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gto.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://swo.yj202588.top

TS:   await Promise.all(tasks)
来源：http://bdx.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://caq.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ghz.xziqi.cn

Ruby: threads.map(&:join)
来源：http://kzz.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nul.mhx1999.top

[O06] 使用进程池
来源：http://kkz.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://woi.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://web.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://jwh.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://egi.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://srb.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://miq.yongpay.top

Ruby: // fork 块
来源：http://dzs.zhijiandao.cn

C#:   Parallel.For
来源：http://hcf.zhixingplan.top

================================================================================
来源：http://isq.yvedp.cn

P. 常用工具函数
来源：http://zkk.yvedp.cn

================================================================================
来源：http://nyg.yfazqb.com

[P01] 生成 UUID
来源：http://uwy.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://hms.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://efu.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://yje.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://rtb.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://qmt.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://tkt.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://aax.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://ljw.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://tiu.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://obg.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ydl.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rmh.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vhy.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hlg.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zsm.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://spt.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cmr.hammf.cn

[P03] 生成短随机字符串
来源：http://kmj.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slv.quarkkingdee.top


<!-- 参考信息 -->