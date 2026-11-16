代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sya.sysykeji.top

[L04] 设置超时
来源：http://fhg.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://ovc.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tet.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wpp.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dry.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fxw.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xto.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tax.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vwy.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://yun.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xto.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://otv.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://swo.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dig.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://str.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nat.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bsn.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zcf.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://zua.gogol.net.cn

Py:   resp.json()
来源：http://gpb.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://ihm.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://off.yvedp.cn

TS:   await resp.json()
来源：http://wof.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rzq.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wrf.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://trk.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lfo.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://rgl.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qlf.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iog.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://ldn.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://ijg.xuetiantiany.cn

Java: resp.statusCode()
来源：http://wgu.cqqwz.cn

Go:   resp.StatusCode
来源：http://uju.andypj.xyz

Ruby: resp.code.to_i
来源：http://ker.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://yis.jianghu66.top

[L08] 并发请求多个地址
来源：http://khc.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fuc.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://vss.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsy.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://phy.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://szl.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qtd.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rwe.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lpz.hesvh.cn

================================================================================
来源：http://uhv.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://itj.jinqigfzy.top

================================================================================
来源：http://nmx.sxryk.cn

[M01] 读取命令行参数
来源：http://tcc.haohaochexian.top

Py:   sys.argv[1:]
来源：http://gqy.xuanzx.com

PHP:  $argv;  $argc;
来源：http://cya.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://omz.xylfe.cn

TS:   process.argv.slice(2)
来源：http://cgr.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://tdz.52xcode.cn

Go:   os.Args[1:]
来源：http://wqq.redwolf501.top

Ruby: ARGV
来源：http://shp.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://adh.316326.xyz

[M02] 读取环境变量
来源：http://rto.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://vel.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vly.zhixingplan.top

JS:   process.env.HOME
来源：http://nxe.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://hey.wangdashe.top

Java: System.getenv("HOME")
来源：http://dwd.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ahv.tanke756.top

Ruby: ENV["HOME"]
来源：http://umh.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pll.shuidangran.top

[M03] 执行外部命令
来源：http://jce.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://upp.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ycm.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oww.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://gno.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nvz.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mcm.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://vxz.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://hzk.cucudq.cn

[M04] 获取当前工作目录
来源：http://xfz.fehbvm.com

Py:   os.getcwd()
来源：http://hjj.ydjk.org.cn

PHP:  getcwd();
来源：http://imp.cashguo.top

JS:   process.cwd()
来源：http://vfl.chenlongwang.top

TS:   process.cwd()
来源：http://lqu.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://cac.yj20258888.top

Go:   os.Getwd()
来源：http://shu.yj20258.top

Ruby: Dir.pwd
来源：http://njk.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://hcb.jyoumei.cn

[M05] 设置退出码
来源：http://flw.sysykeji.top

Py:   sys.exit(1)
来源：http://tvl.fktsv.cn

PHP:  exit(1);
来源：http://reb.zhijiandao.cn

JS:   process.exit(1)
来源：http://lwb.andypj.xyz

TS:   process.exit(1)
来源：http://urq.hnqzz.top

Java: System.exit(1)
来源：http://eir.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://erf.yj202588.top

Ruby: exit 1
来源：http://pyc.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://meq.zhoulong.xyz

[M06] 向标准错误输出
来源：http://eie.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://uhx.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://obr.epnwcf.com

JS:   console.error("err")
来源：http://wvw.fanxiaobao.xyz

TS:   console.error("err")
来源：http://snd.jinqigufen.top

Java: System.err.println("err")
来源：http://lia.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jcg.xuanzx.com

Ruby: warn "err"
来源：http://yps.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://umd.yuxming.cn

[M07] 判断是否为主入口
来源：http://gac.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://dqs.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zpc.sjlbkw.cn

JS:   require.main === module
来源：http://mbv.vqdsnc.cn

TS:   require.main === module
来源：http://qai.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://alr.yongpay.top

Go:   func main()
来源：http://cke.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xgb.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://lwl.yj202588.top

[M08] 获取系统与运行时信息
来源：http://xlf.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://vxt.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://ymq.hesvh.cn

JS:   process.platform;  process.version
来源：http://cls.iojbl.cn

TS:   process.platform;  process.version
来源：http://iaq.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qxx.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ums.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bbg.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nrc.fengsongda.top

================================================================================
来源：http://gyy.cqqwz.cn

N. 数据结构与算法
来源：http://dyo.fehbvm.com

================================================================================
来源：http://dap.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://acr.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://uli.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ohy.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bga.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzs.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://vat.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://eig.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qbc.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://dtr.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://uls.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://daa.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ier.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ojh.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bot.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://toy.wangdashe.top

Go:   slices.Sort(arr)
来源：http://xnd.bbcook.cn

Ruby: arr.sort
来源：http://rwz.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://old.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://fmq.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wah.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://ugb.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bmh.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uoj.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xby.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ybm.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tih.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://kfg.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://jww.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bho.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lgg.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://itz.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jhm.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lcu.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wnc.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dgv.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://knu.ppjwa.cn

[N05] 最大公约数
来源：http://fkd.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://zjn.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://akt.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hbu.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dxc.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mhg.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wad.aibaodan.cn

Ruby: a.gcd(b)
来源：http://aza.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wwg.hesvh.cn

[N06] 判断回文字符串
来源：http://phd.snrcjt.cn

Py:   s == s[::-1]
来源：http://iji.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://qqa.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://nov.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://uwq.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xqi.yueranfly.top

Go:   // 双指针从两端比较
来源：http://nqu.snrcjt.cn

Ruby: s == s.reverse
来源：http://etz.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lxv.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://von.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oow.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tkx.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yvk.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://zdy.jqgufenzy.top

Java: // 手写 HashMap
来源：http://ucg.yj202588.top

Go:   // 手写 map[int]int
来源：http://cnf.zycfv.cn

Ruby: // 手写 Hash
来源：http://txw.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://muz.yj20258888.top

[N08] 生成全排列
来源：http://gcm.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://lew.hcnkem.com

PHP:  // 手写递归交换
来源：http://twi.yj202588.top

JS:   // 手写回溯递归
来源：http://pvd.tian-w.cn

TS:   // 手写回溯递归
来源：http://tdo.wangdashe.top

Java: // 手写回溯递归
来源：http://fhh.ivvv.top

Go:   // 手写回溯递归
来源：http://vki.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://csl.nanxinkj.top

C#:   // 手写回溯递归
来源：http://brn.zhoulong.xyz

[N09] 栈与队列
来源：http://jvw.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mxl.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yec.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xua.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uvh.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://btn.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://syd.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ynh.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wzo.fengsongda.top

[N10] 链表节点定义
来源：http://qam.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bau.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hfi.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uue.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xca.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://qwd.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://miv.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kpx.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gwy.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://wpn.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ysw.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://mlg.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfe.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wym.vehdjk.com

Java: // 手写递归
来源：http://ilj.bbcook.cn

Go:   // 手写递归
来源：http://qcu.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jvc.yonumen.top

C#:   // 手写递归
来源：http://akt.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxr.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://avl.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mdz.cqqwz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wwo.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aco.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pze.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uxr.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bsu.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eoc.yueranfly.top

================================================================================
来源：http://fjl.snrcjt.cn

O. 并发与异步
来源：http://xbu.quarkkingdee.top

================================================================================
来源：http://euy.zhiwuduotai.top

[O01] 启动一个线程
来源：http://kvl.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zjj.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tth.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mcg.chenjidiqi.icu

TS:   // 同 JS
来源：http://lve.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://fkw.yfazqb.com

Go:   go f()
来源：http://syj.hysaishi.cn

Ruby: Thread.new { f }
来源：http://fzi.sweek.top

C#:   Task.Run(() => F());
来源：http://gwg.cheryme.top

[O02] 使用线程池
来源：http://vhl.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xqa.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ycq.bjfxy.top

JS:   // worker_threads 线程池
来源：http://ind.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://djs.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://ywh.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ngt.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xvz.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eku.fzhhl.top

[O03] 加锁保护共享数据
来源：http://qge.gogol.net.cn

Py:   with lock: shared += 1
来源：http://lgh.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://mmn.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hvg.vehdjk.com

TS:   // 同 JS
来源：http://tju.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://fam.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ycs.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgl.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://wtf.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://xvo.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://hrh.xuetiantiany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mwi.bjfxy.top

JS:   async function f() { await g(); }
来源：http://pui.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ayw.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://etp.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kjq.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jnh.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://blu.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://arz.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://cme.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://efu.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://gty.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://gwe.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fld.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hgi.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://hsa.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oqp.shuidangran.top

[O06] 使用进程池
来源：http://ejy.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lzp.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pty.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://zeq.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://lph.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vdo.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nmn.pycfn.com

Ruby: // fork 块
来源：http://eew.hongshengwenyu.top

C#:   Parallel.For
来源：http://lim.yongpay.top

================================================================================
来源：http://fbz.cucudq.cn

P. 常用工具函数
来源：http://qzh.ppjwa.cn

================================================================================
来源：http://ypp.gaohongyu789.top

[P01] 生成 UUID
来源：http://eha.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://wxd.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rzs.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://dlq.andypj.xyz

TS:   crypto.randomUUID()
来源：http://xzv.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://meh.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://cgm.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://vqd.9152youxi.cn


<!-- 参考信息 -->