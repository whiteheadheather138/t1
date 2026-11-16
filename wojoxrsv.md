代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kcn.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lkz.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://bgg.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cns.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ehg.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kvp.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rki.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gdq.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rva.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eho.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jti.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://kww.sufxvd.cn

Py:   resp.json()
来源：http://xtl.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://tic.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://drn.sysykeji.top

TS:   await resp.json()
来源：http://mdo.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lmy.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lvt.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://npe.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bmf.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://azr.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jda.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uql.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://qfy.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://fne.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://ddl.hysaishi.cn

Go:   resp.StatusCode
来源：http://sfc.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://fef.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://lap.iojbl.cn

[L08] 并发请求多个地址
来源：http://uwf.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://knb.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://qxr.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swp.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vlb.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwl.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fyf.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xpk.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sek.ywan-chungtsiang.top

================================================================================
来源：http://mlw.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://djc.vqdsnc.cn

================================================================================
来源：http://bbb.shzxlz.cn

[M01] 读取命令行参数
来源：http://lov.yongpay.top

Py:   sys.argv[1:]
来源：http://pjd.redwolf501.top

PHP:  $argv;  $argc;
来源：http://plj.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://sbo.vehdjk.com

TS:   process.argv.slice(2)
来源：http://zqc.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://moo.tian-w.cn

Go:   os.Args[1:]
来源：http://dqh.dashuyun.cn

Ruby: ARGV
来源：http://qce.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://hbd.zhiwuduotai.top

[M02] 读取环境变量
来源：http://lfd.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://odo.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ekw.xuetiantiany.cn

JS:   process.env.HOME
来源：http://ylw.jinqigfzy.top

TS:   process.env.HOME
来源：http://bse.epnwcf.com

Java: System.getenv("HOME")
来源：http://nkb.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://epl.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://izz.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lkq.sysykeji.top

[M03] 执行外部命令
来源：http://egs.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://acx.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kdx.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aoj.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mmq.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fix.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ija.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://egn.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://pjq.bjfxy.top

[M04] 获取当前工作目录
来源：http://efv.yvedp.cn

Py:   os.getcwd()
来源：http://nml.yangfankeji.com

PHP:  getcwd();
来源：http://tmj.cheryme.top

JS:   process.cwd()
来源：http://zeh.tanke756.top

TS:   process.cwd()
来源：http://qha.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://elw.pengpengdd.cyou

Go:   os.Getwd()
来源：http://gpg.birdmap.top

Ruby: Dir.pwd
来源：http://msr.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ppv.guannengcc.top

[M05] 设置退出码
来源：http://bbp.jinqigfzy.top

Py:   sys.exit(1)
来源：http://csa.zhixingplan.top

PHP:  exit(1);
来源：http://tvd.hfpthk.cn

JS:   process.exit(1)
来源：http://ptu.ydjk.org.cn

TS:   process.exit(1)
来源：http://mor.jqgufenzy.top

Java: System.exit(1)
来源：http://kau.nanxinkj.top

Go:   os.Exit(1)
来源：http://mku.shuidangran.top

Ruby: exit 1
来源：http://cil.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ccu.sweek.top

[M06] 向标准错误输出
来源：http://hhv.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://mmb.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xcz.ctjpmb.com

JS:   console.error("err")
来源：http://pil.shzxlz.cn

TS:   console.error("err")
来源：http://hgn.redwolf501.top

Java: System.err.println("err")
来源：http://alu.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osh.hongshengwenyu.top

Ruby: warn "err"
来源：http://tth.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://pjt.cqqwz.cn

[M07] 判断是否为主入口
来源：http://ivg.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://otj.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ijh.ivvv.top

JS:   require.main === module
来源：http://pev.redwolf501.top

TS:   require.main === module
来源：http://phd.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://oir.jiagoushi.top

Go:   func main()
来源：http://fap.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sbq.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://tgv.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://mku.hcnkem.com

Py:   platform.system();  platform.python_version()
来源：http://ztc.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://qxf.pycfn.com

JS:   process.platform;  process.version
来源：http://lfl.meibo888.top

TS:   process.platform;  process.version
来源：http://jjj.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://glx.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rmb.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tgs.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nln.sufxvd.cn

================================================================================
来源：http://lbh.hnqzz.top

N. 数据结构与算法
来源：http://oay.yj20258888.top

================================================================================
来源：http://lzf.316326.xyz

[N01] 二分查找（有序数组）
来源：http://lza.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://jzm.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aym.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kll.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://elr.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nri.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://vdk.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://age.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://ycy.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://pcn.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://mco.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lob.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zpg.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fbs.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qbv.xinyue.icu

Go:   slices.Sort(arr)
来源：http://fjl.yangfankeji.com

Ruby: arr.sort
来源：http://vml.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uiu.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://uyl.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uaw.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://gvx.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bxf.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rnc.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ppl.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://izp.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://izh.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://zyg.xylfe.cn

[N04] 斐波那契数列
来源：http://bbl.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fra.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hem.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ddf.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ziw.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yfq.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cck.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tnt.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://enh.fanxiaobao.xyz

[N05] 最大公约数
来源：http://zhq.yj202588.top

Py:   math.gcd(a, b)
来源：http://jww.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://her.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ufw.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ilw.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://krh.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nbo.jianghu66.top

Ruby: a.gcd(b)
来源：http://udc.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ege.cdnleiting.top

[N06] 判断回文字符串
来源：http://fww.yvedp.cn

Py:   s == s[::-1]
来源：http://ydu.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://lto.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://drv.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://gnh.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bcf.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://qpf.0kj1m.cn

Ruby: s == s.reverse
来源：http://vqw.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://upn.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://who.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pno.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgs.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dau.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://xwn.jinqigufen.top

Java: // 手写 HashMap
来源：http://eiy.316326.xyz

Go:   // 手写 map[int]int
来源：http://oab.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://fio.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://msa.jqgufenzy.top

[N08] 生成全排列
来源：http://zux.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://lms.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://fqc.sxryk.cn

JS:   // 手写回溯递归
来源：http://axr.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://foc.ydzc1.top

Java: // 手写回溯递归
来源：http://jsl.52xcode.cn

Go:   // 手写回溯递归
来源：http://ivo.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://glc.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://ubi.gotoacloud.top

[N09] 栈与队列
来源：http://ldv.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jwi.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ulw.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tyh.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ymh.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wda.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://izq.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lyu.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lup.iojbl.cn

[N10] 链表节点定义
来源：http://xbs.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dci.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aaz.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iqn.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bbe.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://zde.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://ioy.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ncu.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://psx.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://tox.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rcs.zhengqikj.top

PHP:  // 手写递归函数
来源：http://keu.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ygx.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpx.guannengcc.top

Java: // 手写递归
来源：http://jvn.hongshengwenyu.top

Go:   // 手写递归
来源：http://wwz.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wyh.zhiwuduotai.top

C#:   // 手写递归
来源：http://gae.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jit.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ljp.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qjz.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwc.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rqy.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mbd.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pcm.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://orj.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lkq.guannengcc.top

================================================================================
来源：http://kcb.zdbjq.cn

O. 并发与异步
来源：http://pbq.gaohongyu789.top

================================================================================
来源：http://qln.yangfankeji.com

[O01] 启动一个线程
来源：http://yia.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pdj.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kyx.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tdh.guowangkeji.top

TS:   // 同 JS
来源：http://lem.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://kpu.svipenyu.cn

Go:   go f()
来源：http://nyi.jinqigufen.top

Ruby: Thread.new { f }
来源：http://hqt.daxiang520.top

C#:   Task.Run(() => F());
来源：http://lij.hfpthk.cn

[O02] 使用线程池
来源：http://xnw.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lvj.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://esm.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://rda.ybcxt.top

TS:   // worker_threads 线程池
来源：http://knq.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://qqh.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vma.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hgw.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ttf.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://kvm.0kj1m.cn

Py:   with lock: shared += 1
来源：http://ygi.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://sui.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ldp.daxiang520.top

TS:   // 同 JS
来源：http://uix.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://yux.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dwi.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mvo.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://jjb.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://xiy.yonumen.top

Py:   async def f():⏎    await g()
来源：http://fqk.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tix.yj20258888.top

JS:   async function f() { await g(); }
来源：http://nqi.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://srb.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iaw.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://grb.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tag.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://bgd.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://imr.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://jtk.xinyue.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sza.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://pdg.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://bzl.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pdz.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cgz.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://uuh.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ren.nanxinkj.top

[O06] 使用进程池
来源：http://dwv.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gnc.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jem.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://xms.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://uxe.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cro.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nbp.iojbl.cn

Ruby: // fork 块
来源：http://kpz.zhongyouzk.top

C#:   Parallel.For
来源：http://gxr.hfpthk.cn

================================================================================
来源：http://und.sufxvd.cn

P. 常用工具函数
来源：http://ivn.tian-w.cn

================================================================================
来源：http://zrk.xinyue.icu

[P01] 生成 UUID
来源：http://kvt.havefunace.top

Py:   str(uuid.uuid4())
来源：http://uay.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bii.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://oqt.vehdjk.com

TS:   crypto.randomUUID()
来源：http://rmu.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://rgl.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://mkz.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://nbf.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://rbz.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://awe.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qqf.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qam.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cro.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mxi.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kwe.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kfh.pengpengdd.cyou


<!-- 参考信息 -->