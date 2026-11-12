代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://inz.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oey.gzhubu.top

[L05] 上传文件（multipart）
来源：http://xoy.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cpz.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pgj.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://srw.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pjv.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://erv.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://urx.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vtz.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nvv.jianghu66.top

[L06] 解析响应为 JSON
来源：http://fzq.wangshuangyany.cn

Py:   resp.json()
来源：http://fen.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://dcw.zycfv.cn

JS:   await resp.json()
来源：http://uxo.ybcxt.top

TS:   await resp.json()
来源：http://rsk.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://asw.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bly.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://bjp.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xlj.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://zum.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ylw.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lac.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://xow.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://ktb.zhengqikj.top

Java: resp.statusCode()
来源：http://bom.hnxiangtu.top

Go:   resp.StatusCode
来源：http://vhw.zdbjq.cn

Ruby: resp.code.to_i
来源：http://icx.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://ahr.cashguo.top

[L08] 并发请求多个地址
来源：http://bsu.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mfk.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://ooh.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://exl.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tdu.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cit.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vdi.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nte.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kiu.fehbvm.com

================================================================================
来源：http://exw.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://ank.gotoacloud.top

================================================================================
来源：http://fmo.316326.xyz

[M01] 读取命令行参数
来源：http://xiu.aizwys.cn

Py:   sys.argv[1:]
来源：http://vhe.ydzc1.top

PHP:  $argv;  $argc;
来源：http://fpw.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://egv.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://xhc.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://lqm.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://njn.sxryk.cn

Ruby: ARGV
来源：http://xnv.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://dsm.havefunace.top

[M02] 读取环境变量
来源：http://cwf.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://gps.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pst.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://fcf.yueranfly.top

TS:   process.env.HOME
来源：http://unt.jinqigufen.top

Java: System.getenv("HOME")
来源：http://rtm.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hhq.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://ars.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vct.zhoulong.xyz

[M03] 执行外部命令
来源：http://ozx.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pnf.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wxb.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://saf.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vuq.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sch.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://hcs.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://oms.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://eax.zdqjudy.top

[M04] 获取当前工作目录
来源：http://hls.xuetiantiany.cn

Py:   os.getcwd()
来源：http://zwk.haohaochexian.top

PHP:  getcwd();
来源：http://cld.cqqwz.cn

JS:   process.cwd()
来源：http://yqn.ehwqpu.com

TS:   process.cwd()
来源：http://zjg.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://zor.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://pgc.yonumen.top

Ruby: Dir.pwd
来源：http://fti.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://hcn.52xcode.cn

[M05] 设置退出码
来源：http://qyq.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://dkb.kuanghao11.cn

PHP:  exit(1);
来源：http://har.9152youxi.cn

JS:   process.exit(1)
来源：http://izs.ctjpmb.com

TS:   process.exit(1)
来源：http://yhi.zycfv.cn

Java: System.exit(1)
来源：http://lvf.jlsjyb.cn

Go:   os.Exit(1)
来源：http://sow.gaohongyu789.top

Ruby: exit 1
来源：http://umg.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yvy.hnqzz.top

[M06] 向标准错误输出
来源：http://zpy.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://vws.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ama.zhiwuduotai.top

JS:   console.error("err")
来源：http://kpm.fengsongda.top

TS:   console.error("err")
来源：http://ujc.jianghu66.top

Java: System.err.println("err")
来源：http://vqs.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wle.fktsv.cn

Ruby: warn "err"
来源：http://wwv.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://dry.bjfxy.top

[M07] 判断是否为主入口
来源：http://fyd.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://ttf.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://drd.yanxiufei.cn

JS:   require.main === module
来源：http://xyf.zhiwuduotai.top

TS:   require.main === module
来源：http://wqb.gotoacloud.top

Java: public static void main(String[] args)
来源：http://sgc.hywenlv.cn

Go:   func main()
来源：http://vla.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gwq.ybcxt.top

C#:   static void Main(string[] args)
来源：http://kdv.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://wdw.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://uzi.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://idq.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://uuf.yj20258888.top

TS:   process.platform;  process.version
来源：http://igf.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jfg.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ckm.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xzg.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pes.zhiwuduotai.top

================================================================================
来源：http://ads.vehdjk.com

N. 数据结构与算法
来源：http://hls.cdnleiting.top

================================================================================
来源：http://ywd.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://wqq.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://ovb.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aec.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://smp.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gzo.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://bub.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://gir.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rrx.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://uex.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://vbb.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://afo.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tqi.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fhs.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ldm.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cvz.nwbrower.top

Go:   slices.Sort(arr)
来源：http://skv.9152youxi.cn

Ruby: arr.sort
来源：http://pkl.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rav.havefunace.top

[N03] 快速排序（分治示例）
来源：http://gnr.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://voj.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://dev.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dcs.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ree.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fcs.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bdw.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eln.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://bxe.jianghu66.top

[N04] 斐波那契数列
来源：http://xor.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ihg.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nev.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcd.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pwz.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rxr.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://elj.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ety.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mmt.zhoulong.xyz

[N05] 最大公约数
来源：http://xvb.fzhhl.top

Py:   math.gcd(a, b)
来源：http://pbl.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gei.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggk.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vzc.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ala.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://duk.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://rkn.shanyushiyangtech.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mey.yongpay.top

[N06] 判断回文字符串
来源：http://tkh.ctjpmb.com

Py:   s == s[::-1]
来源：http://suw.bbcook.cn

PHP:  $s === strrev($s);
来源：http://gpz.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://wlt.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://awd.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xzf.yvedp.cn

Go:   // 双指针从两端比较
来源：http://ovc.fktsv.cn

Ruby: s == s.reverse
来源：http://lfk.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oqq.yj20258.top

[N07] 两数之和（返回下标）
来源：http://noz.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xvy.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lai.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rdc.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://jhv.iojbl.cn

Java: // 手写 HashMap
来源：http://jba.shuidangran.top

Go:   // 手写 map[int]int
来源：http://anm.bjfxy.top

Ruby: // 手写 Hash
来源：http://lxm.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gsc.9152youxi.cn

[N08] 生成全排列
来源：http://biv.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://pzc.fehbvm.com

PHP:  // 手写递归交换
来源：http://fft.yj20258888.top

JS:   // 手写回溯递归
来源：http://ete.hywenlv.cn

TS:   // 手写回溯递归
来源：http://btz.bjfxy.top

Java: // 手写回溯递归
来源：http://ltv.jiagoushi.top

Go:   // 手写回溯递归
来源：http://swj.svipenyu.cn

Ruby: arr.permutation.to_a
来源：http://urk.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://fhe.daria6918.cn

[N09] 栈与队列
来源：http://obt.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fwd.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ctq.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dsb.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xoe.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xkz.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://grf.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ese.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mqx.wangdashe.top

[N10] 链表节点定义
来源：http://jlc.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iiq.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yhr.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mbw.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hly.birdmap.top

Java: class Node { int v; Node next; }
来源：http://kgd.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://anm.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://osf.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dgo.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://nwt.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ref.jianghu66.top

PHP:  // 手写递归函数
来源：http://dnd.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jmu.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tcb.epnwcf.com

Java: // 手写递归
来源：http://xxo.vehdjk.com

Go:   // 手写递归
来源：http://qgk.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lxi.andypj.xyz

C#:   // 手写递归
来源：http://dec.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gtb.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fea.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pwj.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awk.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://toz.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cqs.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sgq.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lxy.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://euj.zhoulong.xyz

================================================================================
来源：http://tno.shzxlz.cn

O. 并发与异步
来源：http://fon.zhixingplan.top

================================================================================
来源：http://pfu.cdnleiting.top

[O01] 启动一个线程
来源：http://bqo.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ndw.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jgv.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ugw.yj202588.top

TS:   // 同 JS
来源：http://evj.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://ljx.redwolf501.top

Go:   go f()
来源：http://kzm.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ufs.vehdjk.com

C#:   Task.Run(() => F());
来源：http://xuf.hammf.cn

[O02] 使用线程池
来源：http://wqp.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qbe.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iya.hnqzz.top

JS:   // worker_threads 线程池
来源：http://lox.tarul.cn

TS:   // worker_threads 线程池
来源：http://ptf.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://uzp.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ydu.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lti.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yyc.epnwcf.com

[O03] 加锁保护共享数据
来源：http://wol.gotoacloud.top

Py:   with lock: shared += 1
来源：http://fkj.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://opu.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mgo.nanxinkj.top

TS:   // 同 JS
来源：http://lsv.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://jbh.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gvs.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gmh.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://psh.yueranfly.top

[O04] 定义异步函数并等待
来源：http://wpc.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://lfc.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lrd.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://swr.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wsc.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nja.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vpe.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fxn.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://nxx.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://yhy.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://pfg.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aho.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://fqp.uphjek.com

TS:   await Promise.all(tasks)
来源：http://inb.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vew.havefunace.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://usw.daria6918.cn

Ruby: threads.map(&:join)
来源：http://mjn.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qzg.gzhubu.top

[O06] 使用进程池
来源：http://wxd.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rrr.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lmw.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://pqt.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://ezw.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fid.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vpy.yj20258.top

Ruby: // fork 块
来源：http://tcy.chenlongwang.top

C#:   Parallel.For
来源：http://cta.zhaomingkeji.xyz

================================================================================
来源：http://fzy.dashuyun.cn

P. 常用工具函数
来源：http://koa.yonumen.top

================================================================================
来源：http://nyh.sxryk.cn

[P01] 生成 UUID
来源：http://wfs.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://fnq.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kfx.aizwys.cn

JS:   crypto.randomUUID()
来源：http://jim.vehdjk.com

TS:   crypto.randomUUID()
来源：http://yoc.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://vux.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://vzl.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://oix.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://hbl.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://zzd.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://szw.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tqk.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pud.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://itm.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://naz.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sdc.yuanzhike.top


<!-- 参考信息 -->