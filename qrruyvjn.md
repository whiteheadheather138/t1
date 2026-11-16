代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qlz.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://otp.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://fdb.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bxh.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hfo.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ede.jlsjyb.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://amx.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rpm.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ohj.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ntc.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ncu.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://smw.fktsv.cn

Py:   resp.json()
来源：http://scz.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://cwq.zhengqikj.top

JS:   await resp.json()
来源：http://dnt.shuidangran.top

TS:   await resp.json()
来源：http://ptx.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://omn.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jat.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://fym.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://txj.sweek.top

[L07] 处理 HTTP 状态码
来源：http://rzf.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ofh.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ycl.tanke756.top

JS:   resp.ok;  resp.status
来源：http://nmc.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://pug.hnqzz.top

Java: resp.statusCode()
来源：http://lwu.fzhhl.top

Go:   resp.StatusCode
来源：http://pym.meibo888.top

Ruby: resp.code.to_i
来源：http://zzi.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://vrj.tian-w.cn

[L08] 并发请求多个地址
来源：http://kqh.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wro.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://wlu.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tyh.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nyp.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xrf.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fta.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nvu.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fiw.gzhubu.top

================================================================================
来源：http://bks.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://ijx.tarul.cn

================================================================================
来源：http://apu.yvedp.cn

[M01] 读取命令行参数
来源：http://sgo.guowangkeji.top

Py:   sys.argv[1:]
来源：http://ymr.aizwys.cn

PHP:  $argv;  $argc;
来源：http://sju.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://han.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://ova.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://cpq.zhixingplan.top

Go:   os.Args[1:]
来源：http://typ.yueranfly.top

Ruby: ARGV
来源：http://liq.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://wzh.ppjwa.cn

[M02] 读取环境变量
来源：http://nrq.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://xdm.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uzv.hnxiangtu.top

JS:   process.env.HOME
来源：http://mld.guowangkeji.top

TS:   process.env.HOME
来源：http://vdv.yueranfly.top

Java: System.getenv("HOME")
来源：http://cnx.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rtc.c1oappe.top

Ruby: ENV["HOME"]
来源：http://naj.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uyo.xinyue.icu

[M03] 执行外部命令
来源：http://xfa.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hny.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jjq.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aie.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ncj.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://szo.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://yrq.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xqi.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://ukj.dianchejie.cn

[M04] 获取当前工作目录
来源：http://yys.aibaodan.cn

Py:   os.getcwd()
来源：http://bng.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://kmz.gaohongyu789.top

JS:   process.cwd()
来源：http://esa.xuetiantiany.cn

TS:   process.cwd()
来源：http://dlu.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://huv.yonumen.top

Go:   os.Getwd()
来源：http://nil.fehbvm.com

Ruby: Dir.pwd
来源：http://tie.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://ppw.fengsongda.top

[M05] 设置退出码
来源：http://ees.hysaishi.cn

Py:   sys.exit(1)
来源：http://mwi.shangyingyoupin.top

PHP:  exit(1);
来源：http://src.jyoumei.cn

JS:   process.exit(1)
来源：http://gks.andypj.xyz

TS:   process.exit(1)
来源：http://kjw.sxryk.cn

Java: System.exit(1)
来源：http://ard.wangdashe.top

Go:   os.Exit(1)
来源：http://avh.meibo888.top

Ruby: exit 1
来源：http://mwj.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fze.iojbl.cn

[M06] 向标准错误输出
来源：http://brc.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://ade.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ksk.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://jab.jianghu66.top

TS:   console.error("err")
来源：http://kcc.guannengcc.top

Java: System.err.println("err")
来源：http://vjv.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knd.pycfn.com

Ruby: warn "err"
来源：http://zuh.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://qle.zdbjq.cn

[M07] 判断是否为主入口
来源：http://tub.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://nlm.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zmc.fanxiaobao.xyz

JS:   require.main === module
来源：http://cfb.zhijiandao.cn

TS:   require.main === module
来源：http://tbf.c1oappe.top

Java: public static void main(String[] args)
来源：http://yrb.xuetiantiany.cn

Go:   func main()
来源：http://etl.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rff.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://hyv.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://wyz.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://suk.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://zjv.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://hov.cashguo.top

TS:   process.platform;  process.version
来源：http://akb.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csg.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sfg.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vdw.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pru.cqqwz.cn

================================================================================
来源：http://ulv.yanxiufei.cn

N. 数据结构与算法
来源：http://qqw.gotoacloud.top

================================================================================
来源：http://ufz.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://doi.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://pci.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ryw.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xzj.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ssh.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hql.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://ptx.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://whl.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://umt.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://nkg.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://fwx.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fke.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vxg.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hgi.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cjt.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://yvk.jqgufenzy.top

Ruby: arr.sort
来源：http://moc.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ymx.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://hev.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://paz.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://umy.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hbk.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zrv.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ebw.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oqa.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wdr.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://pfj.tian-w.cn

[N04] 斐波那契数列
来源：http://zgf.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fct.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rqx.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qho.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysa.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qac.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qdd.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wbq.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cxq.hcnkem.com

[N05] 最大公约数
来源：http://jsf.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://bwo.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gjl.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swo.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ndm.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dzc.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kno.xylfe.cn

Ruby: a.gcd(b)
来源：http://enr.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://guk.xuanzx.com

[N06] 判断回文字符串
来源：http://coa.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://qhb.tian-w.cn

PHP:  $s === strrev($s);
来源：http://gns.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://pzl.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://owu.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cqs.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://fpb.jinqigufen.top

Ruby: s == s.reverse
来源：http://awn.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ofm.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://jkt.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jwp.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hrd.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://clw.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://tsc.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://euc.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://tdo.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://xgv.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ewf.cdnleiting.top

[N08] 生成全排列
来源：http://rfx.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://ivm.aibaodan.cn

PHP:  // 手写递归交换
来源：http://qsu.redwolf501.top

JS:   // 手写回溯递归
来源：http://tof.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://kkz.sjlbkw.cn

Java: // 手写回溯递归
来源：http://nrc.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://uub.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://lfq.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://gln.jiagoushi.top

[N09] 栈与队列
来源：http://ths.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://foq.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xze.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pjz.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fti.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jjs.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rnz.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xse.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lcm.jlsjyb.cn

[N10] 链表节点定义
来源：http://evo.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://daw.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zes.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tgh.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iur.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://fry.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://llp.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://way.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kth.316326.xyz

[N11] 二叉树中序遍历
来源：http://ptc.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://typ.mhx1999.top

PHP:  // 手写递归函数
来源：http://drn.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmo.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bib.jqgfzy.top

Java: // 手写递归
来源：http://vdm.shangyingyoupin.top

Go:   // 手写递归
来源：http://dvr.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aav.zhoulong.xyz

C#:   // 手写递归
来源：http://luw.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jfz.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://upl.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hzk.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mta.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zdv.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://isu.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jkb.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mwd.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kux.sjlbkw.cn

================================================================================
来源：http://huq.jinqigufen.top

O. 并发与异步
来源：http://qln.iojbl.cn

================================================================================
来源：http://sem.havefunace.top

[O01] 启动一个线程
来源：http://rzw.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vyk.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pmq.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nht.xylfe.cn

TS:   // 同 JS
来源：http://cli.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://sbx.gzhubu.top

Go:   go f()
来源：http://bjw.jqgfzy.top

Ruby: Thread.new { f }
来源：http://gnp.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://aoz.gaohongyu789.top

[O02] 使用线程池
来源：http://vif.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tcp.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bal.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://ukq.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://zik.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://xpb.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tsv.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cmv.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://shc.yonumen.top

[O03] 加锁保护共享数据
来源：http://ccx.mhx1999.top

Py:   with lock: shared += 1
来源：http://mff.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://isk.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ylp.52xcode.cn

TS:   // 同 JS
来源：http://bog.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://fcl.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xue.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zji.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://nhp.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://cqo.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://zfn.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rxd.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://tij.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sns.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vfq.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ihx.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fof.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://ocp.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://faa.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://yin.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yvj.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://dbu.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://lht.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hvs.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://egy.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://qxr.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://uzb.feifeiyinyue.top

[O06] 使用进程池
来源：http://tui.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iuc.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xoq.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://dqs.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://qml.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://axe.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mwr.jinqigufen.top

Ruby: // fork 块
来源：http://wun.fktsv.cn

C#:   Parallel.For
来源：http://tyk.nanxinkj.top

================================================================================
来源：http://fhl.sweek.top

P. 常用工具函数
来源：http://akh.nanxinkj.top

================================================================================
来源：http://ubs.kuanghao11.cn

[P01] 生成 UUID
来源：http://zrg.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://pwx.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lhq.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://dvo.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://qlr.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://txf.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://clk.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://vpu.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://jpw.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://fqy.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://frb.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://srw.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jlz.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qmz.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wbf.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zbd.mhx1999.top


<!-- 参考信息 -->