代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bfx.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qod.tanke756.top

[L05] 上传文件（multipart）
来源：http://ehx.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://riu.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qml.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kri.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vkx.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pij.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dgn.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://heb.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nry.yj20258888.top

[L06] 解析响应为 JSON
来源：http://yqt.wangdashe.top

Py:   resp.json()
来源：http://aqs.vehdjk.com

PHP:  json_decode($body, true);
来源：http://heh.dashuyun.cn

JS:   await resp.json()
来源：http://mhm.sysykeji.top

TS:   await resp.json()
来源：http://lxn.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pcq.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zzj.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://jkl.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gdz.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://rtt.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eoj.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://itu.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://bny.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://kkq.yfazqb.com

Java: resp.statusCode()
来源：http://okv.jyoumei.cn

Go:   resp.StatusCode
来源：http://nrq.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://sei.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://knz.gogol.net.cn

[L08] 并发请求多个地址
来源：http://txw.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ccx.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://lwv.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zod.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gmj.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wto.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bgx.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://okn.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://agi.fehbvm.com

================================================================================
来源：http://wzd.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://lbw.fengsongda.top

================================================================================
来源：http://ynm.yongpay.top

[M01] 读取命令行参数
来源：http://esb.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://fzi.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://rtf.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://hgy.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://wrs.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://xum.nanxuanxn.top

Go:   os.Args[1:]
来源：http://clv.sjlbkw.cn

Ruby: ARGV
来源：http://scv.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://whb.vqdsnc.cn

[M02] 读取环境变量
来源：http://krn.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://czp.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mtl.ivvv.top

JS:   process.env.HOME
来源：http://ubf.gzhubu.top

TS:   process.env.HOME
来源：http://agv.hywenlv.cn

Java: System.getenv("HOME")
来源：http://lji.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dku.epnwcf.com

Ruby: ENV["HOME"]
来源：http://isf.tarul.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dks.quarkkingdee.top

[M03] 执行外部命令
来源：http://klz.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nmv.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://niq.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gkj.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iko.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bgm.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kbx.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://kty.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://cip.cqqwz.cn

[M04] 获取当前工作目录
来源：http://qta.yj202588.top

Py:   os.getcwd()
来源：http://aum.sweek.top

PHP:  getcwd();
来源：http://wxi.ydzc1.top

JS:   process.cwd()
来源：http://kfs.birdmap.top

TS:   process.cwd()
来源：http://khp.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://mmj.quarkkingdee.top

Go:   os.Getwd()
来源：http://snq.0kj1m.cn

Ruby: Dir.pwd
来源：http://pka.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vsn.yj20258.top

[M05] 设置退出码
来源：http://iwc.cheryme.top

Py:   sys.exit(1)
来源：http://erl.daria6918.cn

PHP:  exit(1);
来源：http://cwx.0kj1m.cn

JS:   process.exit(1)
来源：http://lai.pycfn.com

TS:   process.exit(1)
来源：http://zxm.zhongyouzk.top

Java: System.exit(1)
来源：http://lrr.birdmap.top

Go:   os.Exit(1)
来源：http://edw.ppjwa.cn

Ruby: exit 1
来源：http://ybr.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lur.sysykeji.top

[M06] 向标准错误输出
来源：http://xwd.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://chg.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ieh.jqgufenzy.top

JS:   console.error("err")
来源：http://swi.tianlin.xyz

TS:   console.error("err")
来源：http://vkj.daxiang520.top

Java: System.err.println("err")
来源：http://zco.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cek.shangyingyoupin.top

Ruby: warn "err"
来源：http://otu.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://jlk.smart0.xyz

[M07] 判断是否为主入口
来源：http://gbw.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://kmx.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mjf.jiagoushi.top

JS:   require.main === module
来源：http://bua.shuidangran.top

TS:   require.main === module
来源：http://qhl.daria6918.cn

Java: public static void main(String[] args)
来源：http://ywu.xuanzx.com

Go:   func main()
来源：http://hzw.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gez.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://cep.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://wsg.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://kpx.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://bze.jianghu66.top

JS:   process.platform;  process.version
来源：http://uvy.birdmap.top

TS:   process.platform;  process.version
来源：http://kyu.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ylb.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://oro.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lrr.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmt.yj20258888.top

================================================================================
来源：http://ucb.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://int.wangdashe.top

================================================================================
来源：http://idy.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://tdt.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://ikk.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cpt.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vyr.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://znv.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://qdd.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://fex.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eyc.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://cxf.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://uqm.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://dge.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nxk.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zqh.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ruy.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aws.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://zew.svipenyu.cn

Ruby: arr.sort
来源：http://jis.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ahd.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://scd.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dfj.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://sqi.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uae.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ark.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://urp.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ils.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uyr.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://dtx.jianghu66.top

[N04] 斐波那契数列
来源：http://yxj.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sgg.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://egx.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://die.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wya.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nwv.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ohk.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tym.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://abg.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://cty.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://ycl.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gfe.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swd.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gor.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xna.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ugs.tian-w.cn

Ruby: a.gcd(b)
来源：http://pnq.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dzs.fehbvm.com

[N06] 判断回文字符串
来源：http://iqd.svipenyu.cn

Py:   s == s[::-1]
来源：http://zui.xziqi.cn

PHP:  $s === strrev($s);
来源：http://dfx.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://afs.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://pbh.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kiz.fengsongda.top

Go:   // 双指针从两端比较
来源：http://cnl.jinqigfzy.top

Ruby: s == s.reverse
来源：http://rxa.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xib.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://piw.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iub.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dby.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://yan.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://egd.havefunace.top

Java: // 手写 HashMap
来源：http://rxi.redwolf501.top

Go:   // 手写 map[int]int
来源：http://png.chenzaomai.com

Ruby: // 手写 Hash
来源：http://tkk.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://mqf.feifeiyinyue.top

[N08] 生成全排列
来源：http://tqk.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://lgs.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://ohu.yj20258888.top

JS:   // 手写回溯递归
来源：http://rcx.shzxlz.cn

TS:   // 手写回溯递归
来源：http://iyw.jiagoushi.top

Java: // 手写回溯递归
来源：http://kpc.yonumen.top

Go:   // 手写回溯递归
来源：http://nty.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://xbz.daxiang520.top

C#:   // 手写回溯递归
来源：http://ivm.c1oappe.top

[N09] 栈与队列
来源：http://deu.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jbc.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gzo.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tlu.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zjj.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iaq.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://idu.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fnc.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://clm.zhoulong.xyz

[N10] 链表节点定义
来源：http://ytc.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pgw.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gje.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wqh.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dqo.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://nif.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://mho.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://yff.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cfu.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://gpg.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dbw.zycfv.cn

PHP:  // 手写递归函数
来源：http://xmh.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rks.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jrq.chenzaomai.com

Java: // 手写递归
来源：http://bqs.ydjk.org.cn

Go:   // 手写递归
来源：http://fkc.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pbj.tanke756.top

C#:   // 手写递归
来源：http://bwy.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://req.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rel.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wcb.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rbv.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yyl.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dkg.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ysj.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cug.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pkz.chenjidiqi.icu

================================================================================
来源：http://ylc.hesvh.cn

O. 并发与异步
来源：http://ffr.yongpay.top

================================================================================
来源：http://zaz.gaohongyu789.top

[O01] 启动一个线程
来源：http://qvg.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xsw.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cou.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ied.ydzc1.top

TS:   // 同 JS
来源：http://xuk.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://kjr.mhx1999.top

Go:   go f()
来源：http://muc.zhixingplan.top

Ruby: Thread.new { f }
来源：http://jvk.yj202588.top

C#:   Task.Run(() => F());
来源：http://xch.jinqigufen.top

[O02] 使用线程池
来源：http://gqc.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjw.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ilu.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://fpe.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://vua.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://oox.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kce.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cjt.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iot.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://kgb.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://hco.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://ved.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lwn.316326.xyz

TS:   // 同 JS
来源：http://ujj.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://ops.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fpn.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hwj.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://ijh.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://gkl.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://sxk.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://trf.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://ipt.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jrc.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zij.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mmq.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qle.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://zts.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://kkv.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://cbv.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tvw.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://qea.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://yxz.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wnk.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bnh.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://jfi.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fft.meibo888.top

[O06] 使用进程池
来源：http://mtg.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nkf.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://awz.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://veg.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://lem.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://thc.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://axp.sxryk.cn

Ruby: // fork 块
来源：http://mkj.yangfankeji.com

C#:   Parallel.For
来源：http://mmh.shangyingyoupin.top

================================================================================
来源：http://zrm.kuanghao11.cn

P. 常用工具函数
来源：http://lve.pengpengdd.cyou

================================================================================
来源：http://lxv.bbcook.cn

[P01] 生成 UUID
来源：http://lxe.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://tds.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hcp.fzhhl.top

JS:   crypto.randomUUID()
来源：http://yjd.tarul.cn

TS:   crypto.randomUUID()
来源：http://wtq.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://lgd.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://lsr.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://zid.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://sks.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://rwm.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ell.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ndr.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xbo.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tqg.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ogk.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ntd.ehwqpu.com


<!-- 参考信息 -->