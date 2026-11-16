代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pgh.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://thu.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mtv.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vjy.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nmi.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sui.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yhv.fehbvm.com

[L06] 解析响应为 JSON
来源：http://vxh.zhengqikj.top

Py:   resp.json()
来源：http://oib.fehbvm.com

PHP:  json_decode($body, true);
来源：http://tjd.jinghuilouyu.cn

JS:   await resp.json()
来源：http://yeq.ybcxt.top

TS:   await resp.json()
来源：http://xmg.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nto.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qzx.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://xtl.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uzw.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://oti.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ddj.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://imc.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://zbm.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://gzb.nwbrower.top

Java: resp.statusCode()
来源：http://jtf.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://ome.yfazqb.com

Ruby: resp.code.to_i
来源：http://ohs.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://wee.yfazqb.com

[L08] 并发请求多个地址
来源：http://jhw.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://otv.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://yvq.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pbf.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bjk.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oru.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mxu.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wgf.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xoo.hongshengwenyu.top

================================================================================
来源：http://arp.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://sdo.zhengqikj.top

================================================================================
来源：http://flm.jlsjyb.cn

[M01] 读取命令行参数
来源：http://ujt.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://siw.xziqi.cn

PHP:  $argv;  $argc;
来源：http://crh.c1oappe.top

JS:   process.argv.slice(2)
来源：http://jve.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://itd.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://ayd.52xcode.cn

Go:   os.Args[1:]
来源：http://ncs.jinyuanbaomall.cn

Ruby: ARGV
来源：http://uby.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://pke.aibaodan.cn

[M02] 读取环境变量
来源：http://sbi.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://pgx.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blt.nanxinkj.top

JS:   process.env.HOME
来源：http://iye.yfazqb.com

TS:   process.env.HOME
来源：http://hjt.yj202588.top

Java: System.getenv("HOME")
来源：http://ebn.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tth.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://pro.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rgf.fktsv.cn

[M03] 执行外部命令
来源：http://luw.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zrw.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aey.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dss.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yzr.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cqk.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ihp.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yqu.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://qrz.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://jba.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://wwh.gotoacloud.top

PHP:  getcwd();
来源：http://fzj.chenzaomai.com

JS:   process.cwd()
来源：http://knw.iojbl.cn

TS:   process.cwd()
来源：http://cqh.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://jlp.zhoulong.xyz

Go:   os.Getwd()
来源：http://cet.wangdashe.top

Ruby: Dir.pwd
来源：http://amq.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://qrx.yuanzhike.top

[M05] 设置退出码
来源：http://jcl.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://ocq.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://dlv.yonumen.top

JS:   process.exit(1)
来源：http://wfs.daxiang520.top

TS:   process.exit(1)
来源：http://yie.vehdjk.com

Java: System.exit(1)
来源：http://puy.cucudq.cn

Go:   os.Exit(1)
来源：http://wqd.hongshengwenyu.top

Ruby: exit 1
来源：http://roj.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cth.nanxuanxn.top

[M06] 向标准错误输出
来源：http://tot.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://ohh.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gkr.nanxuanxn.top

JS:   console.error("err")
来源：http://aqn.chenzaomai.com

TS:   console.error("err")
来源：http://chu.svipenyu.cn

Java: System.err.println("err")
来源：http://oac.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://myi.jinghuilouyu.cn

Ruby: warn "err"
来源：http://kvn.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://eph.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://shj.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://izp.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qmy.sjlbkw.cn

JS:   require.main === module
来源：http://dua.52xcode.cn

TS:   require.main === module
来源：http://ite.jqgfzy.top

Java: public static void main(String[] args)
来源：http://jzt.aizwys.cn

Go:   func main()
来源：http://auz.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lql.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://bnt.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://itz.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://scs.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://zdi.pycfn.com

JS:   process.platform;  process.version
来源：http://ymj.xuanzx.com

TS:   process.platform;  process.version
来源：http://tth.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dbh.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rrq.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ayk.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://aiv.guowangkeji.top

================================================================================
来源：http://ihn.hysaishi.cn

N. 数据结构与算法
来源：http://vus.zhongyouzk.top

================================================================================
来源：http://vox.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://qjw.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://ddk.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lfi.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ljh.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://okq.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://cmg.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://pjf.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://xnd.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://dsj.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://jvn.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bjg.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ahv.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zio.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ijw.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fqg.fktsv.cn

Go:   slices.Sort(arr)
来源：http://ysr.fktsv.cn

Ruby: arr.sort
来源：http://qpy.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ykq.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://nwz.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qfa.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://qgw.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ypq.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpd.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://asd.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gta.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://omk.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://dxa.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://nlr.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hmp.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jqo.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lku.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npj.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bxw.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lah.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sak.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oey.316326.xyz

[N05] 最大公约数
来源：http://enh.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://udo.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://moz.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmm.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfl.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://atc.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://heb.hammf.cn

Ruby: a.gcd(b)
来源：http://nxl.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gnb.zycfv.cn

[N06] 判断回文字符串
来源：http://raq.yangfankeji.com

Py:   s == s[::-1]
来源：http://nbr.epnwcf.com

PHP:  $s === strrev($s);
来源：http://gse.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://mzu.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://odv.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lon.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://wxd.smart0.xyz

Ruby: s == s.reverse
来源：http://dyo.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://une.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://ijj.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cnh.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ipy.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wcb.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://ofv.nanxuanxn.top

Java: // 手写 HashMap
来源：http://ulk.redwolf501.top

Go:   // 手写 map[int]int
来源：http://aqs.cashguo.top

Ruby: // 手写 Hash
来源：http://tin.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kdt.tarul.cn

[N08] 生成全排列
来源：http://hpf.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://mbr.zhixingplan.top

PHP:  // 手写递归交换
来源：http://ugg.mhx1999.top

JS:   // 手写回溯递归
来源：http://wwb.redwolf501.top

TS:   // 手写回溯递归
来源：http://ihm.zhijiandao.cn

Java: // 手写回溯递归
来源：http://qeb.tianlin.xyz

Go:   // 手写回溯递归
来源：http://poo.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://wbh.xylfe.cn

C#:   // 手写回溯递归
来源：http://xwv.yongpay.top

[N09] 栈与队列
来源：http://gyq.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://csm.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znn.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bxg.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zxy.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jgj.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jum.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://khw.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ygg.yfazqb.com

[N10] 链表节点定义
来源：http://taw.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dwn.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zcp.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ady.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rib.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://ldp.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://ggv.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nix.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dqz.tarul.cn

[N11] 二叉树中序遍历
来源：http://jir.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://auz.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://pjj.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cne.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fex.yueranfly.top

Java: // 手写递归
来源：http://xlp.yj202588.top

Go:   // 手写递归
来源：http://ycy.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rgp.jqgfzy.top

C#:   // 手写递归
来源：http://hzy.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://khl.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://upg.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ehh.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eqp.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzj.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://abc.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lbm.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yop.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nwe.hywenlv.cn

================================================================================
来源：http://zmt.yuxming.cn

O. 并发与异步
来源：http://wyb.zhengqikj.top

================================================================================
来源：http://qrv.xinyue.icu

[O01] 启动一个线程
来源：http://yrq.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://abd.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jvj.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zdr.zycfv.cn

TS:   // 同 JS
来源：http://hem.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://erf.vqdsnc.cn

Go:   go f()
来源：http://tvy.tian-w.cn

Ruby: Thread.new { f }
来源：http://vun.sxryk.cn

C#:   Task.Run(() => F());
来源：http://pjb.sysykeji.top

[O02] 使用线程池
来源：http://rpi.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ycf.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lyv.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://ata.ybcxt.top

TS:   // worker_threads 线程池
来源：http://szl.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://rrl.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gla.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://euq.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fan.birdmap.top

[O03] 加锁保护共享数据
来源：http://ova.zhixingplan.top

Py:   with lock: shared += 1
来源：http://qct.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://rhw.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://edj.hcnkem.com

TS:   // 同 JS
来源：http://nci.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://zwh.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xdj.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aeg.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://ekg.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://zxk.hammf.cn

Py:   async def f():⏎    await g()
来源：http://xvc.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kkf.wangdashe.top

JS:   async function f() { await g(); }
来源：http://szp.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://krt.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lkx.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://two.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rez.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://auk.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://ppo.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://jid.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ytw.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://ndo.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://mxp.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jvx.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lht.wangdashe.top

Ruby: threads.map(&:join)
来源：http://awz.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://brd.birdmap.top

[O06] 使用进程池
来源：http://mak.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ypt.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lmw.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://olw.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://uyk.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://viq.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cwm.cdnleiting.top

Ruby: // fork 块
来源：http://zct.daxiang520.top

C#:   Parallel.For
来源：http://xfl.jlsjyb.cn

================================================================================
来源：http://seo.316326.xyz

P. 常用工具函数
来源：http://eas.ydjk.org.cn

================================================================================
来源：http://cqm.pycfn.com

[P01] 生成 UUID
来源：http://swg.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://zsl.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mkp.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://vys.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://kdi.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://ojz.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://ylr.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://tad.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://axg.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://aqh.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dts.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sbu.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umy.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vym.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://voe.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://neo.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gih.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://awk.aibaodan.cn

[P03] 生成短随机字符串
来源：http://wkp.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slm.sweek.top


<!-- 参考信息 -->