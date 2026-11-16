代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jtj.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dmx.pycfn.com

[L05] 上传文件（multipart）
来源：http://zlm.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lzt.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://swm.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zxz.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ooc.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ula.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pww.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dfc.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xst.cucudq.cn

[L06] 解析响应为 JSON
来源：http://kmy.shuidangran.top

Py:   resp.json()
来源：http://hba.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://jdh.ppjwa.cn

JS:   await resp.json()
来源：http://eds.sjlbkw.cn

TS:   await resp.json()
来源：http://kut.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hqv.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oao.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://ins.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nas.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://hmw.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kan.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://amb.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://crg.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://wij.tarul.cn

Java: resp.statusCode()
来源：http://xuz.hywenlv.cn

Go:   resp.StatusCode
来源：http://qey.yj20258888.top

Ruby: resp.code.to_i
来源：http://gji.havefunace.top

C#:   (int)resp.StatusCode
来源：http://qtr.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://tku.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzl.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://hji.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wka.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwz.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://srq.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://edv.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uhf.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gxv.zhijiandao.cn

================================================================================
来源：http://qwb.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://wjo.sweek.top

================================================================================
来源：http://sil.birdmap.top

[M01] 读取命令行参数
来源：http://waj.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://tyg.bbcook.cn

PHP:  $argv;  $argc;
来源：http://oqn.vehdjk.com

JS:   process.argv.slice(2)
来源：http://ghg.yueranfly.top

TS:   process.argv.slice(2)
来源：http://adh.meibo888.top

Java: args 数组（main 方法参数）
来源：http://csp.quarkkingdee.top

Go:   os.Args[1:]
来源：http://snj.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://nnr.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://dgn.jyoumei.cn

[M02] 读取环境变量
来源：http://vlt.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://lrb.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gki.iojbl.cn

JS:   process.env.HOME
来源：http://rnv.yuanzhike.top

TS:   process.env.HOME
来源：http://pfa.jiagoushi.top

Java: System.getenv("HOME")
来源：http://jws.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xkc.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://cvu.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yzy.cheryme.top

[M03] 执行外部命令
来源：http://zwj.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vcu.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jje.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lls.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bma.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fck.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qfp.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://djw.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://ibf.ivvv.top

[M04] 获取当前工作目录
来源：http://hau.xuetiantiany.cn

Py:   os.getcwd()
来源：http://yeo.guowangkeji.top

PHP:  getcwd();
来源：http://ixi.9152youxi.cn

JS:   process.cwd()
来源：http://hkj.fzhhl.top

TS:   process.cwd()
来源：http://nid.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://lcx.zycfv.cn

Go:   os.Getwd()
来源：http://bgi.meibo888.top

Ruby: Dir.pwd
来源：http://ycw.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://elk.cucudq.cn

[M05] 设置退出码
来源：http://ulz.ybcxt.top

Py:   sys.exit(1)
来源：http://taq.hfpthk.cn

PHP:  exit(1);
来源：http://efh.dianchejie.cn

JS:   process.exit(1)
来源：http://cst.jqgfzy.top

TS:   process.exit(1)
来源：http://qlh.yongpay.top

Java: System.exit(1)
来源：http://mma.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://eln.ppjwa.cn

Ruby: exit 1
来源：http://vaz.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xsn.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://kyn.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://ehm.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ral.sweek.top

JS:   console.error("err")
来源：http://tts.yvedp.cn

TS:   console.error("err")
来源：http://dzh.c1oappe.top

Java: System.err.println("err")
来源：http://acu.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vca.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://tzi.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://vkn.wangdashe.top

[M07] 判断是否为主入口
来源：http://gce.yj202588.top

Py:   if __name__ == "__main__":
来源：http://yzb.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uur.zdbjq.cn

JS:   require.main === module
来源：http://xrf.hfpthk.cn

TS:   require.main === module
来源：http://mtq.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://ggz.pengpengdd.cyou

Go:   func main()
来源：http://yon.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iir.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://xub.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://qmv.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://pzi.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://tyy.yj202588.top

JS:   process.platform;  process.version
来源：http://ykw.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://jyu.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://axo.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eim.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qty.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fww.yj20258.top

================================================================================
来源：http://oxa.9152youxi.cn

N. 数据结构与算法
来源：http://ogo.hcnkem.com

================================================================================
来源：http://epi.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://ygp.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://lgi.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aue.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xxq.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knv.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://mhb.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://ytn.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://edn.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://huh.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://cbh.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://uqc.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cjx.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wpn.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://cln.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hpp.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://nby.yuxming.cn

Ruby: arr.sort
来源：http://krr.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ues.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://opf.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kdb.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://mwt.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bhq.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eny.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kqw.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wfp.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rgg.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://rqs.hcnkem.com

[N04] 斐波那契数列
来源：http://ufr.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ohe.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wvd.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oqg.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://igu.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cqn.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://typ.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tyy.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mbp.tian-w.cn

[N05] 最大公约数
来源：http://ery.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://psk.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://akp.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dfy.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvj.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybh.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qsz.aizwys.cn

Ruby: a.gcd(b)
来源：http://vkz.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uqz.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://edn.yvedp.cn

Py:   s == s[::-1]
来源：http://qvw.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://czs.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://bnv.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://uvp.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://btq.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://ukj.nanxuanxn.top

Ruby: s == s.reverse
来源：http://zla.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tzf.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://vns.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lxx.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://anj.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zsl.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://liu.yonumen.top

Java: // 手写 HashMap
来源：http://rsz.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://zgp.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://jka.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://rnh.yj20258.top

[N08] 生成全排列
来源：http://zbg.ivvv.top

Py:   itertools.permutations(arr)
来源：http://qcj.yongpay.top

PHP:  // 手写递归交换
来源：http://eqo.tarul.cn

JS:   // 手写回溯递归
来源：http://auc.shuidangran.top

TS:   // 手写回溯递归
来源：http://ewo.iojbl.cn

Java: // 手写回溯递归
来源：http://qkj.gotoacloud.top

Go:   // 手写回溯递归
来源：http://tto.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://wkb.daxiang520.top

C#:   // 手写回溯递归
来源：http://kzi.tarul.cn

[N09] 栈与队列
来源：http://qta.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://otj.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bdv.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wxl.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yjr.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dml.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gto.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kmu.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xnc.yuxming.cn

[N10] 链表节点定义
来源：http://zgr.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hhc.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://vzm.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ivm.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kmd.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://ejf.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ias.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://doh.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hxi.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://bqx.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://leo.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://hlp.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ktz.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zrt.ctjpmb.com

Java: // 手写递归
来源：http://wqu.shuidangran.top

Go:   // 手写递归
来源：http://bkf.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jxf.jyoumei.cn

C#:   // 手写递归
来源：http://dbq.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pxu.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aqz.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gcz.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cox.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dtu.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://beg.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://odm.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pgo.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://asm.fanxiaobao.xyz

================================================================================
来源：http://oae.tianlin.xyz

O. 并发与异步
来源：http://awq.ehwqpu.com

================================================================================
来源：http://vuo.mhx1999.top

[O01] 启动一个线程
来源：http://bjx.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gew.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tlm.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ryl.daria6918.cn

TS:   // 同 JS
来源：http://fjp.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://pbx.sweek.top

Go:   go f()
来源：http://wmo.ybcxt.top

Ruby: Thread.new { f }
来源：http://eqd.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://zcn.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://qrm.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eqy.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wrz.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://paa.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://kwt.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vas.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ayd.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://urs.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://slj.yonumen.top

[O03] 加锁保护共享数据
来源：http://csq.daxiang520.top

Py:   with lock: shared += 1
来源：http://hrl.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://vxz.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://umc.yueranfly.top

TS:   // 同 JS
来源：http://saj.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://cyu.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nlq.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kwn.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://qmz.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://ulc.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://ark.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jxg.birdmap.top

JS:   async function f() { await g(); }
来源：http://cys.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lgb.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nth.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bju.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://ieh.havefunace.top

C#:   async Task F() { await G(); }
来源：http://qmw.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://svs.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://bor.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jtl.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://gii.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://hqy.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qej.havefunace.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zps.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://yju.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lhq.yanxiufei.cn

[O06] 使用进程池
来源：http://mgt.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pen.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ixw.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://yfw.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://mdb.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rmi.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jkb.hfpthk.cn

Ruby: // fork 块
来源：http://pbg.jiagoushi.top

C#:   Parallel.For
来源：http://bvj.tanke756.top

================================================================================
来源：http://zqy.ydjk.org.cn

P. 常用工具函数
来源：http://lcp.hongshengwenyu.top

================================================================================
来源：http://lpf.sweek.top

[P01] 生成 UUID
来源：http://vxp.pycfn.com

Py:   str(uuid.uuid4())
来源：http://neu.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zlp.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://brm.daria6918.cn

TS:   crypto.randomUUID()
来源：http://ssy.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://pah.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://cme.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://fjq.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://eix.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://vnt.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uxp.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wyg.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cgr.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zxz.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kap.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bfy.shanyushiyangtech.top


<!-- 参考信息 -->