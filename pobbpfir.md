代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jds.zhixingplan.top

[L04] 设置超时
来源：http://bnn.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://nwb.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://szo.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdg.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lqp.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://amu.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uvq.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qew.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xfa.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://myv.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qkb.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sag.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://joz.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fen.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://naa.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ljd.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nsg.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qlj.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://qcr.hnxiangtu.top

Py:   resp.json()
来源：http://iex.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://wqq.redwolf501.top

JS:   await resp.json()
来源：http://mzd.fzhhl.top

TS:   await resp.json()
来源：http://bub.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qsy.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mju.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://qoo.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ukx.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://cbi.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yxb.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yph.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://wvd.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://mli.cqqwz.cn

Java: resp.statusCode()
来源：http://ubr.guowangkeji.top

Go:   resp.StatusCode
来源：http://bih.guowangkeji.top

Ruby: resp.code.to_i
来源：http://zzk.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://mzy.yueranfly.top

[L08] 并发请求多个地址
来源：http://cbk.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zjx.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://jiu.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftw.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyt.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cjy.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ofq.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yrw.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aqa.9152youxi.cn

================================================================================
来源：http://fmo.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://cpb.jianghu66.top

================================================================================
来源：http://azi.0kj1m.cn

[M01] 读取命令行参数
来源：http://ezu.yueranfly.top

Py:   sys.argv[1:]
来源：http://djn.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://unw.yj20258.top

JS:   process.argv.slice(2)
来源：http://agu.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://tcu.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://moq.yuanzhike.top

Go:   os.Args[1:]
来源：http://ysm.guowangkeji.top

Ruby: ARGV
来源：http://pqf.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://mkt.xuetiantiany.cn

[M02] 读取环境变量
来源：http://ejd.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://vjq.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uux.feifeiyinyue.top

JS:   process.env.HOME
来源：http://pwn.0kj1m.cn

TS:   process.env.HOME
来源：http://kji.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://tov.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wbg.cashguo.top

Ruby: ENV["HOME"]
来源：http://rvi.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rvj.nwbrower.top

[M03] 执行外部命令
来源：http://plt.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://atx.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://olj.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xgm.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ecg.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cuy.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://zvd.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wjd.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ytp.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://yus.ivvv.top

Py:   os.getcwd()
来源：http://nqe.zhoulong.xyz

PHP:  getcwd();
来源：http://aik.hfpthk.cn

JS:   process.cwd()
来源：http://pbd.xinyue.icu

TS:   process.cwd()
来源：http://arm.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://bgd.ybcxt.top

Go:   os.Getwd()
来源：http://exq.cucudq.cn

Ruby: Dir.pwd
来源：http://zdw.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://cxt.shangyingyoupin.top

[M05] 设置退出码
来源：http://cqy.svipenyu.cn

Py:   sys.exit(1)
来源：http://rho.chenjidiqi.icu

PHP:  exit(1);
来源：http://mpq.cdnleiting.top

JS:   process.exit(1)
来源：http://ovd.gaohongyu789.top

TS:   process.exit(1)
来源：http://ggf.feifeiyinyue.top

Java: System.exit(1)
来源：http://vep.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://nbe.fktsv.cn

Ruby: exit 1
来源：http://zhm.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sas.yanxiufei.cn

[M06] 向标准错误输出
来源：http://nxf.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://rhi.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vcy.sxryk.cn

JS:   console.error("err")
来源：http://quy.shuidangran.top

TS:   console.error("err")
来源：http://eyd.ivvv.top

Java: System.err.println("err")
来源：http://guy.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lne.yangfankeji.com

Ruby: warn "err"
来源：http://wos.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://odt.zdbjq.cn

[M07] 判断是否为主入口
来源：http://fsf.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://lah.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://opn.shanyushiyangtech.top

JS:   require.main === module
来源：http://rrc.hammf.cn

TS:   require.main === module
来源：http://edn.xziqi.cn

Java: public static void main(String[] args)
来源：http://rov.tanke756.top

Go:   func main()
来源：http://yoc.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bgr.c1oappe.top

C#:   static void Main(string[] args)
来源：http://sst.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://wjp.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://cyo.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yzr.ctjpmb.com

JS:   process.platform;  process.version
来源：http://bvh.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://qiu.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yoi.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgb.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sct.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jyl.tianlin.xyz

================================================================================
来源：http://wcf.iojbl.cn

N. 数据结构与算法
来源：http://ewy.hnqzz.top

================================================================================
来源：http://szi.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://sfw.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fvd.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ryz.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baw.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tkq.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://fmm.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://bxm.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://urn.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vjx.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://jgf.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xmv.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mdm.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jde.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tio.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wkp.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://aqv.jlsjyb.cn

Ruby: arr.sort
来源：http://toc.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zfn.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://mgn.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ptt.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://wop.316326.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwl.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bmw.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rji.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fca.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vxu.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://ydg.jinqigufen.top

[N04] 斐波那契数列
来源：http://tes.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yfe.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fuq.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vph.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bsw.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sxs.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uqv.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rhj.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fkl.epnwcf.com

[N05] 最大公约数
来源：http://gjg.pycfn.com

Py:   math.gcd(a, b)
来源：http://uih.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fof.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmh.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qly.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gwu.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ltv.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://awk.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://biz.jqgfzy.top

[N06] 判断回文字符串
来源：http://nvn.dashuyun.cn

Py:   s == s[::-1]
来源：http://ynm.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://xkx.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://aun.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://nfg.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dij.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://ipz.ppjwa.cn

Ruby: s == s.reverse
来源：http://zut.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rbf.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://cet.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sbe.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://brw.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ava.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://vgq.yuanzhike.top

Java: // 手写 HashMap
来源：http://qjr.c1oappe.top

Go:   // 手写 map[int]int
来源：http://wml.epnwcf.com

Ruby: // 手写 Hash
来源：http://xsz.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://cwv.jinqigufen.top

[N08] 生成全排列
来源：http://bci.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://odj.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://het.yj20258888.top

JS:   // 手写回溯递归
来源：http://ycr.c1oappe.top

TS:   // 手写回溯递归
来源：http://mmf.ydzc1.top

Java: // 手写回溯递归
来源：http://nfv.gogol.net.cn

Go:   // 手写回溯递归
来源：http://cie.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://unc.fzhhl.top

C#:   // 手写回溯递归
来源：http://smw.9152youxi.cn

[N09] 栈与队列
来源：http://nzs.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bcy.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cik.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://viz.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eln.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wlj.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jgt.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://trz.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vob.yj202588.top

[N10] 链表节点定义
来源：http://csw.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zli.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vyh.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wts.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cpn.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://dzh.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://yro.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dxq.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://kto.andypj.xyz

[N11] 二叉树中序遍历
来源：http://opt.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mfd.aibaodan.cn

PHP:  // 手写递归函数
来源：http://swu.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://csl.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mkz.wangdashe.top

Java: // 手写递归
来源：http://phv.fehbvm.com

Go:   // 手写递归
来源：http://kxl.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wpb.birdmap.top

C#:   // 手写递归
来源：http://ryu.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tbh.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gmy.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bfr.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvw.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rha.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hyr.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ppi.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hhs.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oav.yfazqb.com

================================================================================
来源：http://say.hammf.cn

O. 并发与异步
来源：http://cxg.pengpengdd.cyou

================================================================================
来源：http://uuf.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://vak.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ewj.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ija.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hbs.zhoulong.xyz

TS:   // 同 JS
来源：http://rde.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://iyy.quarkkingdee.top

Go:   go f()
来源：http://vhb.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://hzu.ivvv.top

C#:   Task.Run(() => F());
来源：http://qge.hywenlv.cn

[O02] 使用线程池
来源：http://kgm.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zfr.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aag.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://njl.daria6918.cn

TS:   // worker_threads 线程池
来源：http://bhu.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://qbg.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zwm.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mwf.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vqa.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://mst.nwbrower.top

Py:   with lock: shared += 1
来源：http://wtp.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://tmg.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vzo.xinyue.icu

TS:   // 同 JS
来源：http://lwe.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://zyr.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xsi.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dks.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://kgv.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://tvl.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://zsj.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hul.havefunace.top

JS:   async function f() { await g(); }
来源：http://mzd.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://imh.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wny.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pog.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://mmn.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://dqp.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://exo.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://oia.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://otc.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://tyr.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://krp.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vej.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eea.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://tlq.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hzm.chenjidiqi.icu

[O06] 使用进程池
来源：http://ipe.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bxr.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://khw.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://fav.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://hlx.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cup.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hdk.iojbl.cn

Ruby: // fork 块
来源：http://nxl.sweek.top

C#:   Parallel.For
来源：http://ojh.shangyingyoupin.top

================================================================================
来源：http://oxs.yongpay.top

P. 常用工具函数
来源：http://oxo.jinqigfzy.top

================================================================================
来源：http://gjo.chenzaomai.com

[P01] 生成 UUID
来源：http://dzj.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://lya.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jnr.yueranfly.top

JS:   crypto.randomUUID()
来源：http://rke.shuidangran.top

TS:   crypto.randomUUID()
来源：http://wxg.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://smm.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://tov.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://zhg.yj20258888.top


<!-- 参考信息 -->