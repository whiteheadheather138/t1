代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xwl.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gei.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://umi.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vwg.52xcode.cn

[L03] 设置自定义请求头
来源：http://jcx.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gqm.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://coz.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nej.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pgp.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zfj.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jmo.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dav.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tea.jinqigfzy.top

[L04] 设置超时
来源：http://wze.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://wto.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dgq.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://usi.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mij.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nvf.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uoh.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yan.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tql.sxryk.cn

[L05] 上传文件（multipart）
来源：http://aeh.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlp.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pmy.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://soo.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://czt.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://egl.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqc.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://khl.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fug.aizwys.cn

[L06] 解析响应为 JSON
来源：http://vin.jinyuanbaomall.cn

Py:   resp.json()
来源：http://cgj.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://bvy.aibaodan.cn

JS:   await resp.json()
来源：http://ujy.nwbrower.top

TS:   await resp.json()
来源：http://fmf.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pug.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pwi.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://eua.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hhq.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://upj.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nsr.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ctp.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://vqj.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://ffw.gogol.net.cn

Java: resp.statusCode()
来源：http://agi.zhoulong.xyz

Go:   resp.StatusCode
来源：http://vzh.fengsongda.top

Ruby: resp.code.to_i
来源：http://iod.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://lww.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://iia.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bro.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://vpe.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://psc.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xfn.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://frr.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://puw.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mtw.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yhe.yvedp.cn

================================================================================
来源：http://dxt.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://uoi.jqgufenzy.top

================================================================================
来源：http://hhf.zhoulong.xyz

[M01] 读取命令行参数
来源：http://ued.fktsv.cn

Py:   sys.argv[1:]
来源：http://zfr.tian-w.cn

PHP:  $argv;  $argc;
来源：http://gbl.bjfxy.top

JS:   process.argv.slice(2)
来源：http://osp.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://lyr.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://kpp.jqgfzy.top

Go:   os.Args[1:]
来源：http://idw.daxiang520.top

Ruby: ARGV
来源：http://pqc.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://omr.zhoulong.xyz

[M02] 读取环境变量
来源：http://iyb.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://thh.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blr.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://ths.sxryk.cn

TS:   process.env.HOME
来源：http://lju.fehbvm.com

Java: System.getenv("HOME")
来源：http://fhv.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dob.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://mjb.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://asy.pycfn.com

[M03] 执行外部命令
来源：http://mte.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ied.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ios.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dyb.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ufp.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sbs.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pzk.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://dyp.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://sch.meibo888.top

[M04] 获取当前工作目录
来源：http://dzt.yueranfly.top

Py:   os.getcwd()
来源：http://ejp.havefunace.top

PHP:  getcwd();
来源：http://ucb.quarkkingdee.top

JS:   process.cwd()
来源：http://xnh.xinyue.icu

TS:   process.cwd()
来源：http://lph.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://ood.gotoacloud.top

Go:   os.Getwd()
来源：http://buu.ctjpmb.com

Ruby: Dir.pwd
来源：http://iej.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://caw.mhx1999.top

[M05] 设置退出码
来源：http://gfy.yanxiufei.cn

Py:   sys.exit(1)
来源：http://vmi.aizwys.cn

PHP:  exit(1);
来源：http://nyd.shangyingyoupin.top

JS:   process.exit(1)
来源：http://wip.epnwcf.com

TS:   process.exit(1)
来源：http://zcn.hesvh.cn

Java: System.exit(1)
来源：http://glg.zhijiandao.cn

Go:   os.Exit(1)
来源：http://giw.jinyuanbaomall.cn

Ruby: exit 1
来源：http://dsl.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hoo.guowangkeji.top

[M06] 向标准错误输出
来源：http://wwm.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://ila.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gzn.hcnkem.com

JS:   console.error("err")
来源：http://gju.fzhhl.top

TS:   console.error("err")
来源：http://ljv.ydzc1.top

Java: System.err.println("err")
来源：http://rtq.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dcg.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://cnw.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://eac.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://hbi.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://cas.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blm.yj20258888.top

JS:   require.main === module
来源：http://vlt.pycfn.com

TS:   require.main === module
来源：http://rul.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://ixr.guannengcc.top

Go:   func main()
来源：http://ozw.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://php.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://per.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://zav.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://ccc.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://rqk.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://yih.jqgfzy.top

TS:   process.platform;  process.version
来源：http://dse.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sdp.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vyb.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eqz.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gqq.316326.xyz

================================================================================
来源：http://vby.xziqi.cn

N. 数据结构与算法
来源：http://zam.gotoacloud.top

================================================================================
来源：http://fvc.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://grz.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://zbq.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xta.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://unf.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvt.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://ksj.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://yyg.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ujo.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://fgs.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://vzu.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://qzv.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ruz.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://axb.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vhj.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jmw.xuanzx.com

Go:   slices.Sort(arr)
来源：http://rit.chenlongwang.top

Ruby: arr.sort
来源：http://ycy.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gxm.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://myl.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kpi.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://ynn.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcg.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvd.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jyo.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gtj.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ffd.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lru.ydjk.org.cn

[N04] 斐波那契数列
来源：http://jcq.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://coq.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jmt.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzn.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cni.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://whb.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oeh.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ysl.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xee.ivvv.top

[N05] 最大公约数
来源：http://uzo.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://lfg.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aoy.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ayj.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nqe.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bti.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hny.ivvv.top

Ruby: a.gcd(b)
来源：http://ifw.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hwk.guowangkeji.top

[N06] 判断回文字符串
来源：http://axz.hywenlv.cn

Py:   s == s[::-1]
来源：http://ntc.yuxming.cn

PHP:  $s === strrev($s);
来源：http://exs.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://bys.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://uor.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wkq.tanke756.top

Go:   // 双指针从两端比较
来源：http://cdu.snrcjt.cn

Ruby: s == s.reverse
来源：http://mer.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wxn.meibo888.top

[N07] 两数之和（返回下标）
来源：http://xcj.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nxv.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uat.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zuh.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://yyx.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://sed.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://aik.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://rcw.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://sub.xziqi.cn

[N08] 生成全排列
来源：http://nzq.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://vml.ppjwa.cn

PHP:  // 手写递归交换
来源：http://fkv.hysaishi.cn

JS:   // 手写回溯递归
来源：http://wfe.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://esb.zdqjudy.top

Java: // 手写回溯递归
来源：http://arm.cashguo.top

Go:   // 手写回溯递归
来源：http://ugb.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://ncy.nwbrower.top

C#:   // 手写回溯递归
来源：http://mgz.jinqigufen.top

[N09] 栈与队列
来源：http://jsj.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ysk.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://klc.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ddj.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xvt.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nab.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lnc.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tje.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mco.jlsjyb.cn

[N10] 链表节点定义
来源：http://ipk.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nwh.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ohn.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dww.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://szx.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://wxx.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://xkg.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hcr.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hbj.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://bfu.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vmo.chenzaomai.com

PHP:  // 手写递归函数
来源：http://rot.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://frj.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fay.nwbrower.top

Java: // 手写递归
来源：http://poi.ehwqpu.com

Go:   // 手写递归
来源：http://mpp.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ewu.yangfankeji.com

C#:   // 手写递归
来源：http://xxa.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ngl.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jae.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dzb.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qmb.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hmz.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://frr.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eeb.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://clp.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xsm.9152youxi.cn

================================================================================
来源：http://kuv.shanyushiyangtech.top

O. 并发与异步
来源：http://sih.quarkkingdee.top

================================================================================
来源：http://gnr.jiagoushi.top

[O01] 启动一个线程
来源：http://hab.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zlr.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pmu.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kne.fzhhl.top

TS:   // 同 JS
来源：http://veb.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://oye.tian-w.cn

Go:   go f()
来源：http://pxr.uphjek.com

Ruby: Thread.new { f }
来源：http://gez.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://qju.zhoulong.xyz

[O02] 使用线程池
来源：http://ebc.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ita.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fmr.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://iml.jinqigufen.top

TS:   // worker_threads 线程池
来源：http://lvg.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ilx.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qgz.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zho.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aor.xuanzx.com

[O03] 加锁保护共享数据
来源：http://cbj.yongpay.top

Py:   with lock: shared += 1
来源：http://dpc.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://mfy.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ocy.zhijiandao.cn

TS:   // 同 JS
来源：http://wxa.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://zkh.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rqz.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yzq.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://ley.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://bzq.yj202588.top

Py:   async def f():⏎    await g()
来源：http://dgz.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bdr.jianghu66.top

JS:   async function f() { await g(); }
来源：http://gko.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://agz.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xlv.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bpk.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://mgq.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://azd.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://dyh.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://gxi.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ejk.hammf.cn

JS:   await Promise.all(tasks)
来源：http://uzs.316326.xyz

TS:   await Promise.all(tasks)
来源：http://vgt.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jdk.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://crk.shuidangran.top

Ruby: threads.map(&:join)
来源：http://pwa.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ofg.zhongyouzk.top

[O06] 使用进程池
来源：http://pkd.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rip.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pjs.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://vta.tarul.cn

TS:   // child_process / cluster 模块
来源：http://rno.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dzk.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://atn.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://gpz.yj20258.top


<!-- 参考信息 -->