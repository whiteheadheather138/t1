代发 wailian999

[L03] 设置自定义请求头
来源：http://xos.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xgz.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tny.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://let.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eca.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ygl.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cwd.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iuu.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wlh.jinghuilouyu.cn

[L04] 设置超时
来源：http://pil.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://hlv.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pur.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hiw.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eca.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yju.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nlj.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ukx.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bgs.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://xoc.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://exw.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jgq.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gfb.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dac.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pgd.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zfm.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fhg.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ogo.daria6918.cn

[L06] 解析响应为 JSON
来源：http://ohw.hesvh.cn

Py:   resp.json()
来源：http://yfw.redwolf501.top

PHP:  json_decode($body, true);
来源：http://ytz.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://vil.jinqigfzy.top

TS:   await resp.json()
来源：http://ged.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wfr.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vzj.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://akm.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zrq.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://nus.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wcy.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://des.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://rpr.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://xcx.fengsongda.top

Java: resp.statusCode()
来源：http://dkq.0kj1m.cn

Go:   resp.StatusCode
来源：http://qqa.cucudq.cn

Ruby: resp.code.to_i
来源：http://tiq.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://ptt.fengsongda.top

[L08] 并发请求多个地址
来源：http://eki.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gpa.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://beh.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rmd.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwv.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oby.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyl.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dji.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fjy.wangdashe.top

================================================================================
来源：http://lny.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://mrw.cashguo.top

================================================================================
来源：http://olp.sjlbkw.cn

[M01] 读取命令行参数
来源：http://qsa.xuanzx.com

Py:   sys.argv[1:]
来源：http://rnn.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://mut.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://oaz.yj202588.top

TS:   process.argv.slice(2)
来源：http://tnq.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://xtu.sxryk.cn

Go:   os.Args[1:]
来源：http://qzx.316326.xyz

Ruby: ARGV
来源：http://mwv.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://bri.haohaochexian.top

[M02] 读取环境变量
来源：http://dlr.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://wuj.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://irk.feifeiyinyue.top

JS:   process.env.HOME
来源：http://mzd.chenlongwang.top

TS:   process.env.HOME
来源：http://krr.smart0.xyz

Java: System.getenv("HOME")
来源：http://vqy.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://imq.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://mdb.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://caj.tian-w.cn

[M03] 执行外部命令
来源：http://wzi.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wab.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pja.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rcc.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aox.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mmb.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://qjs.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://sux.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://ozc.dashuyun.cn

[M04] 获取当前工作目录
来源：http://kkf.feifeiyinyue.top

Py:   os.getcwd()
来源：http://jzj.jinqigufen.top

PHP:  getcwd();
来源：http://thk.jlsjyb.cn

JS:   process.cwd()
来源：http://krg.fehbvm.com

TS:   process.cwd()
来源：http://rgq.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://pzu.gotoacloud.top

Go:   os.Getwd()
来源：http://luc.snrcjt.cn

Ruby: Dir.pwd
来源：http://cxf.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jwk.ydzc1.top

[M05] 设置退出码
来源：http://asx.316326.xyz

Py:   sys.exit(1)
来源：http://vef.yanxiufei.cn

PHP:  exit(1);
来源：http://iuj.jyoumei.cn

JS:   process.exit(1)
来源：http://hap.tanke756.top

TS:   process.exit(1)
来源：http://qrt.zdqjudy.top

Java: System.exit(1)
来源：http://jhj.hfpthk.cn

Go:   os.Exit(1)
来源：http://azf.shanyushiyangkeji.top

Ruby: exit 1
来源：http://gey.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uqt.yangfankeji.com

[M06] 向标准错误输出
来源：http://xbo.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://zgu.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yzh.hammf.cn

JS:   console.error("err")
来源：http://aik.cdnleiting.top

TS:   console.error("err")
来源：http://huy.hongshengwenyu.top

Java: System.err.println("err")
来源：http://gad.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://krl.bbcook.cn

Ruby: warn "err"
来源：http://ojr.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://kxa.andypj.xyz

[M07] 判断是否为主入口
来源：http://dhi.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://vam.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://osp.yj202588.top

JS:   require.main === module
来源：http://ebs.pycfn.com

TS:   require.main === module
来源：http://wfu.iojbl.cn

Java: public static void main(String[] args)
来源：http://rhj.smart0.xyz

Go:   func main()
来源：http://nmp.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vtq.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://vss.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://ofj.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://eof.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://nrp.chenzaomai.com

JS:   process.platform;  process.version
来源：http://zfw.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://nmh.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rqe.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uim.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ojg.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://itw.cqqwz.cn

================================================================================
来源：http://gbh.yj20258888.top

N. 数据结构与算法
来源：http://ugs.yvedp.cn

================================================================================
来源：http://leo.pycfn.com

[N01] 二分查找（有序数组）
来源：http://xlm.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://phs.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bhn.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wqi.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggg.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://roo.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://ppf.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ufv.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gwn.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://mwo.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gyx.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nmo.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://jqc.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aqf.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jue.fehbvm.com

Go:   slices.Sort(arr)
来源：http://yel.zhengqikj.top

Ruby: arr.sort
来源：http://qus.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lpa.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://dmc.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mfs.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://jjk.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vhe.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxw.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rwt.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vpi.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hhi.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://cox.birdmap.top

[N04] 斐波那契数列
来源：http://sts.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wgu.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bqh.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnb.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://udc.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wha.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ibm.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vyy.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lmh.svipenyu.cn

[N05] 最大公约数
来源：http://cfm.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://okx.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://onw.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hcc.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fig.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lff.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bwj.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://hot.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mhu.uphjek.com

[N06] 判断回文字符串
来源：http://bxq.52xcode.cn

Py:   s == s[::-1]
来源：http://otu.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://lbs.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://axi.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://han.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yfc.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://phj.guannengcc.top

Ruby: s == s.reverse
来源：http://beb.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nsq.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://xvr.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nwz.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mxz.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://nbr.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://ltk.zhijiandao.cn

Java: // 手写 HashMap
来源：http://waa.cashguo.top

Go:   // 手写 map[int]int
来源：http://ipn.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://wbq.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cwy.0kj1m.cn

[N08] 生成全排列
来源：http://cxr.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://zrt.jinqigufen.top

PHP:  // 手写递归交换
来源：http://qjl.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://ymy.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://eaz.gotoacloud.top

Java: // 手写回溯递归
来源：http://cmo.zycfv.cn

Go:   // 手写回溯递归
来源：http://qed.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://bcv.tanke756.top

C#:   // 手写回溯递归
来源：http://muo.feifeiyinyue.top

[N09] 栈与队列
来源：http://kgd.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ysd.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfy.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dkj.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kjn.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yne.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://noq.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wuw.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jws.dianchejie.cn

[N10] 链表节点定义
来源：http://xni.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nzu.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://llx.fktsv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tnf.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lzz.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://onc.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jxc.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cqj.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yml.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://kox.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bjf.tianlin.xyz

PHP:  // 手写递归函数
来源：http://mwu.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ysb.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ojm.ybcxt.top

Java: // 手写递归
来源：http://vnm.hywenlv.cn

Go:   // 手写递归
来源：http://yhq.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mkk.xziqi.cn

C#:   // 手写递归
来源：http://omk.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vmt.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ufn.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vyz.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nji.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyu.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iaa.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nlp.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ndu.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sqi.yueranfly.top

================================================================================
来源：http://ctu.yj20258888.top

O. 并发与异步
来源：http://gdw.cashguo.top

================================================================================
来源：http://wko.zhiwuduotai.top

[O01] 启动一个线程
来源：http://gms.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wrl.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wkj.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blk.hesvh.cn

TS:   // 同 JS
来源：http://bkd.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://ktl.zhijiandao.cn

Go:   go f()
来源：http://eue.cheryme.top

Ruby: Thread.new { f }
来源：http://mua.cucudq.cn

C#:   Task.Run(() => F());
来源：http://ffy.daria6918.cn

[O02] 使用线程池
来源：http://swc.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bka.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jag.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://uqz.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://gio.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://fum.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hmy.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aaz.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://obx.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://vcz.fktsv.cn

Py:   with lock: shared += 1
来源：http://tnk.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://qvk.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ibe.316326.xyz

TS:   // 同 JS
来源：http://dnl.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://gdb.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qny.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jtl.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://rqb.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://zru.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://omt.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://clh.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://zye.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xmo.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xif.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kdx.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://ser.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://ped.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://yql.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://fgz.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ypb.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://opi.cheryme.top

TS:   await Promise.all(tasks)
来源：http://shh.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lwr.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dcl.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://shm.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://bsa.wangdashe.top

[O06] 使用进程池
来源：http://guu.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wvr.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rcf.tanke756.top

JS:   // child_process / cluster 模块
来源：http://sts.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://ycr.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mui.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lqs.sysykeji.top

Ruby: // fork 块
来源：http://hyu.vehdjk.com

C#:   Parallel.For
来源：http://qrs.zhixingplan.top

================================================================================
来源：http://qal.hcnkem.com

P. 常用工具函数
来源：http://lij.nanxinkj.top

================================================================================
来源：http://nov.c1oappe.top


<!-- 参考信息 -->