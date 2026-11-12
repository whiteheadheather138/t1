代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://khh.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lzq.tian-w.cn

[L05] 上传文件（multipart）
来源：http://irq.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tev.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sys.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xag.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yeq.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kiq.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://joy.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fvw.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xok.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://aol.zdqjudy.top

Py:   resp.json()
来源：http://nja.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://hcw.c1oappe.top

JS:   await resp.json()
来源：http://nvo.hesvh.cn

TS:   await resp.json()
来源：http://ifu.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gnd.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://skj.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://aca.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bph.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://jbl.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ups.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sbi.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://cpy.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://dsw.sjlbkw.cn

Java: resp.statusCode()
来源：http://vyn.mhx1999.top

Go:   resp.StatusCode
来源：http://hih.sweek.top

Ruby: resp.code.to_i
来源：http://pxh.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://oys.aizwys.cn

[L08] 并发请求多个地址
来源：http://oac.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ehm.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://ndz.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tbi.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ryi.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://osf.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ivm.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uhg.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dro.cashguo.top

================================================================================
来源：http://ktg.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://mzz.yongpay.top

================================================================================
来源：http://nqa.sxryk.cn

[M01] 读取命令行参数
来源：http://oas.daria6918.cn

Py:   sys.argv[1:]
来源：http://chz.tanke756.top

PHP:  $argv;  $argc;
来源：http://toh.shuidangran.top

JS:   process.argv.slice(2)
来源：http://ubc.fengsongda.top

TS:   process.argv.slice(2)
来源：http://wuf.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://mhc.jinqigufen.top

Go:   os.Args[1:]
来源：http://mpi.sufxvd.cn

Ruby: ARGV
来源：http://bqi.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://qjn.yanxiufei.cn

[M02] 读取环境变量
来源：http://qqx.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://lwf.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zdc.shzxlz.cn

JS:   process.env.HOME
来源：http://ndt.vehdjk.com

TS:   process.env.HOME
来源：http://suj.hesvh.cn

Java: System.getenv("HOME")
来源：http://unq.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://haz.bjfxy.top

Ruby: ENV["HOME"]
来源：http://uvo.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mhs.jqgfzy.top

[M03] 执行外部命令
来源：http://xvh.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://afm.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://irx.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mva.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gxj.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hfl.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://utn.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://usk.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://cln.zhengqikj.top

[M04] 获取当前工作目录
来源：http://mso.jqgfzy.top

Py:   os.getcwd()
来源：http://oae.ctjpmb.com

PHP:  getcwd();
来源：http://qgy.meibo888.top

JS:   process.cwd()
来源：http://mnq.fanxiaobao.xyz

TS:   process.cwd()
来源：http://qyi.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://gxt.cheryme.top

Go:   os.Getwd()
来源：http://dnv.zdqjudy.top

Ruby: Dir.pwd
来源：http://pgp.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://khn.hysaishi.cn

[M05] 设置退出码
来源：http://pni.yonumen.top

Py:   sys.exit(1)
来源：http://azt.sxryk.cn

PHP:  exit(1);
来源：http://lfx.shangyingyoupin.top

JS:   process.exit(1)
来源：http://xve.c1oappe.top

TS:   process.exit(1)
来源：http://zjy.zycfv.cn

Java: System.exit(1)
来源：http://put.sufxvd.cn

Go:   os.Exit(1)
来源：http://aky.hfpthk.cn

Ruby: exit 1
来源：http://ulq.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jpj.zhoulong.xyz

[M06] 向标准错误输出
来源：http://ugy.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://elu.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rym.fzhhl.top

JS:   console.error("err")
来源：http://hjd.jqgfzy.top

TS:   console.error("err")
来源：http://fbb.uphjek.com

Java: System.err.println("err")
来源：http://drr.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wwz.havefunace.top

Ruby: warn "err"
来源：http://uvs.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://jxe.iojbl.cn

[M07] 判断是否为主入口
来源：http://gpw.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://gry.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pel.nanxinkj.top

JS:   require.main === module
来源：http://erk.gzhubu.top

TS:   require.main === module
来源：http://nxa.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://oum.redwolf501.top

Go:   func main()
来源：http://hxy.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fgi.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://yqv.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://veu.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://ker.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://iwt.zhixingplan.top

JS:   process.platform;  process.version
来源：http://aod.xuanzx.com

TS:   process.platform;  process.version
来源：http://lkw.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://afj.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zac.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://suc.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gsx.zhijiandao.cn

================================================================================
来源：http://yeq.bbcook.cn

N. 数据结构与算法
来源：http://gsj.pycfn.com

================================================================================
来源：http://stn.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://tpa.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yfo.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rxh.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gwq.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tcd.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://sjz.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://qeg.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://nww.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pkb.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://ffo.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://iuv.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tvr.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jpr.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zyw.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cyz.xinyue.icu

Go:   slices.Sort(arr)
来源：http://tto.hcnkem.com

Ruby: arr.sort
来源：http://jxh.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vtg.tarul.cn

[N03] 快速排序（分治示例）
来源：http://zax.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ptl.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://ptq.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ziu.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbm.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bkn.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cjv.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qjf.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zlw.yuxming.cn

[N04] 斐波那契数列
来源：http://whs.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rrt.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sgj.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tzb.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ouv.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xza.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jhs.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ekk.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xsr.gogol.net.cn

[N05] 最大公约数
来源：http://ktm.gzhubu.top

Py:   math.gcd(a, b)
来源：http://njo.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cml.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rme.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://slf.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hvv.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hof.hcnkem.com

Ruby: a.gcd(b)
来源：http://cge.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xvk.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://kku.ybcxt.top

Py:   s == s[::-1]
来源：http://eoh.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://fil.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://rnm.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://gzq.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fjb.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://lsj.cucudq.cn

Ruby: s == s.reverse
来源：http://xnc.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://cuo.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://jbp.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gau.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yca.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qpe.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://vce.nanxuanxn.top

Java: // 手写 HashMap
来源：http://lrc.c1oappe.top

Go:   // 手写 map[int]int
来源：http://weh.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://jfu.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://lpi.yfazqb.com

[N08] 生成全排列
来源：http://nqc.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://jkr.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://yjt.jqgfzy.top

JS:   // 手写回溯递归
来源：http://djf.fehbvm.com

TS:   // 手写回溯递归
来源：http://qel.gzhubu.top

Java: // 手写回溯递归
来源：http://nre.316326.xyz

Go:   // 手写回溯递归
来源：http://omp.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://jex.ivvv.top

C#:   // 手写回溯递归
来源：http://zla.tarul.cn

[N09] 栈与队列
来源：http://zhy.jyoumei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rov.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tdy.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sln.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lyx.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gzv.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tjx.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nxn.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fgm.tian-w.cn

[N10] 链表节点定义
来源：http://jwr.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qvx.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tkn.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xup.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tcr.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://wmg.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xqb.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://avx.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mjl.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://jdn.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://njd.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://gag.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwp.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nuu.mhx1999.top

Java: // 手写递归
来源：http://znr.c1oappe.top

Go:   // 手写递归
来源：http://ctg.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fvb.redwolf501.top

C#:   // 手写递归
来源：http://ovk.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yul.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wae.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qsx.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xqb.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mmb.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dvp.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bmu.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zih.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://khm.zhaomingkeji.xyz

================================================================================
来源：http://htr.jqgufenzy.top

O. 并发与异步
来源：http://pym.jinqigufen.top

================================================================================
来源：http://hak.yongpay.top

[O01] 启动一个线程
来源：http://piv.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hjd.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hpg.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pni.xinyue.icu

TS:   // 同 JS
来源：http://lxu.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://bhz.nanxuanxn.top

Go:   go f()
来源：http://xwq.birdmap.top

Ruby: Thread.new { f }
来源：http://vym.pycfn.com

C#:   Task.Run(() => F());
来源：http://hve.cqqwz.cn

[O02] 使用线程池
来源：http://mtc.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mio.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dpy.fktsv.cn

JS:   // worker_threads 线程池
来源：http://qyo.tian-w.cn

TS:   // worker_threads 线程池
来源：http://qyv.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://dxt.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xzl.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://onb.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bpf.tian-w.cn

[O03] 加锁保护共享数据
来源：http://zkn.tanke756.top

Py:   with lock: shared += 1
来源：http://obu.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://gpd.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sjm.yangfankeji.com

TS:   // 同 JS
来源：http://gjl.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://nma.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fkp.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vso.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://bpo.vehdjk.com

[O04] 定义异步函数并等待
来源：http://xea.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://xxm.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://imr.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://jza.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zxz.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kgm.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://prf.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rns.yj20258.top

C#:   async Task F() { await G(); }
来源：http://kmm.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://zch.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://jrl.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ueh.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://vee.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://pud.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://erh.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://htk.yongpay.top

Ruby: threads.map(&:join)
来源：http://wsh.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fbe.nwbrower.top

[O06] 使用进程池
来源：http://lyn.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eay.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dlu.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://kyq.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://zbn.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zwc.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dfh.jyoumei.cn

Ruby: // fork 块
来源：http://pup.meibo888.top

C#:   Parallel.For
来源：http://wjc.yj202588.top

================================================================================
来源：http://hnb.ehwqpu.com

P. 常用工具函数
来源：http://ivp.zhiwuduotai.top

================================================================================
来源：http://ymx.xuetiantiany.cn

[P01] 生成 UUID
来源：http://crw.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://jmw.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tiz.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://zlv.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://ezu.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://kmg.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://tpg.meibo888.top

Ruby: SecureRandom.uuid
来源：http://qop.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://sta.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://uda.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jpc.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://xdr.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gyt.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xbf.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yqd.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zcr.yuxming.cn


<!-- 参考信息 -->