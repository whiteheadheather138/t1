代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://naw.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ukk.hesvh.cn

[L05] 上传文件（multipart）
来源：http://ozp.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aly.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nmc.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pov.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fse.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hvu.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ayv.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cif.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hbz.cheryme.top

[L06] 解析响应为 JSON
来源：http://rtf.jinqigfzy.top

Py:   resp.json()
来源：http://npu.fzhhl.top

PHP:  json_decode($body, true);
来源：http://gjx.tarul.cn

JS:   await resp.json()
来源：http://nqz.sweek.top

TS:   await resp.json()
来源：http://xme.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cof.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tbt.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://sot.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xst.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://ehu.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dfs.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://usm.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://fpa.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://dng.jinqigfzy.top

Java: resp.statusCode()
来源：http://szg.hfpthk.cn

Go:   resp.StatusCode
来源：http://yxs.ctjpmb.com

Ruby: resp.code.to_i
来源：http://qjm.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://ccj.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://ohx.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yql.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://zhb.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eze.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://okd.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vlv.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://svi.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eye.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gbh.yueranfly.top

================================================================================
来源：http://jcs.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://vek.shuidangran.top

================================================================================
来源：http://tyf.hywenlv.cn

[M01] 读取命令行参数
来源：http://gxr.cucudq.cn

Py:   sys.argv[1:]
来源：http://qap.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://qoq.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://igb.hcnkem.com

TS:   process.argv.slice(2)
来源：http://cup.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://esk.yanxiufei.cn

Go:   os.Args[1:]
来源：http://kzq.guowangkeji.top

Ruby: ARGV
来源：http://qfw.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://wjh.iojbl.cn

[M02] 读取环境变量
来源：http://bee.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://ecg.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://axw.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://zzq.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://rwr.cdnleiting.top

Java: System.getenv("HOME")
来源：http://mlj.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ipa.guannengcc.top

Ruby: ENV["HOME"]
来源：http://xux.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://krs.ehwqpu.com

[M03] 执行外部命令
来源：http://imr.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ear.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://doo.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://rzu.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uct.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fnp.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://iwq.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://hgx.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://lcr.andypj.xyz

[M04] 获取当前工作目录
来源：http://bri.uphjek.com

Py:   os.getcwd()
来源：http://beb.yonumen.top

PHP:  getcwd();
来源：http://hxy.shangyingyoupin.top

JS:   process.cwd()
来源：http://dss.pengpengdd.cyou

TS:   process.cwd()
来源：http://kgp.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://gxx.daria6918.cn

Go:   os.Getwd()
来源：http://jep.jqgfzy.top

Ruby: Dir.pwd
来源：http://zey.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iio.jinqigufen.top

[M05] 设置退出码
来源：http://pyl.redwolf501.top

Py:   sys.exit(1)
来源：http://hrs.zhengqikj.top

PHP:  exit(1);
来源：http://yyn.ehwqpu.com

JS:   process.exit(1)
来源：http://vbm.zhiwuduotai.top

TS:   process.exit(1)
来源：http://sci.mhx1999.top

Java: System.exit(1)
来源：http://skx.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://rpq.daxiang520.top

Ruby: exit 1
来源：http://bba.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gaa.zdqjudy.top

[M06] 向标准错误输出
来源：http://flc.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://bji.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://itk.shangyingyoupin.top

JS:   console.error("err")
来源：http://sgd.yanxiufei.cn

TS:   console.error("err")
来源：http://xov.nanxuanxn.top

Java: System.err.println("err")
来源：http://sdh.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://chn.0kj1m.cn

Ruby: warn "err"
来源：http://lrm.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://xlx.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://vub.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://gtf.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aaa.zhixingplan.top

JS:   require.main === module
来源：http://ixm.ehwqpu.com

TS:   require.main === module
来源：http://arc.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://lmc.ydjk.org.cn

Go:   func main()
来源：http://hmm.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qpw.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://pqz.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://lku.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://yvq.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://ekm.cucudq.cn

JS:   process.platform;  process.version
来源：http://csv.ctjpmb.com

TS:   process.platform;  process.version
来源：http://enf.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://juu.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://lgz.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pjm.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gri.xuetiantiany.cn

================================================================================
来源：http://opr.0kj1m.cn

N. 数据结构与算法
来源：http://vpn.gogol.net.cn

================================================================================
来源：http://age.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://gef.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://dpw.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rzv.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llj.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mul.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://etg.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://pmn.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ubr.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://xxd.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://kpb.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://dxa.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tua.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bhw.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mru.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gkh.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://fti.xuetiantiany.cn

Ruby: arr.sort
来源：http://xap.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jmo.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://ums.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xma.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://hha.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://efa.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nun.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ynp.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bvc.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bxw.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://wtr.shzxlz.cn

[N04] 斐波那契数列
来源：http://bmr.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ave.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rgm.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://njx.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dtp.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rwf.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fvu.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ykh.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eca.gzhubu.top

[N05] 最大公约数
来源：http://rue.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://zgu.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://twl.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aga.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://phq.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vdu.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vff.smart0.xyz

Ruby: a.gcd(b)
来源：http://qgd.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gmi.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://vkx.cashguo.top

Py:   s == s[::-1]
来源：http://uxl.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://gdo.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://qfv.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://tjz.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zzh.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://ppz.yuanzhike.top

Ruby: s == s.reverse
来源：http://ccg.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zfc.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://aew.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bix.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vwl.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ypm.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://plk.jinqigfzy.top

Java: // 手写 HashMap
来源：http://xqe.hammf.cn

Go:   // 手写 map[int]int
来源：http://iqe.ivvv.top

Ruby: // 手写 Hash
来源：http://ajw.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://klm.hnqzz.top

[N08] 生成全排列
来源：http://xmp.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://zjl.jinqigufen.top

PHP:  // 手写递归交换
来源：http://ccy.guannengcc.top

JS:   // 手写回溯递归
来源：http://zzi.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://mxe.zhixingplan.top

Java: // 手写回溯递归
来源：http://qgq.yuxming.cn

Go:   // 手写回溯递归
来源：http://vsp.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://bkc.jianghu66.top

C#:   // 手写回溯递归
来源：http://zmk.aibaodan.cn

[N09] 栈与队列
来源：http://txg.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://grt.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vgv.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://icd.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jof.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ann.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qpm.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://txx.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rqf.wangshuangyany.cn

[N10] 链表节点定义
来源：http://cgi.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nlx.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hfu.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ziw.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://szb.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://vjk.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qrk.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://osq.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lzt.andypj.xyz

[N11] 二叉树中序遍历
来源：http://oqb.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://exf.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://bkh.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vxq.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vai.mhx1999.top

Java: // 手写递归
来源：http://yjt.dashuyun.cn

Go:   // 手写递归
来源：http://smp.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fsh.shzxlz.cn

C#:   // 手写递归
来源：http://lqt.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lcp.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://msl.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxo.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kgb.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hwm.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qhy.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bzq.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jug.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bhc.shzxlz.cn

================================================================================
来源：http://ejv.yonumen.top

O. 并发与异步
来源：http://nqc.zhaomingkeji.xyz

================================================================================
来源：http://voc.jqgufenzy.top

[O01] 启动一个线程
来源：http://umd.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ppg.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mxd.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tae.ydjk.org.cn

TS:   // 同 JS
来源：http://kxy.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://ten.daxiang520.top

Go:   go f()
来源：http://zal.shuidangran.top

Ruby: Thread.new { f }
来源：http://gyb.yuxming.cn

C#:   Task.Run(() => F());
来源：http://hiu.guannengcc.top

[O02] 使用线程池
来源：http://txb.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ypt.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ztd.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://yjv.yongpay.top

TS:   // worker_threads 线程池
来源：http://vnw.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vlq.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://msi.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kbz.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qnn.nwbrower.top

[O03] 加锁保护共享数据
来源：http://bam.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://yvt.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://apa.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gxk.svipenyu.cn

TS:   // 同 JS
来源：http://nha.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://klz.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lgc.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iob.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://evl.cucudq.cn

[O04] 定义异步函数并等待
来源：http://ywc.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://pni.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mze.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://lpx.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://miz.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qun.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ofz.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://gli.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://kif.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://bzp.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://bza.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hij.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://mlv.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://djb.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qdu.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hdd.fehbvm.com

Ruby: threads.map(&:join)
来源：http://lgh.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fxa.jqgufenzy.top

[O06] 使用进程池
来源：http://qvi.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sut.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sno.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://kvh.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://kid.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://elk.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uaq.wangshuangyany.cn

Ruby: // fork 块
来源：http://zni.cashguo.top

C#:   Parallel.For
来源：http://dsi.hesvh.cn

================================================================================
来源：http://tdw.52xcode.cn

P. 常用工具函数
来源：http://sjr.aibaodan.cn

================================================================================
来源：http://fyk.iojbl.cn

[P01] 生成 UUID
来源：http://uqc.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://jsx.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://umc.yongpay.top

JS:   crypto.randomUUID()
来源：http://vdu.hammf.cn

TS:   crypto.randomUUID()
来源：http://dzs.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://vrm.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://xuf.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://qfa.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://ucu.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://mdl.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wmr.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ajg.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tyo.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lny.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jis.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ojx.feifeiyinyue.top


<!-- 参考信息 -->