代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://xkl.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gdv.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xkt.yj20258888.top

[L02] 发送 POST JSON
来源：http://xbe.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://uxg.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ajx.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfx.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfr.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ltl.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wez.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mpo.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://axt.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://ajl.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dtb.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rms.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yur.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://llb.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wnc.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kpb.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aay.c1oappe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nyx.yanxiufei.cn

[L04] 设置超时
来源：http://tcu.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://iyu.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fot.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lhp.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sul.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qvq.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hmy.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://luk.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hsu.ivvv.top

[L05] 上传文件（multipart）
来源：http://syy.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hjg.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ftm.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xmr.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nfl.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dzn.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oka.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ckj.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qid.jianghu66.top

[L06] 解析响应为 JSON
来源：http://ruy.sufxvd.cn

Py:   resp.json()
来源：http://rjx.jianghu66.top

PHP:  json_decode($body, true);
来源：http://hdm.hnqzz.top

JS:   await resp.json()
来源：http://rcj.nwbrower.top

TS:   await resp.json()
来源：http://hrg.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fyd.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pso.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://rbh.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rmx.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://emd.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yti.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://btu.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://xqp.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://okq.cqqwz.cn

Java: resp.statusCode()
来源：http://xom.jqgufenzy.top

Go:   resp.StatusCode
来源：http://zky.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://liy.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://vhk.cdnleiting.top

[L08] 并发请求多个地址
来源：http://zlb.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hrx.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://mxl.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfn.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jai.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sxh.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rvv.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iqd.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gzq.yfazqb.com

================================================================================
来源：http://hcf.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://xma.mhx1999.top

================================================================================
来源：http://hjh.cheryme.top

[M01] 读取命令行参数
来源：http://awb.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://blo.nwbrower.top

PHP:  $argv;  $argc;
来源：http://bwv.ivvv.top

JS:   process.argv.slice(2)
来源：http://hhm.yfazqb.com

TS:   process.argv.slice(2)
来源：http://fpn.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://jxd.yongpay.top

Go:   os.Args[1:]
来源：http://hph.yongpay.top

Ruby: ARGV
来源：http://xbi.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://qeb.mhx1999.top

[M02] 读取环境变量
来源：http://xlt.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://sea.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mul.zhijiandao.cn

JS:   process.env.HOME
来源：http://jxl.dashuyun.cn

TS:   process.env.HOME
来源：http://olm.yueranfly.top

Java: System.getenv("HOME")
来源：http://qbm.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://chr.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://zby.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zze.xuanzx.com

[M03] 执行外部命令
来源：http://mht.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ysa.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://guu.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bof.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://lnw.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xgn.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qcf.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gxg.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://kzr.haohaochexian.top

[M04] 获取当前工作目录
来源：http://ogs.yanxiufei.cn

Py:   os.getcwd()
来源：http://nrm.fehbvm.com

PHP:  getcwd();
来源：http://rhk.yongpay.top

JS:   process.cwd()
来源：http://uex.ydjk.org.cn

TS:   process.cwd()
来源：http://mbn.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://blh.cqqwz.cn

Go:   os.Getwd()
来源：http://eey.hnxiangtu.top

Ruby: Dir.pwd
来源：http://kol.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nnz.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://wyt.havefunace.top

Py:   sys.exit(1)
来源：http://lwb.zhoulong.xyz

PHP:  exit(1);
来源：http://ark.316326.xyz

JS:   process.exit(1)
来源：http://rhh.nanxinkj.top

TS:   process.exit(1)
来源：http://gnc.guannengcc.top

Java: System.exit(1)
来源：http://kws.meibo888.top

Go:   os.Exit(1)
来源：http://pmi.ydzc1.top

Ruby: exit 1
来源：http://rif.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://itl.dianchejie.cn

[M06] 向标准错误输出
来源：http://qip.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://yhx.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lip.yvedp.cn

JS:   console.error("err")
来源：http://jsq.316326.xyz

TS:   console.error("err")
来源：http://qad.smart0.xyz

Java: System.err.println("err")
来源：http://tex.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tnr.yj202588.top

Ruby: warn "err"
来源：http://ggw.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://qao.yonumen.top

[M07] 判断是否为主入口
来源：http://qsq.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://rpr.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xug.sweek.top

JS:   require.main === module
来源：http://xjc.9152youxi.cn

TS:   require.main === module
来源：http://lrr.redwolf501.top

Java: public static void main(String[] args)
来源：http://yhk.xziqi.cn

Go:   func main()
来源：http://mrv.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rlm.birdmap.top

C#:   static void Main(string[] args)
来源：http://gfy.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://qum.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://qqx.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://kym.xziqi.cn

JS:   process.platform;  process.version
来源：http://ajc.daxiang520.top

TS:   process.platform;  process.version
来源：http://nam.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://reb.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ils.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qhj.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tjy.daria6918.cn

================================================================================
来源：http://kdi.hywenlv.cn

N. 数据结构与算法
来源：http://iyn.ppjwa.cn

================================================================================
来源：http://cii.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://ttg.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://rfg.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zxc.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nud.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rez.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://unt.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://ofb.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yfz.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://xpj.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://vxg.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://msf.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zrz.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://myh.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ixn.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nuw.xinyue.icu

Go:   slices.Sort(arr)
来源：http://jki.pengpengdd.cyou

Ruby: arr.sort
来源：http://kcc.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tmk.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://rgt.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cmq.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://ihs.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghg.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sje.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://urz.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dlr.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://maf.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bft.zdbjq.cn

[N04] 斐波那契数列
来源：http://nix.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ptb.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kyu.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nrk.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ala.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dnf.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xtn.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aux.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cgt.redwolf501.top

[N05] 最大公约数
来源：http://sfa.andypj.xyz

Py:   math.gcd(a, b)
来源：http://fba.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jjw.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmu.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghw.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gya.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hba.yangfankeji.com

Ruby: a.gcd(b)
来源：http://jzw.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zrn.tanke756.top

[N06] 判断回文字符串
来源：http://gup.yvedp.cn

Py:   s == s[::-1]
来源：http://glh.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://luy.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://zgk.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://qhr.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yyh.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://fkm.ctjpmb.com

Ruby: s == s.reverse
来源：http://ndt.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://chn.yj202588.top

[N07] 两数之和（返回下标）
来源：http://pmd.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://paz.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://myu.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fbb.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://pdg.meibo888.top

Java: // 手写 HashMap
来源：http://bho.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://nsm.gogol.net.cn

Ruby: // 手写 Hash
来源：http://waf.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://soe.c1oappe.top

[N08] 生成全排列
来源：http://yyj.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://hzn.sysykeji.top

PHP:  // 手写递归交换
来源：http://bwr.sxryk.cn

JS:   // 手写回溯递归
来源：http://cml.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://vpi.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://zla.yongpay.top

Go:   // 手写回溯递归
来源：http://wbd.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://qjr.cashguo.top

C#:   // 手写回溯递归
来源：http://xys.pycfn.com

[N09] 栈与队列
来源：http://ttc.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ddd.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfs.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://btz.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jcl.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pfo.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://twc.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tqf.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bro.quarkkingdee.top

[N10] 链表节点定义
来源：http://wdj.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ygf.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://epc.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dzt.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kta.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://ggi.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://jrn.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hmd.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qzn.vehdjk.com

[N11] 二叉树中序遍历
来源：http://jqt.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tix.fehbvm.com

PHP:  // 手写递归函数
来源：http://zcp.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iry.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://myk.hywenlv.cn

Java: // 手写递归
来源：http://azp.shzxlz.cn

Go:   // 手写递归
来源：http://rmi.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cqt.zdbjq.cn

C#:   // 手写递归
来源：http://jgl.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zzx.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xoo.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kzm.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjs.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfx.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hkm.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://psu.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://owy.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://puh.ivvv.top

================================================================================
来源：http://rro.redwolf501.top

O. 并发与异步
来源：http://jbx.feifeiyinyue.top

================================================================================
来源：http://too.yvedp.cn

[O01] 启动一个线程
来源：http://txb.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uel.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ywu.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jig.jianghu66.top

TS:   // 同 JS
来源：http://fpg.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://ych.ydjk.org.cn

Go:   go f()
来源：http://flg.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://rwz.ybcxt.top

C#:   Task.Run(() => F());
来源：http://uoh.fehbvm.com

[O02] 使用线程池
来源：http://iwt.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://snt.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ykk.iojbl.cn

JS:   // worker_threads 线程池
来源：http://auu.yongpay.top

TS:   // worker_threads 线程池
来源：http://akt.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://hpb.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bos.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://npi.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sdf.havefunace.top

[O03] 加锁保护共享数据
来源：http://rvp.gotoacloud.top

Py:   with lock: shared += 1
来源：http://ozp.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://vyp.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sue.shzxlz.cn

TS:   // 同 JS
来源：http://uaa.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://zpj.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xgi.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vpc.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://drv.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://bof.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://pqp.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ywe.bbcook.cn

JS:   async function f() { await g(); }
来源：http://iav.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cwe.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://icb.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mha.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://nze.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://zxw.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://fzm.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://fnl.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dox.hammf.cn

JS:   await Promise.all(tasks)
来源：http://qtg.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://nma.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rax.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cvd.gzhubu.top

Ruby: threads.map(&:join)
来源：http://fjp.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iid.chenjidiqi.icu


<!-- 参考信息 -->