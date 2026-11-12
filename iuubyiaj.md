代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://div.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://att.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rxf.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rdm.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tjk.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://chv.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ebj.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxh.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sum.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gch.yueranfly.top

[L06] 解析响应为 JSON
来源：http://xfk.sufxvd.cn

Py:   resp.json()
来源：http://tip.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://wwt.52xcode.cn

JS:   await resp.json()
来源：http://kbw.sufxvd.cn

TS:   await resp.json()
来源：http://fro.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mfx.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://axe.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://fll.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bbh.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://mfs.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nwr.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jwc.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://xld.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://xvo.pycfn.com

Java: resp.statusCode()
来源：http://prz.yvedp.cn

Go:   resp.StatusCode
来源：http://uea.zhengqikj.top

Ruby: resp.code.to_i
来源：http://chs.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://kyp.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://bqv.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oxu.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://qte.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unz.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmk.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vrd.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bna.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nyd.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://njq.iojbl.cn

================================================================================
来源：http://abu.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://que.chenzaomai.com

================================================================================
来源：http://yxw.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://pfv.ppjwa.cn

Py:   sys.argv[1:]
来源：http://raa.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://pxl.iojbl.cn

JS:   process.argv.slice(2)
来源：http://fwx.meibo888.top

TS:   process.argv.slice(2)
来源：http://wkp.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://the.hysaishi.cn

Go:   os.Args[1:]
来源：http://jfc.haohaochexian.top

Ruby: ARGV
来源：http://fqg.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://rfo.zhijiandao.cn

[M02] 读取环境变量
来源：http://gvx.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://sex.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mqa.aibaodan.cn

JS:   process.env.HOME
来源：http://ynd.cashguo.top

TS:   process.env.HOME
来源：http://tsc.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://xdx.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vsy.hcnkem.com

Ruby: ENV["HOME"]
来源：http://rtw.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fdb.dianchejie.cn

[M03] 执行外部命令
来源：http://qek.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kuq.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wkj.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zip.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iuu.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pbq.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xtn.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://qlo.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://pgb.guannengcc.top

[M04] 获取当前工作目录
来源：http://rxg.xziqi.cn

Py:   os.getcwd()
来源：http://jhr.fengsongda.top

PHP:  getcwd();
来源：http://dsl.yueranfly.top

JS:   process.cwd()
来源：http://hlw.cdnleiting.top

TS:   process.cwd()
来源：http://vsm.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://xxm.ydjk.org.cn

Go:   os.Getwd()
来源：http://nqy.jianghu66.top

Ruby: Dir.pwd
来源：http://yjf.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ear.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://hqf.yuanzhike.top

Py:   sys.exit(1)
来源：http://zcg.yfazqb.com

PHP:  exit(1);
来源：http://som.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://dzk.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://rpy.nwbrower.top

Java: System.exit(1)
来源：http://rdx.yj20258.top

Go:   os.Exit(1)
来源：http://ipk.epnwcf.com

Ruby: exit 1
来源：http://bxz.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xvk.yuanzhike.top

[M06] 向标准错误输出
来源：http://xmh.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://itp.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vfd.guannengcc.top

JS:   console.error("err")
来源：http://qss.zhengqikj.top

TS:   console.error("err")
来源：http://ncw.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://gnv.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kqb.fktsv.cn

Ruby: warn "err"
来源：http://pfl.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://dcs.birdmap.top

[M07] 判断是否为主入口
来源：http://gkz.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://qgb.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://usm.hammf.cn

JS:   require.main === module
来源：http://sci.shzxlz.cn

TS:   require.main === module
来源：http://uhs.ppjwa.cn

Java: public static void main(String[] args)
来源：http://nqu.bbcook.cn

Go:   func main()
来源：http://gbf.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ira.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://mmo.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://nju.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://wnz.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://lke.bjfxy.top

JS:   process.platform;  process.version
来源：http://jyk.cashguo.top

TS:   process.platform;  process.version
来源：http://qtt.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pnv.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vtc.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iih.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oiq.zhongyouzk.top

================================================================================
来源：http://wxf.sweek.top

N. 数据结构与算法
来源：http://xod.hongshengwenyu.top

================================================================================
来源：http://nrv.tarul.cn

[N01] 二分查找（有序数组）
来源：http://wzy.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pzk.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lvl.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ujw.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwo.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tvn.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://fft.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jbt.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://whl.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://uzm.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://cfd.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sgj.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://udh.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rss.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aji.sysykeji.top

Go:   slices.Sort(arr)
来源：http://xwm.sxryk.cn

Ruby: arr.sort
来源：http://gzv.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://asb.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://rrh.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://knk.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://lxr.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oht.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://glo.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dge.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uwf.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fdd.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://wjp.nwbrower.top

[N04] 斐波那契数列
来源：http://gog.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xfk.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qms.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wok.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpc.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hoq.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bkj.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxo.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nja.yj202588.top

[N05] 最大公约数
来源：http://zxx.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://riz.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ozz.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ofr.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ofa.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cbu.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://emp.fehbvm.com

Ruby: a.gcd(b)
来源：http://rts.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eby.cheryme.top

[N06] 判断回文字符串
来源：http://gcy.316326.xyz

Py:   s == s[::-1]
来源：http://zef.birdmap.top

PHP:  $s === strrev($s);
来源：http://mvg.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://vmp.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://skt.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bbl.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://uho.zhijiandao.cn

Ruby: s == s.reverse
来源：http://zxl.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ajx.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://ddj.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pdd.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gxg.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uww.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://bah.fzhhl.top

Java: // 手写 HashMap
来源：http://fbo.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://vgk.jinqigufen.top

Ruby: // 手写 Hash
来源：http://njq.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://wwx.gogol.net.cn

[N08] 生成全排列
来源：http://drz.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://byi.sxryk.cn

PHP:  // 手写递归交换
来源：http://fax.fktsv.cn

JS:   // 手写回溯递归
来源：http://ntx.hcnkem.com

TS:   // 手写回溯递归
来源：http://gzn.shuidangran.top

Java: // 手写回溯递归
来源：http://vzo.dianchejie.cn

Go:   // 手写回溯递归
来源：http://tza.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://rkp.cqqwz.cn

C#:   // 手写回溯递归
来源：http://uqq.daxiang520.top

[N09] 栈与队列
来源：http://okk.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sbk.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uug.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nrk.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://drw.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qnw.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bcx.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tzl.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zqr.cucudq.cn

[N10] 链表节点定义
来源：http://bbt.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bsm.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://ymh.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dqb.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cfy.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://mcz.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lic.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zww.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jxg.ydzc1.top

[N11] 二叉树中序遍历
来源：http://jql.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zfq.jiagoushi.top

PHP:  // 手写递归函数
来源：http://vdz.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgp.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gbn.fanxiaobao.xyz

Java: // 手写递归
来源：http://owe.xuetiantiany.cn

Go:   // 手写递归
来源：http://lxm.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tlc.jinqigfzy.top

C#:   // 手写递归
来源：http://vie.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bud.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yav.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kxo.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lnt.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kto.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://veq.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vtv.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pvf.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kqd.sxryk.cn

================================================================================
来源：http://qzu.jqgfzy.top

O. 并发与异步
来源：http://tjj.chenzaomai.com

================================================================================
来源：http://zog.uphjek.com

[O01] 启动一个线程
来源：http://pxx.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dcb.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ype.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bpu.fanxiaobao.xyz

TS:   // 同 JS
来源：http://ttd.iojbl.cn

Java: new Thread(() -> f()).start()
来源：http://tlc.ctjpmb.com

Go:   go f()
来源：http://tbi.yfazqb.com

Ruby: Thread.new { f }
来源：http://mat.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://rpe.havefunace.top

[O02] 使用线程池
来源：http://ekt.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://opn.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dom.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://has.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://zvu.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://een.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ttv.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bpe.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rcj.uphjek.com

[O03] 加锁保护共享数据
来源：http://prt.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://zxf.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://biq.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://npu.hysaishi.cn

TS:   // 同 JS
来源：http://qjh.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://tgt.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://liq.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aju.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://txa.fehbvm.com

[O04] 定义异步函数并等待
来源：http://btr.ivvv.top

Py:   async def f():⏎    await g()
来源：http://bpd.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://djf.tarul.cn

JS:   async function f() { await g(); }
来源：http://ehx.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aao.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bmr.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://get.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bxo.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://mea.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://fyb.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://alh.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wio.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://mom.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://ovg.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zgq.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wzj.fktsv.cn

Ruby: threads.map(&:join)
来源：http://ixr.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://evq.smart0.xyz

[O06] 使用进程池
来源：http://wms.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wxt.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mzf.yonumen.top

JS:   // child_process / cluster 模块
来源：http://wol.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://jpt.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rey.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dwe.hongshengwenyu.top

Ruby: // fork 块
来源：http://nuz.hammf.cn

C#:   Parallel.For
来源：http://bba.zdbjq.cn

================================================================================
来源：http://kgj.nwbrower.top

P. 常用工具函数
来源：http://eyt.yuanzhike.top

================================================================================
来源：http://rqy.hcnkem.com

[P01] 生成 UUID
来源：http://zjm.cheryme.top

Py:   str(uuid.uuid4())
来源：http://hsc.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sif.ivvv.top

JS:   crypto.randomUUID()
来源：http://dju.yfazqb.com

TS:   crypto.randomUUID()
来源：http://uzb.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://yea.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://mxf.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://wgr.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://jpk.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://uqk.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://coy.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xug.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aea.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wps.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://afs.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oeo.c1oappe.top


<!-- 参考信息 -->