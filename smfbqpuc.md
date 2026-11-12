代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mny.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fkf.nwbrower.top

[L05] 上传文件（multipart）
来源：http://wmp.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mxa.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dig.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xzq.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kvl.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sah.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tjs.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zhn.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lrc.hnqzz.top

[L06] 解析响应为 JSON
来源：http://amq.fktsv.cn

Py:   resp.json()
来源：http://wmn.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://sxt.zycfv.cn

JS:   await resp.json()
来源：http://gqa.meibo888.top

TS:   await resp.json()
来源：http://ure.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qnd.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ihr.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://mek.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://trd.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://rpj.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ixm.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ida.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://itl.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://iwt.c1oappe.top

Java: resp.statusCode()
来源：http://ios.sufxvd.cn

Go:   resp.StatusCode
来源：http://mwo.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://tpy.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://jnr.ivvv.top

[L08] 并发请求多个地址
来源：http://lqo.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://myc.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://toa.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://poi.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ace.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ycb.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wqg.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ikw.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lev.316326.xyz

================================================================================
来源：http://rec.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://syx.ydjk.org.cn

================================================================================
来源：http://zxj.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://cxj.epnwcf.com

Py:   sys.argv[1:]
来源：http://mjg.sysykeji.top

PHP:  $argv;  $argc;
来源：http://kdx.daria6918.cn

JS:   process.argv.slice(2)
来源：http://dcv.smart0.xyz

TS:   process.argv.slice(2)
来源：http://age.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://kwp.snrcjt.cn

Go:   os.Args[1:]
来源：http://ysx.daria6918.cn

Ruby: ARGV
来源：http://yhd.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://ucz.meibo888.top

[M02] 读取环境变量
来源：http://xzx.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://gua.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rvs.quarkkingdee.top

JS:   process.env.HOME
来源：http://zhj.hesvh.cn

TS:   process.env.HOME
来源：http://doq.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://ebu.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vsg.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://hvp.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ibx.316326.xyz

[M03] 执行外部命令
来源：http://vgn.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xyi.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cxd.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vkw.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ojw.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wlz.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yxu.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://jvd.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://bgt.hcnkem.com

[M04] 获取当前工作目录
来源：http://ufc.vqdsnc.cn

Py:   os.getcwd()
来源：http://enb.cheryme.top

PHP:  getcwd();
来源：http://yxi.ppjwa.cn

JS:   process.cwd()
来源：http://ijw.jqgufenzy.top

TS:   process.cwd()
来源：http://xdg.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://fzr.hywenlv.cn

Go:   os.Getwd()
来源：http://erj.c1oappe.top

Ruby: Dir.pwd
来源：http://uut.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iic.vqdsnc.cn

[M05] 设置退出码
来源：http://ayz.gotoacloud.top

Py:   sys.exit(1)
来源：http://prr.zhongyouzk.top

PHP:  exit(1);
来源：http://mzt.shuidangran.top

JS:   process.exit(1)
来源：http://tyl.shzxlz.cn

TS:   process.exit(1)
来源：http://bbm.nwbrower.top

Java: System.exit(1)
来源：http://uny.yj20258888.top

Go:   os.Exit(1)
来源：http://xit.svipenyu.cn

Ruby: exit 1
来源：http://gwo.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pso.zhixingplan.top

[M06] 向标准错误输出
来源：http://mmp.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://sfh.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fbk.hongshengwenyu.top

JS:   console.error("err")
来源：http://neh.fehbvm.com

TS:   console.error("err")
来源：http://btp.fengsongda.top

Java: System.err.println("err")
来源：http://lbx.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvz.wangdashe.top

Ruby: warn "err"
来源：http://wcz.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://efx.ehwqpu.com

[M07] 判断是否为主入口
来源：http://aos.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://yzp.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oys.sysykeji.top

JS:   require.main === module
来源：http://qae.sjlbkw.cn

TS:   require.main === module
来源：http://rip.daxiang520.top

Java: public static void main(String[] args)
来源：http://icf.cucudq.cn

Go:   func main()
来源：http://elw.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://osl.pycfn.com

C#:   static void Main(string[] args)
来源：http://sig.yongpay.top

[M08] 获取系统与运行时信息
来源：http://yli.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://tih.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://uml.snrcjt.cn

JS:   process.platform;  process.version
来源：http://jcf.c1oappe.top

TS:   process.platform;  process.version
来源：http://vcg.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://osj.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iuv.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gbx.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fpl.ehwqpu.com

================================================================================
来源：http://qas.yj20258888.top

N. 数据结构与算法
来源：http://stx.haohaochexian.top

================================================================================
来源：http://xbi.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://nsi.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://ohk.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rjc.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxq.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tad.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ixf.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://wlb.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://yes.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://nbj.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://fuu.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://thn.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ugb.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kgr.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://skn.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jfe.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://zoq.xylfe.cn

Ruby: arr.sort
来源：http://xwa.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mof.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://lke.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mcb.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://enq.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgu.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wlx.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nnt.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://asz.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://voi.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://txn.svipenyu.cn

[N04] 斐波那契数列
来源：http://ofa.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lrw.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://luv.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://swd.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vni.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dgh.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hho.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fgd.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pyh.zdbjq.cn

[N05] 最大公约数
来源：http://sgh.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://kxs.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ecy.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evo.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohe.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ugl.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pco.hesvh.cn

Ruby: a.gcd(b)
来源：http://odt.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yjp.wangdashe.top

[N06] 判断回文字符串
来源：http://lyr.sweek.top

Py:   s == s[::-1]
来源：http://mka.yongpay.top

PHP:  $s === strrev($s);
来源：http://lep.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://rqy.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://ssz.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xmx.redwolf501.top

Go:   // 双指针从两端比较
来源：http://neq.yongpay.top

Ruby: s == s.reverse
来源：http://vgp.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ytb.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://cwt.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ikq.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bsh.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://tqv.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://tda.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://wlt.c1oappe.top

Go:   // 手写 map[int]int
来源：http://zui.cdnleiting.top

Ruby: // 手写 Hash
来源：http://fey.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://jzt.smart0.xyz

[N08] 生成全排列
来源：http://wpw.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://igv.zhengqikj.top

PHP:  // 手写递归交换
来源：http://hkg.ybcxt.top

JS:   // 手写回溯递归
来源：http://byy.yangfankeji.com

TS:   // 手写回溯递归
来源：http://jgg.ydzc1.top

Java: // 手写回溯递归
来源：http://fsg.zhengqikj.top

Go:   // 手写回溯递归
来源：http://oru.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://ioc.ivvv.top

C#:   // 手写回溯递归
来源：http://dbc.jlsjyb.cn

[N09] 栈与队列
来源：http://usd.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://twh.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pfu.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hxd.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://piu.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dna.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bia.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://utd.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mft.snrcjt.cn

[N10] 链表节点定义
来源：http://lbt.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zyj.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jpw.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aff.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aci.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://lit.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vte.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://chj.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ffl.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://sun.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lhi.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://dej.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gsh.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tnk.hywenlv.cn

Java: // 手写递归
来源：http://rga.jinqigfzy.top

Go:   // 手写递归
来源：http://tcj.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rxf.bjfxy.top

C#:   // 手写递归
来源：http://arf.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ood.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zle.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sol.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hap.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uhh.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ivs.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ovf.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zmn.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sht.yanxiufei.cn

================================================================================
来源：http://sym.daria6918.cn

O. 并发与异步
来源：http://jee.c1oappe.top

================================================================================
来源：http://nmn.shzxlz.cn

[O01] 启动一个线程
来源：http://wrv.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kbc.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bjk.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lsw.jyoumei.cn

TS:   // 同 JS
来源：http://yje.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://vqh.hywenlv.cn

Go:   go f()
来源：http://vlv.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://rns.tarul.cn

C#:   Task.Run(() => F());
来源：http://ynu.uphjek.com

[O02] 使用线程池
来源：http://gpj.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kef.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zkx.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://opy.cashguo.top

TS:   // worker_threads 线程池
来源：http://rak.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://szb.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kkw.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xax.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dgn.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://hia.zycfv.cn

Py:   with lock: shared += 1
来源：http://xgq.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://pur.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pmp.zhiwuduotai.top

TS:   // 同 JS
来源：http://fxj.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://xky.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kju.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rws.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://hfm.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://wec.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://cqh.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tdr.yvedp.cn

JS:   async function f() { await g(); }
来源：http://bej.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xop.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mfi.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dqa.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://crh.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://dma.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://wgx.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://wwe.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://coj.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://uxl.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://tpy.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oco.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://igq.fzhhl.top

Ruby: threads.map(&:join)
来源：http://usw.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kqy.havefunace.top

[O06] 使用进程池
来源：http://wpd.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://avc.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://szg.iojbl.cn

JS:   // child_process / cluster 模块
来源：http://xaf.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://xkp.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gtl.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kvt.vehdjk.com

Ruby: // fork 块
来源：http://vpp.yongpay.top

C#:   Parallel.For
来源：http://oau.yongpay.top

================================================================================
来源：http://ynj.hnxiangtu.top

P. 常用工具函数
来源：http://jad.haohaochexian.top

================================================================================
来源：http://taq.hysaishi.cn

[P01] 生成 UUID
来源：http://kkr.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://evi.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://anu.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://mmv.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://qwo.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://exs.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://ace.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://yzk.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://hpz.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://zsh.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://urh.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hep.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ckp.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wdj.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uce.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rln.zycfv.cn


<!-- 参考信息 -->