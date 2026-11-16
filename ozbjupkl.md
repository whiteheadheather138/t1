代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dft.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yoi.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sqh.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qiw.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xgf.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iii.316326.xyz

[L05] 上传文件（multipart）
来源：http://pnk.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oxw.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://izh.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pqa.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ypc.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://szo.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ghw.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xeb.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://swd.ybcxt.top

[L06] 解析响应为 JSON
来源：http://ooj.smart0.xyz

Py:   resp.json()
来源：http://ysk.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://dfs.ydjk.org.cn

JS:   await resp.json()
来源：http://cpm.sweek.top

TS:   await resp.json()
来源：http://lln.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pgf.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xwq.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://prk.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pet.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://deb.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xkk.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nts.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://chw.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://sbx.cashguo.top

Java: resp.statusCode()
来源：http://pmy.kuanghao11.cn

Go:   resp.StatusCode
来源：http://hhd.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://etv.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://tee.hysaishi.cn

[L08] 并发请求多个地址
来源：http://fwz.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jaq.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://fhy.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gxr.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwm.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://klh.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qfr.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://klt.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kyo.fanxiaobao.xyz

================================================================================
来源：http://hut.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://goj.cucudq.cn

================================================================================
来源：http://wnn.zhoulong.xyz

[M01] 读取命令行参数
来源：http://yqm.vehdjk.com

Py:   sys.argv[1:]
来源：http://mry.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://nzh.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://yyp.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://tod.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://kak.yuanzhike.top

Go:   os.Args[1:]
来源：http://bph.andypj.xyz

Ruby: ARGV
来源：http://owk.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://jyg.hammf.cn

[M02] 读取环境变量
来源：http://onv.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://qmr.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ctd.mhx1999.top

JS:   process.env.HOME
来源：http://gng.tanke756.top

TS:   process.env.HOME
来源：http://rnh.ivvv.top

Java: System.getenv("HOME")
来源：http://pca.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vvy.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://jti.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bdj.fzhhl.top

[M03] 执行外部命令
来源：http://uza.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzd.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aar.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://wlk.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zix.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tks.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://als.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://fxe.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://huo.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://mnv.zhengqikj.top

Py:   os.getcwd()
来源：http://dlo.jyoumei.cn

PHP:  getcwd();
来源：http://ret.52xcode.cn

JS:   process.cwd()
来源：http://fcz.yanxiufei.cn

TS:   process.cwd()
来源：http://uys.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://ifb.yvedp.cn

Go:   os.Getwd()
来源：http://npu.uphjek.com

Ruby: Dir.pwd
来源：http://wpr.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://blz.xylfe.cn

[M05] 设置退出码
来源：http://rol.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://hdk.jinghuilouyu.cn

PHP:  exit(1);
来源：http://ggx.aizwys.cn

JS:   process.exit(1)
来源：http://qpp.nanxinkj.top

TS:   process.exit(1)
来源：http://tup.fehbvm.com

Java: System.exit(1)
来源：http://dqs.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://dmm.hcnkem.com

Ruby: exit 1
来源：http://tlx.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iem.tian-w.cn

[M06] 向标准错误输出
来源：http://ydf.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://slu.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fbi.gzhubu.top

JS:   console.error("err")
来源：http://jae.jiagoushi.top

TS:   console.error("err")
来源：http://iwk.yongpay.top

Java: System.err.println("err")
来源：http://oui.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xux.tarul.cn

Ruby: warn "err"
来源：http://oxy.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://xod.jiagoushi.top

[M07] 判断是否为主入口
来源：http://zwk.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://ejb.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dzg.sufxvd.cn

JS:   require.main === module
来源：http://obf.hysaishi.cn

TS:   require.main === module
来源：http://oev.vehdjk.com

Java: public static void main(String[] args)
来源：http://ngz.jlsjyb.cn

Go:   func main()
来源：http://fjs.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ful.ydzc1.top

C#:   static void Main(string[] args)
来源：http://zhm.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://nmy.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://ugx.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://odf.guowangkeji.top

JS:   process.platform;  process.version
来源：http://wbk.fengsongda.top

TS:   process.platform;  process.version
来源：http://xsf.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jik.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cqh.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nsl.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hzw.gotoacloud.top

================================================================================
来源：http://xou.yfazqb.com

N. 数据结构与算法
来源：http://tfv.shangyingyoupin.top

================================================================================
来源：http://mcx.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://oto.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rxi.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xte.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nnx.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msj.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://tgb.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://xmz.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ocs.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://nef.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://whw.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://jyy.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fla.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tsw.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://mtl.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ggy.fzhhl.top

Go:   slices.Sort(arr)
来源：http://bnd.tanke756.top

Ruby: arr.sort
来源：http://sca.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zah.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://cpi.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lnr.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://ssp.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vfc.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cgl.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lku.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mys.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://maj.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qkh.vqdsnc.cn

[N04] 斐波那契数列
来源：http://aak.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lli.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://njv.chenlongwang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yym.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ndw.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cya.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yhp.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://drj.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uxy.zhongyouzk.top

[N05] 最大公约数
来源：http://jvz.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://gre.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ubm.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cvq.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qzr.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sii.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qhn.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://hoz.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bvb.yangfankeji.com

[N06] 判断回文字符串
来源：http://ycz.jlsjyb.cn

Py:   s == s[::-1]
来源：http://eba.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://soh.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://nwb.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://nbf.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yvd.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://urh.tian-w.cn

Ruby: s == s.reverse
来源：http://yng.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eym.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://ubi.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kkk.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fqs.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://mfy.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://iwc.jinqigfzy.top

Java: // 手写 HashMap
来源：http://ynk.guannengcc.top

Go:   // 手写 map[int]int
来源：http://hye.yuanzhike.top

Ruby: // 手写 Hash
来源：http://sno.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://opd.iojbl.cn

[N08] 生成全排列
来源：http://lkh.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://von.guowangkeji.top

PHP:  // 手写递归交换
来源：http://whg.snrcjt.cn

JS:   // 手写回溯递归
来源：http://pqv.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://ocu.cashguo.top

Java: // 手写回溯递归
来源：http://ltj.yj202588.top

Go:   // 手写回溯递归
来源：http://zai.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://tgg.chenzaomai.com

C#:   // 手写回溯递归
来源：http://bfj.shzxlz.cn

[N09] 栈与队列
来源：http://mlc.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://exg.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qmn.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gwi.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xns.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pxp.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aoc.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tip.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kuu.sweek.top

[N10] 链表节点定义
来源：http://ftb.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hce.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sty.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oqk.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://isa.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://ncu.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://nyz.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qzt.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ycn.daria6918.cn

[N11] 二叉树中序遍历
来源：http://bbv.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://znd.feifeiyinyue.top

PHP:  // 手写递归函数
来源：http://vaq.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lby.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bbb.shzxlz.cn

Java: // 手写递归
来源：http://lpy.kuanghao11.cn

Go:   // 手写递归
来源：http://qps.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ych.nanxinkj.top

C#:   // 手写递归
来源：http://mks.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://emn.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xad.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fme.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kih.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tct.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://reu.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://asl.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jjj.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ned.jinyuanbaomall.cn

================================================================================
来源：http://zwc.zhijiandao.cn

O. 并发与异步
来源：http://txj.redwolf501.top

================================================================================
来源：http://afo.vehdjk.com

[O01] 启动一个线程
来源：http://hry.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pgi.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iov.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dgy.svipenyu.cn

TS:   // 同 JS
来源：http://aox.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://fnw.pycfn.com

Go:   go f()
来源：http://zla.daxiang520.top

Ruby: Thread.new { f }
来源：http://bab.yongpay.top

C#:   Task.Run(() => F());
来源：http://fjs.shzxlz.cn

[O02] 使用线程池
来源：http://ird.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uzu.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mkd.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://ocl.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://qau.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://yjd.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uso.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mku.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://clf.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://zav.wangdashe.top

Py:   with lock: shared += 1
来源：http://lub.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://tvu.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://adj.sweek.top

TS:   // 同 JS
来源：http://vwj.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://uip.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xmq.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://arj.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://rmr.nwbrower.top

[O04] 定义异步函数并等待
来源：http://pqy.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://jww.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vno.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://yin.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rkj.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yug.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://juy.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://pku.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://zty.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://kdj.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://yhf.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zla.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://zff.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://vsf.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mgb.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cxe.smart0.xyz

Ruby: threads.map(&:join)
来源：http://pdh.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://giw.tianlin.xyz

[O06] 使用进程池
来源：http://dcw.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://prf.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ban.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://ijv.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://svx.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ddo.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vfq.yuxming.cn

Ruby: // fork 块
来源：http://pri.haohaochexian.top

C#:   Parallel.For
来源：http://rce.nanxuanxn.top

================================================================================
来源：http://ysb.gzhubu.top

P. 常用工具函数
来源：http://gek.316326.xyz

================================================================================
来源：http://bpp.jinqigufen.top

[P01] 生成 UUID
来源：http://jnj.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://cyp.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lfn.yfazqb.com

JS:   crypto.randomUUID()
来源：http://mzl.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://ezk.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://hsd.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://vnd.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://tlb.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://cal.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://nyf.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rml.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cfh.0kj1m.cn


<!-- 参考信息 -->