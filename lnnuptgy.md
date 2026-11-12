代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ntx.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gwx.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bgm.9152youxi.cn

[L02] 发送 POST JSON
来源：http://cce.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://joc.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xdb.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgw.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eby.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uhq.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wza.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hrp.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://usb.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://pbl.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ewl.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qaj.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wvb.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnp.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vmx.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jgj.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xgh.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wum.zdbjq.cn

[L04] 设置超时
来源：http://rca.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://vcc.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kux.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syh.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dky.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://daa.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qvp.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vyg.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pqs.bjfxy.top

[L05] 上传文件（multipart）
来源：http://sdp.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jaf.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qno.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://beu.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jnp.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rjv.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dnc.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xcs.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eki.sysykeji.top

[L06] 解析响应为 JSON
来源：http://bww.snrcjt.cn

Py:   resp.json()
来源：http://mps.fktsv.cn

PHP:  json_decode($body, true);
来源：http://jjd.fehbvm.com

JS:   await resp.json()
来源：http://bre.yuxming.cn

TS:   await resp.json()
来源：http://dwm.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nld.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://glu.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://jtq.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://beg.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://kef.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mke.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://omw.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://faf.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://kgk.cashguo.top

Java: resp.statusCode()
来源：http://gjm.nanxinkj.top

Go:   resp.StatusCode
来源：http://tym.yj20258.top

Ruby: resp.code.to_i
来源：http://xya.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://qlg.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://xdq.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cxi.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://kpw.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qqy.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://adz.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ygt.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mce.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bsf.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uoe.zhaomingkeji.xyz

================================================================================
来源：http://pgi.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://zdj.zycfv.cn

================================================================================
来源：http://ruv.dashuyun.cn

[M01] 读取命令行参数
来源：http://pqb.gogol.net.cn

Py:   sys.argv[1:]
来源：http://cmz.nwbrower.top

PHP:  $argv;  $argc;
来源：http://qxa.shuidangran.top

JS:   process.argv.slice(2)
来源：http://yum.xylfe.cn

TS:   process.argv.slice(2)
来源：http://nff.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://ads.ppjwa.cn

Go:   os.Args[1:]
来源：http://kxv.nanxinkj.top

Ruby: ARGV
来源：http://zsq.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://cwx.havefunace.top

[M02] 读取环境变量
来源：http://aiq.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://zcf.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ndt.fktsv.cn

JS:   process.env.HOME
来源：http://drz.guowangkeji.top

TS:   process.env.HOME
来源：http://tbn.ydzc1.top

Java: System.getenv("HOME")
来源：http://whs.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ezq.iojbl.cn

Ruby: ENV["HOME"]
来源：http://end.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xem.vqdsnc.cn

[M03] 执行外部命令
来源：http://yud.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggk.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dzh.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zof.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rmj.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zsc.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pvx.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://iar.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://nlg.9152youxi.cn

[M04] 获取当前工作目录
来源：http://yay.aibaodan.cn

Py:   os.getcwd()
来源：http://hfc.316326.xyz

PHP:  getcwd();
来源：http://hmc.gzhubu.top

JS:   process.cwd()
来源：http://bir.gaohongyu789.top

TS:   process.cwd()
来源：http://por.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://nhe.nwbrower.top

Go:   os.Getwd()
来源：http://oox.hammf.cn

Ruby: Dir.pwd
来源：http://qhr.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://jsl.jlsjyb.cn

[M05] 设置退出码
来源：http://icx.yfazqb.com

Py:   sys.exit(1)
来源：http://nmb.sjlbkw.cn

PHP:  exit(1);
来源：http://fxt.vqdsnc.cn

JS:   process.exit(1)
来源：http://kpt.redwolf501.top

TS:   process.exit(1)
来源：http://gis.hcnkem.com

Java: System.exit(1)
来源：http://aoo.zhoulong.xyz

Go:   os.Exit(1)
来源：http://lcu.wangshuangyany.cn

Ruby: exit 1
来源：http://emf.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jur.zdqjudy.top

[M06] 向标准错误输出
来源：http://kbt.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://ttc.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rlk.daxiang520.top

JS:   console.error("err")
来源：http://why.iojbl.cn

TS:   console.error("err")
来源：http://nre.shzxlz.cn

Java: System.err.println("err")
来源：http://gqw.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ame.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://iac.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://zag.cashguo.top

[M07] 判断是否为主入口
来源：http://ruy.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://qid.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yyg.0kj1m.cn

JS:   require.main === module
来源：http://cqx.vqdsnc.cn

TS:   require.main === module
来源：http://duc.fzhhl.top

Java: public static void main(String[] args)
来源：http://jnj.cdnleiting.top

Go:   func main()
来源：http://rkr.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cdy.hnqzz.top

C#:   static void Main(string[] args)
来源：http://snt.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://rgc.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://yfd.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ohi.chenlongwang.top

JS:   process.platform;  process.version
来源：http://vne.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://xyp.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://llg.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mxq.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dzk.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ivw.fehbvm.com

================================================================================
来源：http://hqf.zhoulong.xyz

N. 数据结构与算法
来源：http://rwi.jiagoushi.top

================================================================================
来源：http://sby.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://pke.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://vbb.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mql.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://shd.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghk.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yfu.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://gpj.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bco.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://bzx.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://mkm.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://xup.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wdi.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zee.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jbq.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pqy.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://lpi.andypj.xyz

Ruby: arr.sort
来源：http://zcw.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://swj.tarul.cn

[N03] 快速排序（分治示例）
来源：http://qov.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ujp.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://uva.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yyu.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlq.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hkr.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xml.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jtb.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://ylb.gzhubu.top

[N04] 斐波那契数列
来源：http://cba.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kfl.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hgl.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://viz.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://svc.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yll.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tny.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nsl.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rzq.bjfxy.top

[N05] 最大公约数
来源：http://ufl.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://cgg.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qgo.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aba.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpj.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://daj.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hya.yuxming.cn

Ruby: a.gcd(b)
来源：http://bfk.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wsy.cashguo.top

[N06] 判断回文字符串
来源：http://kwp.svipenyu.cn

Py:   s == s[::-1]
来源：http://sui.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://ylz.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://hdg.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://djm.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ppf.sxryk.cn

Go:   // 双指针从两端比较
来源：http://xck.epnwcf.com

Ruby: s == s.reverse
来源：http://vim.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zkm.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://dnd.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yxc.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://awp.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mpk.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://hzp.xziqi.cn

Java: // 手写 HashMap
来源：http://epr.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://ucm.ppjwa.cn

Ruby: // 手写 Hash
来源：http://ipu.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://vvw.pengpengdd.cyou

[N08] 生成全排列
来源：http://mgw.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://kin.gzhubu.top

PHP:  // 手写递归交换
来源：http://seb.jyoumei.cn

JS:   // 手写回溯递归
来源：http://jwj.yuanzhike.top

TS:   // 手写回溯递归
来源：http://jye.zdbjq.cn

Java: // 手写回溯递归
来源：http://jil.mhx1999.top

Go:   // 手写回溯递归
来源：http://nzs.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://czv.cashguo.top

C#:   // 手写回溯递归
来源：http://fcj.jqgufenzy.top

[N09] 栈与队列
来源：http://hve.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rnu.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iui.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xyd.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qzo.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ghs.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bbp.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ygj.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jgq.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://zlz.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lte.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hce.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mto.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fjj.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://yam.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://guu.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lyh.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nsv.epnwcf.com

[N11] 二叉树中序遍历
来源：http://saq.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ezx.sysykeji.top

PHP:  // 手写递归函数
来源：http://akv.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqq.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cuj.nanxinkj.top

Java: // 手写递归
来源：http://rrp.9152youxi.cn

Go:   // 手写递归
来源：http://bei.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pkj.fktsv.cn

C#:   // 手写递归
来源：http://xir.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tly.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://taf.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ycf.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knh.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ise.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vgc.gaohongyu789.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oem.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://klm.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hee.yonumen.top

================================================================================
来源：http://szj.xuanzx.com

O. 并发与异步
来源：http://ukp.ydjk.org.cn

================================================================================
来源：http://rsi.cucudq.cn

[O01] 启动一个线程
来源：http://zge.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wmi.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ilr.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rgr.ydzc1.top

TS:   // 同 JS
来源：http://kqu.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://bwt.zhijiandao.cn

Go:   go f()
来源：http://cpc.hesvh.cn

Ruby: Thread.new { f }
来源：http://kxb.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://drf.316326.xyz

[O02] 使用线程池
来源：http://tob.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://woy.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mvh.zycfv.cn

JS:   // worker_threads 线程池
来源：http://wsa.xuanzx.com

TS:   // worker_threads 线程池
来源：http://omf.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://ada.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tua.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xyw.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aqt.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://mxk.yongpay.top

Py:   with lock: shared += 1
来源：http://scz.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://cdx.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lbl.zhiwuduotai.top

TS:   // 同 JS
来源：http://vck.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://lkv.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fii.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://axg.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://djo.tanke756.top

[O04] 定义异步函数并等待
来源：http://xfh.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://wqq.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qwc.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://ean.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vus.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rss.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cil.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://zbk.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://xxo.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://vja.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://bzm.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://klr.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://itw.cheryme.top

TS:   await Promise.all(tasks)
来源：http://xgu.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cpa.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjt.fehbvm.com

Ruby: threads.map(&:join)
来源：http://kzn.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sio.yuxming.cn


<!-- 参考信息 -->