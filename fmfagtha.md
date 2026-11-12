代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjh.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vco.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eew.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://msq.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lle.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mwv.tanke756.top

[L05] 上传文件（multipart）
来源：http://buu.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlu.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jdi.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ear.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lrd.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://irw.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vuy.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lah.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uga.uphjek.com

[L06] 解析响应为 JSON
来源：http://byt.hywenlv.cn

Py:   resp.json()
来源：http://fkg.nwbrower.top

PHP:  json_decode($body, true);
来源：http://sus.wangdashe.top

JS:   await resp.json()
来源：http://fvs.chenzaomai.com

TS:   await resp.json()
来源：http://lkb.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gbx.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aqx.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://lgz.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kjd.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://giw.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dqc.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eyp.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://sho.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://qaa.hnxiangtu.top

Java: resp.statusCode()
来源：http://zqx.sweek.top

Go:   resp.StatusCode
来源：http://xgq.havefunace.top

Ruby: resp.code.to_i
来源：http://vrc.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://nad.fzhhl.top

[L08] 并发请求多个地址
来源：http://nzb.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zhu.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://utd.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfu.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xkk.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dns.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://szk.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cjp.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qis.ydjk.org.cn

================================================================================
来源：http://hiv.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://dyp.shzxlz.cn

================================================================================
来源：http://bbh.nwbrower.top

[M01] 读取命令行参数
来源：http://dog.havefunace.top

Py:   sys.argv[1:]
来源：http://kgu.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://ayi.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://jei.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://opo.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://oco.hammf.cn

Go:   os.Args[1:]
来源：http://ttd.c1oappe.top

Ruby: ARGV
来源：http://tiu.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://pmt.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://igv.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://xqr.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mmw.yj20258888.top

JS:   process.env.HOME
来源：http://ytm.svipenyu.cn

TS:   process.env.HOME
来源：http://uri.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://bsv.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bjl.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://tkn.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pak.ydzc1.top

[M03] 执行外部命令
来源：http://tbs.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ipo.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zyq.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://caa.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mwv.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fnj.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uys.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://czk.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ehv.gotoacloud.top

[M04] 获取当前工作目录
来源：http://srs.fzhhl.top

Py:   os.getcwd()
来源：http://qdb.bbcook.cn

PHP:  getcwd();
来源：http://jcn.chenlongwang.top

JS:   process.cwd()
来源：http://ljw.zdbjq.cn

TS:   process.cwd()
来源：http://pct.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://lii.chenjidiqi.icu

Go:   os.Getwd()
来源：http://ibw.guowangkeji.top

Ruby: Dir.pwd
来源：http://smz.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vgi.havefunace.top

[M05] 设置退出码
来源：http://lqj.yvedp.cn

Py:   sys.exit(1)
来源：http://pwf.daria6918.cn

PHP:  exit(1);
来源：http://cyv.jyoumei.cn

JS:   process.exit(1)
来源：http://gfu.ydjk.org.cn

TS:   process.exit(1)
来源：http://wrx.yonumen.top

Java: System.exit(1)
来源：http://jro.yangfankeji.com

Go:   os.Exit(1)
来源：http://mvl.9152youxi.cn

Ruby: exit 1
来源：http://olc.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eqs.cheryme.top

[M06] 向标准错误输出
来源：http://lbm.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://rkp.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wyb.daria6918.cn

JS:   console.error("err")
来源：http://abn.yongpay.top

TS:   console.error("err")
来源：http://bks.zhijiandao.cn

Java: System.err.println("err")
来源：http://czj.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://maw.daxiang520.top

Ruby: warn "err"
来源：http://bdl.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://uum.havefunace.top

[M07] 判断是否为主入口
来源：http://svc.yongpay.top

Py:   if __name__ == "__main__":
来源：http://ksw.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xsw.9152youxi.cn

JS:   require.main === module
来源：http://muv.ppjwa.cn

TS:   require.main === module
来源：http://rcu.fengsongda.top

Java: public static void main(String[] args)
来源：http://kwq.hcnkem.com

Go:   func main()
来源：http://xoi.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sfh.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://trj.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://foy.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://csy.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://nji.ppjwa.cn

JS:   process.platform;  process.version
来源：http://fvn.zhengqikj.top

TS:   process.platform;  process.version
来源：http://zjj.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hky.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jvk.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qum.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://odp.xuanzx.com

================================================================================
来源：http://zus.yuxming.cn

N. 数据结构与算法
来源：http://lpv.ywan-chungtsiang.top

================================================================================
来源：http://ryt.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://ozh.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kpg.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mnp.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dkt.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjl.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fxz.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://nuv.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykx.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kjv.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://yxb.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://uix.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wnp.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dzc.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ygf.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lnq.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://pyk.cqqwz.cn

Ruby: arr.sort
来源：http://auk.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qfb.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://edi.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qnx.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://mth.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sxh.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yta.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dsg.xingfuxueyuan.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hxa.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://smq.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://glt.meibo888.top

[N04] 斐波那契数列
来源：http://usx.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jsj.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vdv.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ecd.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hwh.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qwk.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jtv.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hup.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vni.birdmap.top

[N05] 最大公约数
来源：http://ouy.xylfe.cn

Py:   math.gcd(a, b)
来源：http://cma.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kvr.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcf.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zrt.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyr.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ldy.gogol.net.cn

Ruby: a.gcd(b)
来源：http://lxi.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ari.tianlin.xyz

[N06] 判断回文字符串
来源：http://dlh.redwolf501.top

Py:   s == s[::-1]
来源：http://huo.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://fpj.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://nzj.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://lwy.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xgn.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://rhu.fzhhl.top

Ruby: s == s.reverse
来源：http://dri.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ydz.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://xaa.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ooz.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kdp.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://htt.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://sdk.havefunace.top

Java: // 手写 HashMap
来源：http://isg.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://nlm.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://qay.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://dbn.gotoacloud.top

[N08] 生成全排列
来源：http://znp.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://wch.guowangkeji.top

PHP:  // 手写递归交换
来源：http://zub.gotoacloud.top

JS:   // 手写回溯递归
来源：http://xcu.yonumen.top

TS:   // 手写回溯递归
来源：http://uqt.jinqigfzy.top

Java: // 手写回溯递归
来源：http://xra.yonumen.top

Go:   // 手写回溯递归
来源：http://eid.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://udq.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://ocg.xziqi.cn

[N09] 栈与队列
来源：http://zit.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hsa.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wtv.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://asm.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tys.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sgl.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yxq.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zba.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://srs.bbcook.cn

[N10] 链表节点定义
来源：http://avr.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rsv.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://fyx.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ebx.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jwx.yj20258.top

Java: class Node { int v; Node next; }
来源：http://ext.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wsv.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://tiv.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qvb.wangdashe.top

[N11] 二叉树中序遍历
来源：http://czx.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uib.sysykeji.top

PHP:  // 手写递归函数
来源：http://hta.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ong.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbn.hysaishi.cn

Java: // 手写递归
来源：http://tuc.zhiwuduotai.top

Go:   // 手写递归
来源：http://znm.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://exf.shanyushiyangtech.top

C#:   // 手写递归
来源：http://pyh.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rlf.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dht.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fxn.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjl.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnk.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vkp.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eer.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zdu.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ytw.c1oappe.top

================================================================================
来源：http://ppt.zhoulong.xyz

O. 并发与异步
来源：http://hww.fktsv.cn

================================================================================
来源：http://guy.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://rwo.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lvn.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zyx.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qec.zdqjudy.top

TS:   // 同 JS
来源：http://jvp.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://jhj.epnwcf.com

Go:   go f()
来源：http://fhm.zdbjq.cn

Ruby: Thread.new { f }
来源：http://gns.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://nly.uphjek.com

[O02] 使用线程池
来源：http://qgu.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oon.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wxt.sysykeji.top

JS:   // worker_threads 线程池
来源：http://gcg.yvedp.cn

TS:   // worker_threads 线程池
来源：http://pvg.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://drv.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qbg.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cik.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cqp.tanke756.top

[O03] 加锁保护共享数据
来源：http://jtj.sxryk.cn

Py:   with lock: shared += 1
来源：http://opk.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://umr.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bnk.yueranfly.top

TS:   // 同 JS
来源：http://cqo.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://cyh.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fqs.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mll.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://jpr.hesvh.cn

[O04] 定义异步函数并等待
来源：http://fjs.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://gds.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kwb.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://wcv.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://pni.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vyh.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qlp.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xft.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://jxb.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://lwg.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://lvh.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xvl.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://nie.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://xjp.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ryz.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qrp.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://hpq.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dri.yongpay.top

[O06] 使用进程池
来源：http://qye.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ypf.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://eiv.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://kow.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://dvp.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gpg.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xyt.snrcjt.cn

Ruby: // fork 块
来源：http://tna.fktsv.cn

C#:   Parallel.For
来源：http://xfy.sjlbkw.cn

================================================================================
来源：http://dxe.zhongyouzk.top

P. 常用工具函数
来源：http://mqw.yuanzhike.top

================================================================================
来源：http://nqm.tanke756.top

[P01] 生成 UUID
来源：http://iud.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://ykw.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fnh.aizwys.cn

JS:   crypto.randomUUID()
来源：http://dwg.fehbvm.com

TS:   crypto.randomUUID()
来源：http://mcu.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://efo.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://mvj.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://rvd.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://gdf.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://clb.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zuz.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fps.ppjwa.cn


<!-- 参考信息 -->