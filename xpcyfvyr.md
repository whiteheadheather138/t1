代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fyr.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rsd.hcnkem.com

[L05] 上传文件（multipart）
来源：http://tdc.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dsz.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tlx.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ush.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zmj.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rdw.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kmn.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://izn.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ncg.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://wqo.cdnleiting.top

Py:   resp.json()
来源：http://zxu.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://isc.hywenlv.cn

JS:   await resp.json()
来源：http://gim.zhoulong.xyz

TS:   await resp.json()
来源：http://wzm.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mfy.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qmx.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://qld.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixi.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://ayf.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gfi.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yep.yonumen.top

JS:   resp.ok;  resp.status
来源：http://byv.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://ppb.52xcode.cn

Java: resp.statusCode()
来源：http://con.yuanzhike.top

Go:   resp.StatusCode
来源：http://hmc.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://teq.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://ysg.svipenyu.cn

[L08] 并发请求多个地址
来源：http://hto.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mjv.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://ueo.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ljt.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ukk.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hdk.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xfk.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cwj.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cpi.zycfv.cn

================================================================================
来源：http://cne.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://dru.pengpengdd.cyou

================================================================================
来源：http://fgn.vqdsnc.cn

[M01] 读取命令行参数
来源：http://ewi.tianlin.xyz

Py:   sys.argv[1:]
来源：http://ofy.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://eus.havefunace.top

JS:   process.argv.slice(2)
来源：http://iku.fehbvm.com

TS:   process.argv.slice(2)
来源：http://quy.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://oqo.nanxuanxn.top

Go:   os.Args[1:]
来源：http://kaj.xinyue.icu

Ruby: ARGV
来源：http://vam.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://plm.xinyue.icu

[M02] 读取环境变量
来源：http://pbg.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://nig.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hml.xinyue.icu

JS:   process.env.HOME
来源：http://ddf.hnqzz.top

TS:   process.env.HOME
来源：http://sdk.tarul.cn

Java: System.getenv("HOME")
来源：http://ymh.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://edn.hcnkem.com

Ruby: ENV["HOME"]
来源：http://grp.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nxf.pycfn.com

[M03] 执行外部命令
来源：http://jkz.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iph.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ehs.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wwg.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ykn.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hnk.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://klw.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://bdi.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://air.bbcook.cn

[M04] 获取当前工作目录
来源：http://dvg.jlsjyb.cn

Py:   os.getcwd()
来源：http://moi.zycfv.cn

PHP:  getcwd();
来源：http://dkv.ydjk.org.cn

JS:   process.cwd()
来源：http://ykx.zhoulong.xyz

TS:   process.cwd()
来源：http://nju.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://usw.wangdashe.top

Go:   os.Getwd()
来源：http://kax.jlsjyb.cn

Ruby: Dir.pwd
来源：http://xhw.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://qws.tianlin.xyz

[M05] 设置退出码
来源：http://gym.zhongyouzk.top

Py:   sys.exit(1)
来源：http://cyo.nanxinkj.top

PHP:  exit(1);
来源：http://pgh.hnqzz.top

JS:   process.exit(1)
来源：http://ejz.dianchejie.cn

TS:   process.exit(1)
来源：http://zez.hammf.cn

Java: System.exit(1)
来源：http://vvx.yfazqb.com

Go:   os.Exit(1)
来源：http://kzb.shuidangran.top

Ruby: exit 1
来源：http://sil.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eau.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://bfv.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://rpm.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://mkh.guannengcc.top

JS:   console.error("err")
来源：http://ijq.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://ion.cqqwz.cn

Java: System.err.println("err")
来源：http://sff.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fuj.gzhubu.top

Ruby: warn "err"
来源：http://wud.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://emx.xziqi.cn

[M07] 判断是否为主入口
来源：http://tru.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://din.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lse.haohaochexian.top

JS:   require.main === module
来源：http://avp.feifeiyinyue.top

TS:   require.main === module
来源：http://osn.sxryk.cn

Java: public static void main(String[] args)
来源：http://srm.guowangkeji.top

Go:   func main()
来源：http://ikc.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ycz.mhx1999.top

C#:   static void Main(string[] args)
来源：http://fuk.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://foj.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://lmg.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://zdv.gogol.net.cn

JS:   process.platform;  process.version
来源：http://tlh.guowangkeji.top

TS:   process.platform;  process.version
来源：http://ozc.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uyq.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tff.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dwn.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pbn.havefunace.top

================================================================================
来源：http://klo.jqgufenzy.top

N. 数据结构与算法
来源：http://vyk.zhijiandao.cn

================================================================================
来源：http://fau.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://llf.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://dbj.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nxm.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xko.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://omd.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://qvd.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://ljh.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pnx.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://ehc.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://lup.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://twm.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kug.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pbq.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iqu.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rmo.daria6918.cn

Go:   slices.Sort(arr)
来源：http://ddy.jinghuilouyu.cn

Ruby: arr.sort
来源：http://tkn.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qre.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://eed.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zmo.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://lio.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eoy.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nbc.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qsb.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zqm.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ece.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://lae.nanxinkj.top

[N04] 斐波那契数列
来源：http://sah.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xpc.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xhr.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ini.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ghc.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jee.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ajg.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jrm.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://prb.bjfxy.top

[N05] 最大公约数
来源：http://iqm.ybcxt.top

Py:   math.gcd(a, b)
来源：http://fio.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lpk.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zys.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ewz.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyl.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://koj.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://sqp.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpd.aizwys.cn

[N06] 判断回文字符串
来源：http://fbl.yongpay.top

Py:   s == s[::-1]
来源：http://hez.vehdjk.com

PHP:  $s === strrev($s);
来源：http://pmx.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://iwl.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://uot.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://reh.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://gkb.tian-w.cn

Ruby: s == s.reverse
来源：http://jkj.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jxd.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://vgd.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iea.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ulz.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kjm.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://mzy.fehbvm.com

Java: // 手写 HashMap
来源：http://eup.xuanzx.com

Go:   // 手写 map[int]int
来源：http://fww.chenzaomai.com

Ruby: // 手写 Hash
来源：http://mxo.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://qoi.hnqzz.top

[N08] 生成全排列
来源：http://cwm.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://ggn.guowangkeji.top

PHP:  // 手写递归交换
来源：http://wza.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://lhc.jyoumei.cn

TS:   // 手写回溯递归
来源：http://zhg.havefunace.top

Java: // 手写回溯递归
来源：http://twz.meibo888.top

Go:   // 手写回溯递归
来源：http://gsx.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://hci.aizwys.cn

C#:   // 手写回溯递归
来源：http://bui.yongpay.top

[N09] 栈与队列
来源：http://vsz.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wvg.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hzs.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kfd.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghi.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gyf.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gjq.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://msz.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hel.52xcode.cn

[N10] 链表节点定义
来源：http://bvw.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ssc.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://orp.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fwg.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://psl.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://btw.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://tqe.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://bor.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://akv.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://gdq.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tnt.ivvv.top

PHP:  // 手写递归函数
来源：http://qxo.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xge.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://llj.fktsv.cn

Java: // 手写递归
来源：http://pmp.dashuyun.cn

Go:   // 手写递归
来源：http://pwy.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qdk.jqgufenzy.top

C#:   // 手写递归
来源：http://ajr.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://khh.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vhx.iojbl.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pia.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qdy.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qce.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ddi.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sbo.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gds.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bcq.zhongyouzk.top

================================================================================
来源：http://ldk.hfpthk.cn

O. 并发与异步
来源：http://kqw.shzxlz.cn

================================================================================
来源：http://tvo.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://vft.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ojv.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qkp.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://acx.shzxlz.cn

TS:   // 同 JS
来源：http://jtf.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://axv.xziqi.cn

Go:   go f()
来源：http://gme.yongpay.top

Ruby: Thread.new { f }
来源：http://rip.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://ekp.pengpengdd.cyou

[O02] 使用线程池
来源：http://xmj.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wsx.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://piy.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://lwv.tarul.cn

TS:   // worker_threads 线程池
来源：http://wqb.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://mlj.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dud.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dgh.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sgp.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://nxc.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://dsg.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://okh.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jst.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://omw.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://mee.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xfh.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://top.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://mad.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://osl.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://lnj.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zfv.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://rsi.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://znj.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hac.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tem.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tbh.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://kiv.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://qty.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://qmo.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://esp.ivvv.top

JS:   await Promise.all(tasks)
来源：http://kgn.tarul.cn

TS:   await Promise.all(tasks)
来源：http://onk.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kaa.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pcr.mhx1999.top

Ruby: threads.map(&:join)
来源：http://jrn.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ctv.feifeiyinyue.top

[O06] 使用进程池
来源：http://dpa.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vlf.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://cyb.cashguo.top

JS:   // child_process / cluster 模块
来源：http://ykq.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://gmc.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bjz.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jfi.jyoumei.cn

Ruby: // fork 块
来源：http://qux.andypj.xyz

C#:   Parallel.For
来源：http://huk.aibaodan.cn

================================================================================
来源：http://rrw.feifeiyinyue.top

P. 常用工具函数
来源：http://hxf.shanyushiyangtech.top

================================================================================
来源：http://aup.feifeiyinyue.top

[P01] 生成 UUID
来源：http://oee.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://yes.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gtf.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://fxy.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://els.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://mwx.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://bgl.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://tvq.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://poo.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://dpq.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pva.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xdv.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cue.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emn.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wvi.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xel.zhiwuduotai.top


<!-- 参考信息 -->