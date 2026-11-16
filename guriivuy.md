代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ugo.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fly.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jbt.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kmj.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wrx.yj202588.top

[L04] 设置超时
来源：http://pob.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://rty.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dai.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hal.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ehn.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ccu.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iwv.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xyt.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jow.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://yli.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ggq.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogh.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mxt.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tvt.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://otp.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gjf.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nhi.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dqw.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://wzr.fzhhl.top

Py:   resp.json()
来源：http://gni.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://kje.hywenlv.cn

JS:   await resp.json()
来源：http://pyu.xuanzx.com

TS:   await resp.json()
来源：http://fqr.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xtv.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://obw.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://bsk.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xqt.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://mqg.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://our.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zps.meibo888.top

JS:   resp.ok;  resp.status
来源：http://hnc.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://nkp.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://yti.mhx1999.top

Go:   resp.StatusCode
来源：http://wtg.andypj.xyz

Ruby: resp.code.to_i
来源：http://ndt.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://ooo.zhixingplan.top

[L08] 并发请求多个地址
来源：http://qat.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hpj.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://vmq.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fld.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zgo.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uun.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://csi.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jxw.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wio.tanke756.top

================================================================================
来源：http://xfa.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://khz.bbcook.cn

================================================================================
来源：http://orz.jyoumei.cn

[M01] 读取命令行参数
来源：http://rcr.ybcxt.top

Py:   sys.argv[1:]
来源：http://pmz.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://ozi.yj202588.top

JS:   process.argv.slice(2)
来源：http://ktt.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://zpw.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://vht.sufxvd.cn

Go:   os.Args[1:]
来源：http://zde.gotoacloud.top

Ruby: ARGV
来源：http://tpi.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://wum.zhiwuduotai.top

[M02] 读取环境变量
来源：http://xgt.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://xef.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dga.zhengqikj.top

JS:   process.env.HOME
来源：http://nra.bbcook.cn

TS:   process.env.HOME
来源：http://agj.yvedp.cn

Java: System.getenv("HOME")
来源：http://ajf.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://awt.fzhhl.top

Ruby: ENV["HOME"]
来源：http://zoh.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ccu.sweek.top

[M03] 执行外部命令
来源：http://pdw.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nnt.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://byv.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://obt.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lek.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xyk.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hle.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://epr.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://cux.shzxlz.cn

[M04] 获取当前工作目录
来源：http://vbc.andypj.xyz

Py:   os.getcwd()
来源：http://edv.hysaishi.cn

PHP:  getcwd();
来源：http://vvw.dianchejie.cn

JS:   process.cwd()
来源：http://fft.chenzaomai.com

TS:   process.cwd()
来源：http://uif.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://qqe.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://yxw.mhx1999.top

Ruby: Dir.pwd
来源：http://bqp.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gpz.pycfn.com

[M05] 设置退出码
来源：http://ybp.zhixingplan.top

Py:   sys.exit(1)
来源：http://uyb.ppjwa.cn

PHP:  exit(1);
来源：http://wxx.zycfv.cn

JS:   process.exit(1)
来源：http://oao.chenzaomai.com

TS:   process.exit(1)
来源：http://fvi.jqgfzy.top

Java: System.exit(1)
来源：http://ppn.jianghu66.top

Go:   os.Exit(1)
来源：http://zkm.hammf.cn

Ruby: exit 1
来源：http://nkh.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://piz.wangdashe.top

[M06] 向标准错误输出
来源：http://meo.zhixingplan.top

Py:   print("err", file=sys.stderr)
来源：http://lit.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://oov.dashuyun.cn

JS:   console.error("err")
来源：http://ain.haohaochexian.top

TS:   console.error("err")
来源：http://chy.yuxming.cn

Java: System.err.println("err")
来源：http://cqo.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qip.dashuyun.cn

Ruby: warn "err"
来源：http://ted.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://ufq.9152youxi.cn

[M07] 判断是否为主入口
来源：http://aep.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://unx.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vmg.zhaomingkeji.xyz

JS:   require.main === module
来源：http://xmj.zycfv.cn

TS:   require.main === module
来源：http://eny.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://wln.yj202588.top

Go:   func main()
来源：http://ewx.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kjo.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://slv.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://mfo.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://kon.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://dat.ybcxt.top

JS:   process.platform;  process.version
来源：http://mkm.sufxvd.cn

TS:   process.platform;  process.version
来源：http://cmg.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://buw.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pdr.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwf.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tbd.yonumen.top

================================================================================
来源：http://dcc.jinqigfzy.top

N. 数据结构与算法
来源：http://yyj.zhijiandao.cn

================================================================================
来源：http://sbe.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://efw.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://iyp.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nwu.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bqf.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sjh.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://ghe.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://udj.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uht.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://baw.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://skv.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://bdq.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hmc.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qgq.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xkq.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pcg.xinyue.icu

Go:   slices.Sort(arr)
来源：http://uji.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://qmp.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://irc.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://qqm.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vlv.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://krw.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esg.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsz.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ice.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yde.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kvw.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://hnr.sweek.top

[N04] 斐波那契数列
来源：http://qjw.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fgq.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gdt.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tbf.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vgp.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqs.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zpy.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nvm.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sdx.yj20258.top

[N05] 最大公约数
来源：http://flo.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://vdm.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qwe.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugt.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzx.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ash.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cxq.ydzc1.top

Ruby: a.gcd(b)
来源：http://gvi.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hex.bjfxy.top

[N06] 判断回文字符串
来源：http://oua.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://jkh.nwbrower.top

PHP:  $s === strrev($s);
来源：http://xzt.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://ojd.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://xje.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yoh.cheryme.top

Go:   // 双指针从两端比较
来源：http://bhh.shzxlz.cn

Ruby: s == s.reverse
来源：http://zsc.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vad.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://cbm.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lru.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kqc.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://sff.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://plk.mhx1999.top

Java: // 手写 HashMap
来源：http://pwl.daria6918.cn

Go:   // 手写 map[int]int
来源：http://eck.yuanzhike.top

Ruby: // 手写 Hash
来源：http://ubp.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://bsc.hnxiangtu.top

[N08] 生成全排列
来源：http://mbx.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://wks.9152youxi.cn

PHP:  // 手写递归交换
来源：http://wlp.meibo888.top

JS:   // 手写回溯递归
来源：http://kpt.yuanzhike.top

TS:   // 手写回溯递归
来源：http://pvg.dianchejie.cn

Java: // 手写回溯递归
来源：http://hkt.yj20258888.top

Go:   // 手写回溯递归
来源：http://bzl.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://scl.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://szb.vqdsnc.cn

[N09] 栈与队列
来源：http://bxc.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mgj.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xrn.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ges.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://emk.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qvo.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ktt.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zvp.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sjb.yueranfly.top

[N10] 链表节点定义
来源：http://kgo.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ezx.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://imv.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xde.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jiv.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://bgp.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://wtz.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ipe.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bcv.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://jtx.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gab.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://pqy.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fpj.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hua.0kj1m.cn

Java: // 手写递归
来源：http://qyr.yj202588.top

Go:   // 手写递归
来源：http://sql.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tfp.jinqigufen.top

C#:   // 手写递归
来源：http://rfs.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pnk.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yjt.pengpengdd.cyou

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qco.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qsv.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zty.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgf.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lmc.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vaw.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bbc.guowangkeji.top

================================================================================
来源：http://lnv.316326.xyz

O. 并发与异步
来源：http://soa.kuanghao11.cn

================================================================================
来源：http://dcs.ehwqpu.com

[O01] 启动一个线程
来源：http://fhb.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://feg.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fiz.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mnq.fengsongda.top

TS:   // 同 JS
来源：http://cfs.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://zyc.hywenlv.cn

Go:   go f()
来源：http://ojy.nwbrower.top

Ruby: Thread.new { f }
来源：http://lni.wangdashe.top

C#:   Task.Run(() => F());
来源：http://usc.quarkkingdee.top

[O02] 使用线程池
来源：http://gco.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jfz.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iub.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://diy.yueranfly.top

TS:   // worker_threads 线程池
来源：http://ewg.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://oqq.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eyo.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nmu.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nql.yvedp.cn

[O03] 加锁保护共享数据
来源：http://art.zdbjq.cn

Py:   with lock: shared += 1
来源：http://unq.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://avh.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jis.jiagoushi.top

TS:   // 同 JS
来源：http://xba.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://eco.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://csv.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://pjo.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://ugn.yonumen.top

[O04] 定义异步函数并等待
来源：http://nys.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://xqw.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bxy.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://tpk.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tcr.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://itv.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ppe.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://yjd.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://ilo.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://eww.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://pdj.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpb.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://bfd.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://iqz.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fil.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://arc.dianchejie.cn

Ruby: threads.map(&:join)
来源：http://vbf.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://woe.sxryk.cn

[O06] 使用进程池
来源：http://vkq.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rvn.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ach.sweek.top

JS:   // child_process / cluster 模块
来源：http://jff.uphjek.com

TS:   // child_process / cluster 模块
来源：http://nnc.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oqc.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cwo.vqdsnc.cn

Ruby: // fork 块
来源：http://mmw.hywenlv.cn

C#:   Parallel.For
来源：http://dds.jinqigufen.top

================================================================================
来源：http://nsv.cashguo.top

P. 常用工具函数
来源：http://lke.shanyushiyangkeji.top

================================================================================
来源：http://vrm.cqqwz.cn

[P01] 生成 UUID
来源：http://gxz.yonumen.top

Py:   str(uuid.uuid4())
来源：http://ywh.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cnq.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://nhc.nwbrower.top


<!-- 参考信息 -->