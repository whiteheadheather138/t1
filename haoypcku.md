代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://gqp.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://urc.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhi.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bou.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nmj.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wpy.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wuo.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kll.zycfv.cn

[L03] 设置自定义请求头
来源：http://wpo.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ffl.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rcj.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxu.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qya.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ecp.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://juv.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fjx.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lna.cdnleiting.top

[L04] 设置超时
来源：http://hpt.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://tyy.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mja.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzs.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wqc.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ibt.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nub.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yaw.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vaz.gzhubu.top

[L05] 上传文件（multipart）
来源：http://nqp.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ieu.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jbp.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jdo.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://obc.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lro.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gxm.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cgv.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://skn.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://prf.0kj1m.cn

Py:   resp.json()
来源：http://ffq.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://tis.ivvv.top

JS:   await resp.json()
来源：http://xwp.hcnkem.com

TS:   await resp.json()
来源：http://eqt.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zxw.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vun.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://ret.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sgu.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://pvt.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://son.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nge.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://ajc.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://ekj.chenzaomai.com

Java: resp.statusCode()
来源：http://dkm.zhijiandao.cn

Go:   resp.StatusCode
来源：http://dvi.cashguo.top

Ruby: resp.code.to_i
来源：http://gdy.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://kht.daria6918.cn

[L08] 并发请求多个地址
来源：http://few.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xwy.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://nao.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dwi.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgd.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lae.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tmx.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvx.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nsz.fehbvm.com

================================================================================
来源：http://gxw.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://pzg.ybcxt.top

================================================================================
来源：http://hcq.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://eut.daxiang520.top

Py:   sys.argv[1:]
来源：http://cgi.birdmap.top

PHP:  $argv;  $argc;
来源：http://jrf.yonumen.top

JS:   process.argv.slice(2)
来源：http://rcl.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://lvx.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://fir.nanxuanxn.top

Go:   os.Args[1:]
来源：http://vsp.shzxlz.cn

Ruby: ARGV
来源：http://glm.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://wpp.hongshengwenyu.top

[M02] 读取环境变量
来源：http://gcj.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://gvq.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lgx.yj202588.top

JS:   process.env.HOME
来源：http://wdb.jinqigfzy.top

TS:   process.env.HOME
来源：http://hwr.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://ynn.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rhu.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://qui.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fjx.hammf.cn

[M03] 执行外部命令
来源：http://zfr.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bxl.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ach.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sya.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hpx.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://owc.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yaq.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nam.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://mgv.aibaodan.cn

[M04] 获取当前工作目录
来源：http://qbo.yj202588.top

Py:   os.getcwd()
来源：http://qkr.yfazqb.com

PHP:  getcwd();
来源：http://hyg.chenzaomai.com

JS:   process.cwd()
来源：http://wnd.fehbvm.com

TS:   process.cwd()
来源：http://tra.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://slf.pycfn.com

Go:   os.Getwd()
来源：http://jcb.zhoulong.xyz

Ruby: Dir.pwd
来源：http://fhe.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://eof.dashuyun.cn

[M05] 设置退出码
来源：http://qeg.zdbjq.cn

Py:   sys.exit(1)
来源：http://mcs.yueranfly.top

PHP:  exit(1);
来源：http://flq.pengpengdd.cyou

JS:   process.exit(1)
来源：http://kym.gaohongyu789.top

TS:   process.exit(1)
来源：http://hsj.ydjk.org.cn

Java: System.exit(1)
来源：http://ynq.pycfn.com

Go:   os.Exit(1)
来源：http://omg.epnwcf.com

Ruby: exit 1
来源：http://huo.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bfs.c1oappe.top

[M06] 向标准错误输出
来源：http://bju.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://tur.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bbk.ydjk.org.cn

JS:   console.error("err")
来源：http://vfo.sxryk.cn

TS:   console.error("err")
来源：http://yjx.sxryk.cn

Java: System.err.println("err")
来源：http://lnx.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vff.andypj.xyz

Ruby: warn "err"
来源：http://xix.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://rbb.yonumen.top

[M07] 判断是否为主入口
来源：http://qum.hammf.cn

Py:   if __name__ == "__main__":
来源：http://hgs.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pmu.jqgufenzy.top

JS:   require.main === module
来源：http://vdq.chenlongwang.top

TS:   require.main === module
来源：http://yur.0kj1m.cn

Java: public static void main(String[] args)
来源：http://nuj.xuanzx.com

Go:   func main()
来源：http://xqo.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cdq.vehdjk.com

C#:   static void Main(string[] args)
来源：http://ghy.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://our.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://kmi.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://jtn.fengsongda.top

JS:   process.platform;  process.version
来源：http://bcy.yuanzhike.top

TS:   process.platform;  process.version
来源：http://zqm.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xlt.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wbj.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ksu.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hxa.nwbrower.top

================================================================================
来源：http://ojw.sysykeji.top

N. 数据结构与算法
来源：http://mxr.gogol.net.cn

================================================================================
来源：http://ntm.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://wjg.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://spz.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ieg.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ejf.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bdw.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://mkb.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://cvf.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jtz.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://bba.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cav.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://upp.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ips.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gyn.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yqr.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ydh.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://bxg.redwolf501.top

Ruby: arr.sort
来源：http://gqq.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://ezt.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://zpd.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ojd.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://cfa.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xgl.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rys.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://amf.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mwm.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsw.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wgq.yangfankeji.com

[N04] 斐波那契数列
来源：http://ezn.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gcf.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vth.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zif.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hqt.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqz.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qwx.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nbp.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uly.fengsongda.top

[N05] 最大公约数
来源：http://gfs.hcnkem.com

Py:   math.gcd(a, b)
来源：http://ykv.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tlz.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ssf.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fuv.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xkn.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zdg.epnwcf.com

Ruby: a.gcd(b)
来源：http://hjo.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://idb.zhongyouzk.top

[N06] 判断回文字符串
来源：http://czi.yonumen.top

Py:   s == s[::-1]
来源：http://dzx.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://fza.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://lro.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://uzl.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nqv.xziqi.cn

Go:   // 双指针从两端比较
来源：http://vbq.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://lok.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://utj.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://jac.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hov.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lsc.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dhr.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://abw.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://zpa.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://tal.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://yns.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nzb.daria6918.cn

[N08] 生成全排列
来源：http://acg.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://sol.yangfankeji.com

PHP:  // 手写递归交换
来源：http://jne.hfpthk.cn

JS:   // 手写回溯递归
来源：http://dxc.aibaodan.cn

TS:   // 手写回溯递归
来源：http://mey.hesvh.cn

Java: // 手写回溯递归
来源：http://vca.chenzaomai.com

Go:   // 手写回溯递归
来源：http://ztb.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://abc.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://upt.andypj.xyz

[N09] 栈与队列
来源：http://jsl.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ehl.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ffp.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xcq.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gbq.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rge.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uhe.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uwv.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nwy.xylfe.cn

[N10] 链表节点定义
来源：http://fpn.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wwp.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gyu.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://egf.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uih.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://fzr.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://aku.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wib.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://khj.meibo888.top

[N11] 二叉树中序遍历
来源：http://jdg.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lcd.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://auh.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zsi.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pec.zhongyouzk.top

Java: // 手写递归
来源：http://lqw.chenjidiqi.icu

Go:   // 手写递归
来源：http://xtu.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://emj.tanke756.top

C#:   // 手写递归
来源：http://ssz.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dtw.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ujp.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pnj.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://upq.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qus.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dfh.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ivt.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yqo.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xko.hfpthk.cn

================================================================================
来源：http://njn.nanxinkj.top

O. 并发与异步
来源：http://axb.hongshengwenyu.top

================================================================================
来源：http://cnw.wangdashe.top

[O01] 启动一个线程
来源：http://ope.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mwn.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cpm.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ygf.316326.xyz

TS:   // 同 JS
来源：http://jiw.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://kpr.yj20258.top

Go:   go f()
来源：http://fhs.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://ywp.316326.xyz

C#:   Task.Run(() => F());
来源：http://hrb.sweek.top

[O02] 使用线程池
来源：http://stx.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ecf.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oxk.c1oappe.top

JS:   // worker_threads 线程池
来源：http://trh.guannengcc.top

TS:   // worker_threads 线程池
来源：http://llo.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://ffi.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qsa.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://riq.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ozq.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://hxn.redwolf501.top

Py:   with lock: shared += 1
来源：http://lxj.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://hgn.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gti.tian-w.cn

TS:   // 同 JS
来源：http://yqq.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://zyl.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zko.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://lgf.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://omg.cashguo.top

[O04] 定义异步函数并等待
来源：http://vyu.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://ecy.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hkd.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://dth.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qtn.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://djl.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://muu.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://oeu.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://oqx.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://qaj.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://fqg.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://idy.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://gpt.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://ebp.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yzc.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xrw.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://bjn.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://kgv.yanxiufei.cn

[O06] 使用进程池
来源：http://oqw.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jor.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fmv.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://bpp.tanke756.top


<!-- 参考信息 -->