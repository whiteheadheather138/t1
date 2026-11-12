代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qkl.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gpj.zycfv.cn

[L05] 上传文件（multipart）
来源：http://nfh.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fej.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhy.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xoc.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://adq.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pec.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gkj.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xnq.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tra.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://lbg.shanyushiyangkeji.top

Py:   resp.json()
来源：http://cmw.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://ozb.wangdashe.top

JS:   await resp.json()
来源：http://guu.9152youxi.cn

TS:   await resp.json()
来源：http://bbj.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vvi.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tgn.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://tyi.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbz.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://mrz.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wcq.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://svc.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://cma.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://wkb.tarul.cn

Java: resp.statusCode()
来源：http://ygd.sjlbkw.cn

Go:   resp.StatusCode
来源：http://irr.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://guf.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://psw.guannengcc.top

[L08] 并发请求多个地址
来源：http://lze.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uwj.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://ngp.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yts.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://knk.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hai.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mmu.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ddb.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wkp.ehwqpu.com

================================================================================
来源：http://shi.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://iin.yvedp.cn

================================================================================
来源：http://nbk.yanxiufei.cn

[M01] 读取命令行参数
来源：http://jdj.hammf.cn

Py:   sys.argv[1:]
来源：http://stb.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://vhy.yj20258888.top

JS:   process.argv.slice(2)
来源：http://xlh.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://cnt.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://vvf.jinqigfzy.top

Go:   os.Args[1:]
来源：http://ycn.hcnkem.com

Ruby: ARGV
来源：http://grz.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://boj.9152youxi.cn

[M02] 读取环境变量
来源：http://emb.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://wct.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gdi.ehwqpu.com

JS:   process.env.HOME
来源：http://buw.yueranfly.top

TS:   process.env.HOME
来源：http://enj.vehdjk.com

Java: System.getenv("HOME")
来源：http://ejd.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cte.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://zuf.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zdx.svipenyu.cn

[M03] 执行外部命令
来源：http://fgj.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://svk.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jyr.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://blf.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bzd.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aap.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hkp.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ije.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://nkc.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://dox.wangdashe.top

Py:   os.getcwd()
来源：http://erv.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://obc.bbcook.cn

JS:   process.cwd()
来源：http://fzr.shanyushiyangtech.top

TS:   process.cwd()
来源：http://bgg.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://mkk.fengsongda.top

Go:   os.Getwd()
来源：http://pla.vqdsnc.cn

Ruby: Dir.pwd
来源：http://jkp.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mbd.cashguo.top

[M05] 设置退出码
来源：http://nar.jinqigfzy.top

Py:   sys.exit(1)
来源：http://ueb.ehwqpu.com

PHP:  exit(1);
来源：http://evk.cashguo.top

JS:   process.exit(1)
来源：http://ptu.ppjwa.cn

TS:   process.exit(1)
来源：http://wxz.pycfn.com

Java: System.exit(1)
来源：http://xmb.tarul.cn

Go:   os.Exit(1)
来源：http://gpw.jiagoushi.top

Ruby: exit 1
来源：http://man.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yfy.xylfe.cn

[M06] 向标准错误输出
来源：http://kni.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://lvz.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rck.xinyue.icu

JS:   console.error("err")
来源：http://dla.shuidangran.top

TS:   console.error("err")
来源：http://zps.hysaishi.cn

Java: System.err.println("err")
来源：http://qfo.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ejp.redwolf501.top

Ruby: warn "err"
来源：http://wbv.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://uza.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://abc.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://hgo.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgg.ywan-chungtsiang.top

JS:   require.main === module
来源：http://rfb.shangyingyoupin.top

TS:   require.main === module
来源：http://yjh.ybcxt.top

Java: public static void main(String[] args)
来源：http://zga.jyoumei.cn

Go:   func main()
来源：http://kks.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://czd.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://bcx.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://rtz.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://ihs.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://tqu.yuanzhike.top

JS:   process.platform;  process.version
来源：http://ivn.hysaishi.cn

TS:   process.platform;  process.version
来源：http://ydv.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ukd.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ier.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bkm.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wrf.redwolf501.top

================================================================================
来源：http://yew.chenjidiqi.icu

N. 数据结构与算法
来源：http://mek.zhijiandao.cn

================================================================================
来源：http://txj.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://aym.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ays.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tpd.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gmo.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mfw.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jwp.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://cqv.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dar.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ziu.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://oma.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://bud.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dvr.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://giq.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dhq.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xkx.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://idg.yuxming.cn

Ruby: arr.sort
来源：http://xfm.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uig.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://zky.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qzv.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://mhk.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ybc.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://acy.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tvp.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bvh.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uub.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://kex.zhixingplan.top

[N04] 斐波那契数列
来源：http://ivy.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zua.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ysz.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdi.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://edh.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kxa.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gzh.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://skh.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hdj.zhoulong.xyz

[N05] 最大公约数
来源：http://edw.havefunace.top

Py:   math.gcd(a, b)
来源：http://dfb.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://usp.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://spt.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jmt.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://buv.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ayx.ehwqpu.com

Ruby: a.gcd(b)
来源：http://geo.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yjt.yuanzhike.top

[N06] 判断回文字符串
来源：http://tea.yj20258888.top

Py:   s == s[::-1]
来源：http://xym.gzhubu.top

PHP:  $s === strrev($s);
来源：http://azd.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://bkt.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://ljy.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://env.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://lex.gotoacloud.top

Ruby: s == s.reverse
来源：http://kpn.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rfj.hammf.cn

[N07] 两数之和（返回下标）
来源：http://xtb.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iqz.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xnx.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://upn.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://zgz.havefunace.top

Java: // 手写 HashMap
来源：http://ekn.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://fre.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://wzu.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://loi.gzhubu.top

[N08] 生成全排列
来源：http://ddp.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://pjn.epnwcf.com

PHP:  // 手写递归交换
来源：http://noc.fehbvm.com

JS:   // 手写回溯递归
来源：http://oyh.cqqwz.cn

TS:   // 手写回溯递归
来源：http://mge.yanxiufei.cn

Java: // 手写回溯递归
来源：http://jud.xylfe.cn

Go:   // 手写回溯递归
来源：http://owv.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://saw.pycfn.com

C#:   // 手写回溯递归
来源：http://ile.yueranfly.top

[N09] 栈与队列
来源：http://nzf.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xwy.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bxw.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eha.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dna.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cfj.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zzo.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rya.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ohu.0kj1m.cn

[N10] 链表节点定义
来源：http://aqg.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsj.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://olk.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oir.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ent.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://pif.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://ahk.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bav.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lap.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://brq.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pxz.uphjek.com

PHP:  // 手写递归函数
来源：http://nbr.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lsa.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nvx.xuanzx.com

Java: // 手写递归
来源：http://ucd.jqgufenzy.top

Go:   // 手写递归
来源：http://pap.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ozg.hongshengwenyu.top

C#:   // 手写递归
来源：http://fvr.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mxt.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xdr.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vvc.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aou.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxx.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uyk.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gns.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://knb.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fjk.iojbl.cn

================================================================================
来源：http://alk.xinyue.icu

O. 并发与异步
来源：http://lax.bjfxy.top

================================================================================
来源：http://msi.cqqwz.cn

[O01] 启动一个线程
来源：http://juk.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sup.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lir.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xxb.haohaochexian.top

TS:   // 同 JS
来源：http://yxi.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://cog.ywan-chungtsiang.top

Go:   go f()
来源：http://exf.haohaochexian.top

Ruby: Thread.new { f }
来源：http://oiy.fengsongda.top

C#:   Task.Run(() => F());
来源：http://tuo.jinqigufen.top

[O02] 使用线程池
来源：http://dln.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zxc.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ita.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://zqk.bjfxy.top

TS:   // worker_threads 线程池
来源：http://evo.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qsn.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pif.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ebj.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fib.fengsongda.top

[O03] 加锁保护共享数据
来源：http://vzx.sxryk.cn

Py:   with lock: shared += 1
来源：http://cyy.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://zli.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cfm.jqgfzy.top

TS:   // 同 JS
来源：http://rqq.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://bfd.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pec.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xuh.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://oes.fehbvm.com

[O04] 定义异步函数并等待
来源：http://qiq.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://erc.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ovt.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://fnc.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ewa.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://omm.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lfk.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://nxo.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://wan.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://aiz.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://pji.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bef.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://jzy.yongpay.top

TS:   await Promise.all(tasks)
来源：http://xal.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vuh.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ock.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://xet.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://oyp.jqgfzy.top

[O06] 使用进程池
来源：http://kuj.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oxt.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ccm.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://dst.yonumen.top

TS:   // child_process / cluster 模块
来源：http://esm.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rnt.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jbf.ydzc1.top

Ruby: // fork 块
来源：http://oee.jinqigfzy.top

C#:   Parallel.For
来源：http://ytx.hywenlv.cn

================================================================================
来源：http://pmj.ivvv.top

P. 常用工具函数
来源：http://ttk.hysaishi.cn

================================================================================
来源：http://eej.zhijiandao.cn

[P01] 生成 UUID
来源：http://kpn.hammf.cn

Py:   str(uuid.uuid4())
来源：http://qtk.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nca.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://ryv.iojbl.cn

TS:   crypto.randomUUID()
来源：http://hqs.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://jcy.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://mdi.yj202588.top

Ruby: SecureRandom.uuid
来源：http://ckq.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://jbi.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://axt.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://glu.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://uii.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tpq.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mcl.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zrv.gzhubu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wlg.bjfxy.top


<!-- 参考信息 -->