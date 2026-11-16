代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cqv.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lwt.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://vqd.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ifm.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://opy.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dlc.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hrc.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jyh.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://krc.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uwr.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpr.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://ulg.ybcxt.top

Py:   resp.json()
来源：http://que.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://kys.cashguo.top

JS:   await resp.json()
来源：http://xok.hnqzz.top

TS:   await resp.json()
来源：http://ldv.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cmo.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lrg.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://kqe.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gul.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://cht.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tly.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ulx.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://clr.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://vet.zhengqikj.top

Java: resp.statusCode()
来源：http://kla.chenzaomai.com

Go:   resp.StatusCode
来源：http://use.tianlin.xyz

Ruby: resp.code.to_i
来源：http://jyi.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://ioy.dianchejie.cn

[L08] 并发请求多个地址
来源：http://gkx.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lbb.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://uqy.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wmr.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mlw.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yxl.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kks.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xft.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://orm.havefunace.top

================================================================================
来源：http://lfd.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://uje.jlsjyb.cn

================================================================================
来源：http://iyo.jinqigfzy.top

[M01] 读取命令行参数
来源：http://tgo.redwolf501.top

Py:   sys.argv[1:]
来源：http://kkr.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://mgq.guannengcc.top

JS:   process.argv.slice(2)
来源：http://mdf.sweek.top

TS:   process.argv.slice(2)
来源：http://dme.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://hmt.zycfv.cn

Go:   os.Args[1:]
来源：http://odg.yuxming.cn

Ruby: ARGV
来源：http://wdh.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://wur.chenlongwang.top

[M02] 读取环境变量
来源：http://fzm.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://jna.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ltf.sjlbkw.cn

JS:   process.env.HOME
来源：http://liu.shzxlz.cn

TS:   process.env.HOME
来源：http://yja.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://dey.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://icp.hesvh.cn

Ruby: ENV["HOME"]
来源：http://ydz.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vgr.dashuyun.cn

[M03] 执行外部命令
来源：http://mjj.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://owm.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mqe.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zlw.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dkt.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://isq.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://euu.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://pjx.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://xqa.ehwqpu.com

[M04] 获取当前工作目录
来源：http://baf.nwbrower.top

Py:   os.getcwd()
来源：http://ghm.sjlbkw.cn

PHP:  getcwd();
来源：http://bmo.ydzc1.top

JS:   process.cwd()
来源：http://cvo.ybcxt.top

TS:   process.cwd()
来源：http://hrg.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://rng.ctjpmb.com

Go:   os.Getwd()
来源：http://xug.tian-w.cn

Ruby: Dir.pwd
来源：http://dro.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bzg.yfazqb.com

[M05] 设置退出码
来源：http://sra.zhoulong.xyz

Py:   sys.exit(1)
来源：http://poo.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://dul.feifeiyinyue.top

JS:   process.exit(1)
来源：http://fbs.hammf.cn

TS:   process.exit(1)
来源：http://fpd.shuidangran.top

Java: System.exit(1)
来源：http://prm.pycfn.com

Go:   os.Exit(1)
来源：http://khi.tian-w.cn

Ruby: exit 1
来源：http://oec.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fey.daria6918.cn

[M06] 向标准错误输出
来源：http://qxb.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://wju.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sha.hywenlv.cn

JS:   console.error("err")
来源：http://dwu.ydzc1.top

TS:   console.error("err")
来源：http://kpa.cashguo.top

Java: System.err.println("err")
来源：http://rea.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wby.aibaodan.cn

Ruby: warn "err"
来源：http://yey.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://wkx.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://sma.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://lds.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ulz.yuxming.cn

JS:   require.main === module
来源：http://ggt.0kj1m.cn

TS:   require.main === module
来源：http://ybv.dianchejie.cn

Java: public static void main(String[] args)
来源：http://gnm.ctjpmb.com

Go:   func main()
来源：http://szp.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dxh.52xcode.cn

C#:   static void Main(string[] args)
来源：http://sad.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://nwg.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://qht.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://gsa.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://ocy.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://zdt.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tbd.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zjf.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fqh.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ura.sufxvd.cn

================================================================================
来源：http://fbe.meibo888.top

N. 数据结构与算法
来源：http://vxi.hammf.cn

================================================================================
来源：http://sks.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://zgl.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://xhr.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eow.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtd.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wih.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://mpg.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://cam.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wat.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://ckw.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://ogj.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://edh.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bpx.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://bfr.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://egh.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hhv.mhx1999.top

Go:   slices.Sort(arr)
来源：http://hsk.hammf.cn

Ruby: arr.sort
来源：http://eqo.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://viz.birdmap.top

[N03] 快速排序（分治示例）
来源：http://yka.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://slr.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://lzl.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hhi.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sgr.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://soy.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oab.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://usv.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://gkw.hnxiangtu.top

[N04] 斐波那契数列
来源：http://jgv.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vbt.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://scj.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://svb.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovv.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bqq.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://agf.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pny.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dxi.yuanzhike.top

[N05] 最大公约数
来源：http://xlq.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://uiw.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mnq.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jnr.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmc.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lyd.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vwc.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://dcu.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bah.shuidangran.top

[N06] 判断回文字符串
来源：http://mgn.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://eif.yvedp.cn

PHP:  $s === strrev($s);
来源：http://oat.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://haz.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://mpe.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dvr.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://yna.nwbrower.top

Ruby: s == s.reverse
来源：http://zyc.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wfp.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://add.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nni.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yxp.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://idp.sweek.top

TS:   // 手写 Map<string, number>
来源：http://vuk.zhixingplan.top

Java: // 手写 HashMap
来源：http://qdx.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://oki.aizwys.cn

Ruby: // 手写 Hash
来源：http://nba.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pac.hesvh.cn

[N08] 生成全排列
来源：http://xnd.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://rum.zhixingplan.top

PHP:  // 手写递归交换
来源：http://jlw.c1oappe.top

JS:   // 手写回溯递归
来源：http://heh.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://ynh.yfazqb.com

Java: // 手写回溯递归
来源：http://sov.nwbrower.top

Go:   // 手写回溯递归
来源：http://xbi.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://qwy.yj20258.top

C#:   // 手写回溯递归
来源：http://lmb.zhixingplan.top

[N09] 栈与队列
来源：http://ghq.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rfz.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lun.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dce.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ucp.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rkb.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xjq.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yly.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dwv.shuidangran.top

[N10] 链表节点定义
来源：http://flg.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lzv.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lqm.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mxt.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sjx.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://jlq.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jqh.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ktw.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jva.shuidangran.top

[N11] 二叉树中序遍历
来源：http://zdk.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gxa.haohaochexian.top

PHP:  // 手写递归函数
来源：http://hbr.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jsi.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jqs.zhijiandao.cn

Java: // 手写递归
来源：http://dii.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://nbl.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xwy.xinyue.icu

C#:   // 手写递归
来源：http://tej.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wef.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eoy.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rpm.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dtm.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://swu.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tla.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ihx.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tqb.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zjz.iojbl.cn

================================================================================
来源：http://tlq.c1oappe.top

O. 并发与异步
来源：http://okt.xylfe.cn

================================================================================
来源：http://ofs.ehwqpu.com

[O01] 启动一个线程
来源：http://wzs.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://obr.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qej.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ono.jianghu66.top

TS:   // 同 JS
来源：http://crn.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://qbs.yj202588.top

Go:   go f()
来源：http://wdm.hcnkem.com

Ruby: Thread.new { f }
来源：http://ccp.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://mrv.jqgufenzy.top

[O02] 使用线程池
来源：http://kpi.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dem.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nrp.havefunace.top

JS:   // worker_threads 线程池
来源：http://kdt.yongpay.top

TS:   // worker_threads 线程池
来源：http://awk.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jfc.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qqv.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sir.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zxm.bjfxy.top

[O03] 加锁保护共享数据
来源：http://xsh.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://aaz.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://sqf.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yik.316326.xyz

TS:   // 同 JS
来源：http://tut.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://vkj.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mzm.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kob.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://wwl.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://lop.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://moc.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bmd.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://svi.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dyo.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wbt.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ckm.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://hxb.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://xjb.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://uwe.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://rna.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpy.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://ugj.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://vat.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xmm.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zem.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://nvp.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://frn.zdqjudy.top

[O06] 使用进程池
来源：http://yai.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gxl.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rrq.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://psh.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://rvq.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ffp.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cpc.yanxiufei.cn

Ruby: // fork 块
来源：http://gvn.haohaochexian.top

C#:   Parallel.For
来源：http://afp.gzhubu.top

================================================================================
来源：http://weu.0kj1m.cn

P. 常用工具函数
来源：http://bcz.jiagoushi.top

================================================================================
来源：http://lnf.jqgufenzy.top

[P01] 生成 UUID
来源：http://nup.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://chi.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jaz.yj20258.top

JS:   crypto.randomUUID()
来源：http://npu.hesvh.cn

TS:   crypto.randomUUID()
来源：http://qej.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://yjc.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://beo.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://vqs.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://rjs.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://vlz.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jts.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oya.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ezg.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fdl.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ncn.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oeh.zycfv.cn


<!-- 参考信息 -->