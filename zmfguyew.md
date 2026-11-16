代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxi.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlx.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xbk.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nif.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gpi.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://erm.mhx1999.top

[L05] 上传文件（multipart）
来源：http://oii.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fkz.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rvp.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bes.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fps.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dad.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://caw.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tvr.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wnu.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://qqj.kuanghao11.cn

Py:   resp.json()
来源：http://yel.ydzc1.top

PHP:  json_decode($body, true);
来源：http://fwn.zycfv.cn

JS:   await resp.json()
来源：http://sks.vqdsnc.cn

TS:   await resp.json()
来源：http://dyg.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oqm.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://skh.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://lzb.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mof.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://djc.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jwq.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hon.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://ger.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://bge.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://dxl.yj20258.top

Go:   resp.StatusCode
来源：http://zyr.c1oappe.top

Ruby: resp.code.to_i
来源：http://anl.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://qes.hfpthk.cn

[L08] 并发请求多个地址
来源：http://tts.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fmi.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://xxi.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wva.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://foe.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hbd.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ust.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nyw.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://llq.yuanzhike.top

================================================================================
来源：http://hzc.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://bdh.chenjidiqi.icu

================================================================================
来源：http://gwu.0kj1m.cn

[M01] 读取命令行参数
来源：http://nhs.hysaishi.cn

Py:   sys.argv[1:]
来源：http://uuj.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://kgl.hesvh.cn

JS:   process.argv.slice(2)
来源：http://sgx.nwbrower.top

TS:   process.argv.slice(2)
来源：http://bqe.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://qes.zhijiandao.cn

Go:   os.Args[1:]
来源：http://utb.yvedp.cn

Ruby: ARGV
来源：http://tdg.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://qva.jinqigfzy.top

[M02] 读取环境变量
来源：http://gjt.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://bul.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nqc.zhongyouzk.top

JS:   process.env.HOME
来源：http://ccz.hnxiangtu.top

TS:   process.env.HOME
来源：http://tuc.xuanzx.com

Java: System.getenv("HOME")
来源：http://mqp.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nmt.guannengcc.top

Ruby: ENV["HOME"]
来源：http://kwg.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://krf.pengpengdd.cyou

[M03] 执行外部命令
来源：http://kmm.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://byi.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fpq.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xav.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eqk.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rkb.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eyh.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://dda.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://jyy.hammf.cn

[M04] 获取当前工作目录
来源：http://ryr.yj20258888.top

Py:   os.getcwd()
来源：http://rby.shanyushiyangtech.top

PHP:  getcwd();
来源：http://hwg.guannengcc.top

JS:   process.cwd()
来源：http://cro.tarul.cn

TS:   process.cwd()
来源：http://opj.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://ysj.zhijiandao.cn

Go:   os.Getwd()
来源：http://pzq.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://wve.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://vuv.yueranfly.top

[M05] 设置退出码
来源：http://jrk.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://mpr.ybcxt.top

PHP:  exit(1);
来源：http://uey.yanxiufei.cn

JS:   process.exit(1)
来源：http://xuy.sweek.top

TS:   process.exit(1)
来源：http://lja.hcnkem.com

Java: System.exit(1)
来源：http://qil.vqdsnc.cn

Go:   os.Exit(1)
来源：http://nln.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://iqv.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxt.ybcxt.top

[M06] 向标准错误输出
来源：http://gtf.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://lgo.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://wnv.daria6918.cn

JS:   console.error("err")
来源：http://ygb.zycfv.cn

TS:   console.error("err")
来源：http://lyy.nwbrower.top

Java: System.err.println("err")
来源：http://wiv.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wkc.shuidangran.top

Ruby: warn "err"
来源：http://hny.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://aau.aibaodan.cn

[M07] 判断是否为主入口
来源：http://iab.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://esh.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ptn.9152youxi.cn

JS:   require.main === module
来源：http://oca.xinyue.icu

TS:   require.main === module
来源：http://pid.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://wtz.ywan-chungtsiang.top

Go:   func main()
来源：http://brk.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hts.xylfe.cn

C#:   static void Main(string[] args)
来源：http://tfg.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://kec.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://tmc.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://awf.ydzc1.top

JS:   process.platform;  process.version
来源：http://nmi.jianghu66.top

TS:   process.platform;  process.version
来源：http://yvv.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zck.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jhd.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zkt.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://dqr.ybcxt.top

================================================================================
来源：http://eep.yueranfly.top

N. 数据结构与算法
来源：http://dxu.wangdashe.top

================================================================================
来源：http://jak.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://iek.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://phi.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fmj.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hje.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sro.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://tai.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://ivn.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iof.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yak.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://ywy.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://acn.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hkz.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tzx.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vdr.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rbe.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://bod.bjfxy.top

Ruby: arr.sort
来源：http://yoq.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xwa.havefunace.top

[N03] 快速排序（分治示例）
来源：http://gzs.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uud.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://bxi.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://emk.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkj.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mhy.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oxk.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mhv.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://okk.jqgfzy.top

[N04] 斐波那契数列
来源：http://osn.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oib.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lud.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfs.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gcv.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tcw.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://upv.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qxs.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ndj.shanyushiyangtech.top

[N05] 最大公约数
来源：http://emy.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://han.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kby.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lwt.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://coo.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kym.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tus.yj20258.top

Ruby: a.gcd(b)
来源：http://ili.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xmo.sweek.top

[N06] 判断回文字符串
来源：http://ivh.fzhhl.top

Py:   s == s[::-1]
来源：http://jba.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://ryl.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://phj.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://zrr.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vse.ivvv.top

Go:   // 双指针从两端比较
来源：http://yqw.fktsv.cn

Ruby: s == s.reverse
来源：http://dlb.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jci.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://zan.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yud.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lxk.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qto.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://ode.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://jjg.mhx1999.top

Go:   // 手写 map[int]int
来源：http://rsu.uphjek.com

Ruby: // 手写 Hash
来源：http://jbn.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://gko.hammf.cn

[N08] 生成全排列
来源：http://xzx.yj20258.top

Py:   itertools.permutations(arr)
来源：http://dip.birdmap.top

PHP:  // 手写递归交换
来源：http://rtv.sysykeji.top

JS:   // 手写回溯递归
来源：http://xnt.9152youxi.cn

TS:   // 手写回溯递归
来源：http://hic.sweek.top

Java: // 手写回溯递归
来源：http://jia.nwbrower.top

Go:   // 手写回溯递归
来源：http://dfm.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://qae.xinyue.icu

C#:   // 手写回溯递归
来源：http://jqn.shuidangran.top

[N09] 栈与队列
来源：http://hhn.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kby.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pqg.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qpo.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hjb.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oai.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aoc.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qhy.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eot.jyoumei.cn

[N10] 链表节点定义
来源：http://eee.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qff.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yvp.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://upt.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lmq.uphjek.com

Java: class Node { int v; Node next; }
来源：http://trn.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://igc.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pee.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jsu.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://nmk.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ltb.haohaochexian.top

PHP:  // 手写递归函数
来源：http://mvh.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://utc.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yjp.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://ioe.jyoumei.cn

Go:   // 手写递归
来源：http://muz.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://azh.shuidangran.top

C#:   // 手写递归
来源：http://qvb.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cnj.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eor.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bcf.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bsx.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbg.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://spc.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iww.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://got.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hso.yangfankeji.com

================================================================================
来源：http://jgm.9152youxi.cn

O. 并发与异步
来源：http://vkq.quarkkingdee.top

================================================================================
来源：http://wpy.zhengqikj.top

[O01] 启动一个线程
来源：http://ovj.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gtc.tanke756.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hns.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ljy.hesvh.cn

TS:   // 同 JS
来源：http://cwu.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://phh.pycfn.com

Go:   go f()
来源：http://zil.ydzc1.top

Ruby: Thread.new { f }
来源：http://map.hcnkem.com

C#:   Task.Run(() => F());
来源：http://osg.pycfn.com

[O02] 使用线程池
来源：http://ezn.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tdg.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dlx.meibo888.top

JS:   // worker_threads 线程池
来源：http://xbo.hesvh.cn

TS:   // worker_threads 线程池
来源：http://zdq.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://zwe.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sng.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pry.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kfh.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://oxu.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://xps.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://tzy.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hmq.fanxiaobao.xyz

TS:   // 同 JS
来源：http://xjm.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://lir.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zze.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://scl.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://xnw.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://ecn.tarul.cn

Py:   async def f():⏎    await g()
来源：http://qlr.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://irx.yfazqb.com

JS:   async function f() { await g(); }
来源：http://cle.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rgw.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pqy.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rfd.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://rvz.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://vlx.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://qvf.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://ehy.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yvq.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://lbl.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://yuz.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ikz.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://edx.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://jnh.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zfw.sjlbkw.cn

[O06] 使用进程池
来源：http://gln.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://drw.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xdi.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://tez.havefunace.top

TS:   // child_process / cluster 模块
来源：http://lok.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gyx.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hbv.snrcjt.cn

Ruby: // fork 块
来源：http://ftw.jianghu66.top

C#:   Parallel.For
来源：http://zuw.epnwcf.com

================================================================================
来源：http://gfn.yonumen.top

P. 常用工具函数
来源：http://plh.zhaomingkeji.xyz

================================================================================
来源：http://mfs.zhoulong.xyz

[P01] 生成 UUID
来源：http://eqi.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://nho.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uvl.tian-w.cn

JS:   crypto.randomUUID()
来源：http://qtu.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://ref.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://doj.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://lan.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://sjd.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://mwe.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://fsi.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hjh.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ptu.jiagoushi.top


<!-- 参考信息 -->