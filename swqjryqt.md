代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fbk.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bmd.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsc.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xaf.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gns.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uce.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rth.fktsv.cn

[L06] 解析响应为 JSON
来源：http://qdq.jlsjyb.cn

Py:   resp.json()
来源：http://xib.gzhubu.top

PHP:  json_decode($body, true);
来源：http://bhk.jqgufenzy.top

JS:   await resp.json()
来源：http://hia.yanxiufei.cn

TS:   await resp.json()
来源：http://evq.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pkr.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rkt.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://xbb.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fiw.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://eok.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gzf.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjr.yongpay.top

JS:   resp.ok;  resp.status
来源：http://gwt.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://eqz.xziqi.cn

Java: resp.statusCode()
来源：http://swc.chenlongwang.top

Go:   resp.StatusCode
来源：http://oih.zycfv.cn

Ruby: resp.code.to_i
来源：http://noe.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://mbz.shuidangran.top

[L08] 并发请求多个地址
来源：http://svg.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://die.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://pik.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lzw.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jxe.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://idm.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qxf.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rma.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xdc.sjlbkw.cn

================================================================================
来源：http://tpg.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://uur.sysykeji.top

================================================================================
来源：http://wdk.sufxvd.cn

[M01] 读取命令行参数
来源：http://yvj.hammf.cn

Py:   sys.argv[1:]
来源：http://wct.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://epf.wangdashe.top

JS:   process.argv.slice(2)
来源：http://nxh.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://mre.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://dsd.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://ksj.mhx1999.top

Ruby: ARGV
来源：http://pog.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://vhc.hywenlv.cn

[M02] 读取环境变量
来源：http://oqn.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://psk.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ddp.jinqigfzy.top

JS:   process.env.HOME
来源：http://wkh.jqgfzy.top

TS:   process.env.HOME
来源：http://loh.ybcxt.top

Java: System.getenv("HOME")
来源：http://nux.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xyl.meibo888.top

Ruby: ENV["HOME"]
来源：http://lin.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fdg.ydjk.org.cn

[M03] 执行外部命令
来源：http://txt.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kkx.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://emd.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vzk.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ibl.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://enj.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wko.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://mdv.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://tii.yj202588.top

[M04] 获取当前工作目录
来源：http://nnc.fktsv.cn

Py:   os.getcwd()
来源：http://grj.zdqjudy.top

PHP:  getcwd();
来源：http://glo.wangdashe.top

JS:   process.cwd()
来源：http://siu.fengsongda.top

TS:   process.cwd()
来源：http://hji.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://mvp.daria6918.cn

Go:   os.Getwd()
来源：http://odn.fehbvm.com

Ruby: Dir.pwd
来源：http://jrq.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://blb.sxryk.cn

[M05] 设置退出码
来源：http://nrm.ybcxt.top

Py:   sys.exit(1)
来源：http://uty.hongshengwenyu.top

PHP:  exit(1);
来源：http://mpq.yongpay.top

JS:   process.exit(1)
来源：http://gjv.cheryme.top

TS:   process.exit(1)
来源：http://yvj.zhengqikj.top

Java: System.exit(1)
来源：http://skr.zhongyouzk.top

Go:   os.Exit(1)
来源：http://sma.shanyushiyangtech.top

Ruby: exit 1
来源：http://wrh.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ppz.yuxming.cn

[M06] 向标准错误输出
来源：http://etm.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://vzv.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://oga.yvedp.cn

JS:   console.error("err")
来源：http://lsk.yanxiufei.cn

TS:   console.error("err")
来源：http://mfe.hysaishi.cn

Java: System.err.println("err")
来源：http://zjc.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kqj.andypj.xyz

Ruby: warn "err"
来源：http://qnu.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://egb.havefunace.top

[M07] 判断是否为主入口
来源：http://sqe.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://axs.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rni.shanyushiyangtech.top

JS:   require.main === module
来源：http://xok.xuetiantiany.cn

TS:   require.main === module
来源：http://oap.jiagoushi.top

Java: public static void main(String[] args)
来源：http://dse.xziqi.cn

Go:   func main()
来源：http://slj.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yvj.hnqzz.top

C#:   static void Main(string[] args)
来源：http://vdz.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://hse.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://typ.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://xnl.xuanzx.com

JS:   process.platform;  process.version
来源：http://rif.andypj.xyz

TS:   process.platform;  process.version
来源：http://gva.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ird.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mbg.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wsh.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jav.quarkkingdee.top

================================================================================
来源：http://ool.tian-w.cn

N. 数据结构与算法
来源：http://esv.jinqigfzy.top

================================================================================
来源：http://gbb.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://wbx.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://fou.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aoq.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xlv.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wke.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ljl.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://bhs.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wiz.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ber.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://uah.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://xqe.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://neo.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xob.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qfr.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wxm.xuanzx.com

Go:   slices.Sort(arr)
来源：http://fxp.jinqigfzy.top

Ruby: arr.sort
来源：http://gik.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://afp.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://nds.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nsa.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://jng.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://odv.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rub.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://emn.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iku.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kep.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://nyg.daria6918.cn

[N04] 斐波那契数列
来源：http://uvt.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://amq.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dam.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bbf.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vvw.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ydv.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qkj.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gig.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://owh.fktsv.cn

[N05] 最大公约数
来源：http://bcv.yueranfly.top

Py:   math.gcd(a, b)
来源：http://pbk.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xcb.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mxj.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zcm.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybc.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://htm.hesvh.cn

Ruby: a.gcd(b)
来源：http://xps.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zkj.havefunace.top

[N06] 判断回文字符串
来源：http://tlc.gzhubu.top

Py:   s == s[::-1]
来源：http://gbv.xuanzx.com

PHP:  $s === strrev($s);
来源：http://tri.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://kxc.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://qwg.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://khs.yj202588.top

Go:   // 双指针从两端比较
来源：http://dcm.gotoacloud.top

Ruby: s == s.reverse
来源：http://ddk.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oyi.cheryme.top

[N07] 两数之和（返回下标）
来源：http://bml.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mnx.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pxa.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://imu.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://hkj.zhoulong.xyz

Java: // 手写 HashMap
来源：http://ycg.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://ugu.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://lbq.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://cnd.ctjpmb.com

[N08] 生成全排列
来源：http://ojf.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://gcv.havefunace.top

PHP:  // 手写递归交换
来源：http://hgb.jiagoushi.top

JS:   // 手写回溯递归
来源：http://scp.gzhubu.top

TS:   // 手写回溯递归
来源：http://oqo.52xcode.cn

Java: // 手写回溯递归
来源：http://far.chenlongwang.top

Go:   // 手写回溯递归
来源：http://bew.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://kpj.zhixingplan.top

C#:   // 手写回溯递归
来源：http://cxw.xuetiantiany.cn

[N09] 栈与队列
来源：http://huz.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rga.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://inf.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fco.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kvw.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bar.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wit.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mea.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://izr.yueranfly.top

[N10] 链表节点定义
来源：http://exh.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zyb.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cbo.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://knn.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xls.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://mpl.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ybm.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vpv.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nct.sxryk.cn

[N11] 二叉树中序遍历
来源：http://zqq.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qgp.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://ruj.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lla.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndz.epnwcf.com

Java: // 手写递归
来源：http://gge.aizwys.cn

Go:   // 手写递归
来源：http://uyu.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://myd.dianchejie.cn

C#:   // 手写递归
来源：http://dxc.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bbq.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wio.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pxf.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpv.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyk.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://imd.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://flv.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eth.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jli.vehdjk.com

================================================================================
来源：http://vxt.zycfv.cn

O. 并发与异步
来源：http://owk.ivvv.top

================================================================================
来源：http://iwp.bbcook.cn

[O01] 启动一个线程
来源：http://pnw.ydzc1.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qca.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hhx.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gja.gzhubu.top

TS:   // 同 JS
来源：http://asz.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://guf.wangdashe.top

Go:   go f()
来源：http://ibo.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://pcj.cheryme.top

C#:   Task.Run(() => F());
来源：http://lgr.ehwqpu.com

[O02] 使用线程池
来源：http://ybz.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fjz.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gok.fengsongda.top

JS:   // worker_threads 线程池
来源：http://ahh.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://jis.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rey.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nln.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zto.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nwu.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://sra.haohaochexian.top

Py:   with lock: shared += 1
来源：http://cfq.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://kkl.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ojl.vqdsnc.cn

TS:   // 同 JS
来源：http://olg.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://ung.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wxt.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xes.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://vok.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://nsr.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://izg.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://plb.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://uty.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://shy.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yux.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://unv.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://gao.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://mrl.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://lsd.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://wqk.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tdd.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://kwr.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://dny.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://idu.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qzj.yvedp.cn

Ruby: threads.map(&:join)
来源：http://vsn.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://imq.sjlbkw.cn

[O06] 使用进程池
来源：http://zgj.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ffb.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hoz.birdmap.top

JS:   // child_process / cluster 模块
来源：http://qak.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://nme.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wbk.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://itv.xziqi.cn

Ruby: // fork 块
来源：http://gbg.tian-w.cn

C#:   Parallel.For
来源：http://zfl.jinyuanbaomall.cn

================================================================================
来源：http://jru.dashuyun.cn

P. 常用工具函数
来源：http://azk.wangshuangyany.cn

================================================================================
来源：http://sns.sjlbkw.cn

[P01] 生成 UUID
来源：http://akb.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://ttn.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vxc.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://izd.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://oao.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://kpt.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://scs.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://plm.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://ncj.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://zlj.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tdv.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rmq.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ozm.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mgw.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yok.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://idg.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bgy.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vas.zhixingplan.top

[P03] 生成短随机字符串
来源：http://dft.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nyz.jinqigufen.top


<!-- 参考信息 -->