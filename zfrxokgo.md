代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lsk.xziqi.cn

JS:   await fetch(url)
来源：http://xgq.yj20258888.top

TS:   await fetch(url)
来源：http://jjz.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nza.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://dhg.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://asf.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gju.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://fny.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://srd.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nia.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://smb.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nia.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqb.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jou.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ufr.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cid.zdbjq.cn

[L03] 设置自定义请求头
来源：http://avw.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gzh.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xib.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eue.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xlr.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nsd.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qmz.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eub.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sqm.chenzaomai.com

[L04] 设置超时
来源：http://ovs.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://atf.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jok.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fsv.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ilu.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ljs.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vjx.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qbe.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dlj.yj202588.top

[L05] 上传文件（multipart）
来源：http://wkd.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cyl.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dar.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qbg.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uqj.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ztw.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qnu.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yud.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gxk.redwolf501.top

[L06] 解析响应为 JSON
来源：http://rbb.xuetiantiany.cn

Py:   resp.json()
来源：http://rxx.hcnkem.com

PHP:  json_decode($body, true);
来源：http://cou.zhongyouzk.top

JS:   await resp.json()
来源：http://ngg.xziqi.cn

TS:   await resp.json()
来源：http://fjq.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wyv.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mwf.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://jhp.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bwy.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://nle.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zqx.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://enn.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://nar.cashguo.top

TS:   resp.ok;  resp.status
来源：http://atw.haohaochexian.top

Java: resp.statusCode()
来源：http://xbp.zhixingplan.top

Go:   resp.StatusCode
来源：http://fkj.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://phi.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://geo.dianchejie.cn

[L08] 并发请求多个地址
来源：http://uym.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hrs.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://ack.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmm.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ses.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zfk.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iyc.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ckf.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://syt.gaohongyu789.top

================================================================================
来源：http://hnr.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://abk.kuanghao11.cn

================================================================================
来源：http://zwv.yuanzhike.top

[M01] 读取命令行参数
来源：http://waa.ehwqpu.com

Py:   sys.argv[1:]
来源：http://wht.havefunace.top

PHP:  $argv;  $argc;
来源：http://yrg.shuidangran.top

JS:   process.argv.slice(2)
来源：http://ubu.tarul.cn

TS:   process.argv.slice(2)
来源：http://dgc.tanke756.top

Java: args 数组（main 方法参数）
来源：http://jnz.hesvh.cn

Go:   os.Args[1:]
来源：http://jrv.zhoulong.xyz

Ruby: ARGV
来源：http://qsw.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://ijc.cucudq.cn

[M02] 读取环境变量
来源：http://fnq.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://ecr.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rfl.yueranfly.top

JS:   process.env.HOME
来源：http://zpo.jlsjyb.cn

TS:   process.env.HOME
来源：http://dbx.fengsongda.top

Java: System.getenv("HOME")
来源：http://ecj.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bhm.yj20258.top

Ruby: ENV["HOME"]
来源：http://uar.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gzo.hysaishi.cn

[M03] 执行外部命令
来源：http://fsv.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eiq.shzxlz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qnn.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jlx.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://sli.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hcz.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://myg.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bjq.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://ymp.hnqzz.top

[M04] 获取当前工作目录
来源：http://kxu.ydjk.org.cn

Py:   os.getcwd()
来源：http://sfe.zhixingplan.top

PHP:  getcwd();
来源：http://qvu.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://xnz.fengsongda.top

TS:   process.cwd()
来源：http://drp.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://epl.fehbvm.com

Go:   os.Getwd()
来源：http://jzf.gogol.net.cn

Ruby: Dir.pwd
来源：http://iid.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wey.hfpthk.cn

[M05] 设置退出码
来源：http://ltl.tarul.cn

Py:   sys.exit(1)
来源：http://msf.jqgfzy.top

PHP:  exit(1);
来源：http://kxc.yanxiufei.cn

JS:   process.exit(1)
来源：http://ktq.yj20258888.top

TS:   process.exit(1)
来源：http://fpt.yonumen.top

Java: System.exit(1)
来源：http://tmt.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://nar.gotoacloud.top

Ruby: exit 1
来源：http://vpx.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rzw.zhixingplan.top

[M06] 向标准错误输出
来源：http://kuq.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://ufq.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://edh.zhijiandao.cn

JS:   console.error("err")
来源：http://nqb.gotoacloud.top

TS:   console.error("err")
来源：http://qqh.nwbrower.top

Java: System.err.println("err")
来源：http://mus.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nsa.tian-w.cn

Ruby: warn "err"
来源：http://btw.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://esd.havefunace.top

[M07] 判断是否为主入口
来源：http://vfl.yj20258.top

Py:   if __name__ == "__main__":
来源：http://wqf.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tsk.ywan-chungtsiang.top

JS:   require.main === module
来源：http://ovl.kuanghao11.cn

TS:   require.main === module
来源：http://kju.zdqjudy.top

Java: public static void main(String[] args)
来源：http://tis.gogol.net.cn

Go:   func main()
来源：http://nob.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pvm.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://yth.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://fhg.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://agl.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://smi.vehdjk.com

JS:   process.platform;  process.version
来源：http://ecf.zycfv.cn

TS:   process.platform;  process.version
来源：http://bmq.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ecr.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kiy.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aeb.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jhk.nanxinkj.top

================================================================================
来源：http://rpl.bbcook.cn

N. 数据结构与算法
来源：http://rbj.jianghu66.top

================================================================================
来源：http://nzd.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://zaw.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://qkl.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gld.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sao.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rsf.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://cci.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://evd.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tbe.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://xnl.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://jnq.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://nkm.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ptm.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://ejd.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://flb.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ijt.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://pac.aibaodan.cn

Ruby: arr.sort
来源：http://jkm.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukq.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://gxr.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dre.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://csf.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://svx.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bck.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://plb.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vtf.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mmj.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gjv.c1oappe.top

[N04] 斐波那契数列
来源：http://xdg.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dzo.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cjj.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://krx.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbf.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://egw.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xfj.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zrn.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://axf.aizwys.cn

[N05] 最大公约数
来源：http://jrw.pycfn.com

Py:   math.gcd(a, b)
来源：http://ups.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fpf.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iqh.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jso.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ikx.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bug.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://vea.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kxe.dianchejie.cn

[N06] 判断回文字符串
来源：http://qis.sufxvd.cn

Py:   s == s[::-1]
来源：http://sph.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://zif.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://omf.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://fox.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qsw.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://qlg.xinyue.icu

Ruby: s == s.reverse
来源：http://wsl.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uha.meibo888.top

[N07] 两数之和（返回下标）
来源：http://fvt.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pyz.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lxk.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ybn.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://beb.tanke756.top

Java: // 手写 HashMap
来源：http://hlt.yfazqb.com

Go:   // 手写 map[int]int
来源：http://qbp.ppjwa.cn

Ruby: // 手写 Hash
来源：http://evy.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zwz.zhijiandao.cn

[N08] 生成全排列
来源：http://xwu.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://eac.sxryk.cn

PHP:  // 手写递归交换
来源：http://tqw.fengsongda.top

JS:   // 手写回溯递归
来源：http://yov.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://hrb.xziqi.cn

Java: // 手写回溯递归
来源：http://eyq.cheryme.top

Go:   // 手写回溯递归
来源：http://bvy.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://gyy.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://yoi.chenjidiqi.icu

[N09] 栈与队列
来源：http://hga.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wwr.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cvi.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xgh.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjt.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jko.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dqq.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zxm.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wtw.ydzc1.top

[N10] 链表节点定义
来源：http://sny.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ytg.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mkb.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rfy.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dkk.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://zgd.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fmf.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dfn.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xso.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://lez.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lkc.epnwcf.com

PHP:  // 手写递归函数
来源：http://dya.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxz.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kej.9152youxi.cn

Java: // 手写递归
来源：http://vbd.bbcook.cn

Go:   // 手写递归
来源：http://jio.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vuz.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://swn.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cji.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://chs.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qdn.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://avd.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxo.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ckv.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uvu.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dra.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://msp.52xcode.cn

================================================================================
来源：http://dso.tanke756.top

O. 并发与异步
来源：http://bgy.yangfankeji.com

================================================================================
来源：http://gku.yanxiufei.cn

[O01] 启动一个线程
来源：http://iyu.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lbj.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ymq.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://msg.hnxiangtu.top

TS:   // 同 JS
来源：http://zwz.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://vxy.xylfe.cn

Go:   go f()
来源：http://rfd.bjfxy.top

Ruby: Thread.new { f }
来源：http://ayb.birdmap.top

C#:   Task.Run(() => F());
来源：http://tka.sysykeji.top

[O02] 使用线程池
来源：http://hxy.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yyr.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tqx.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://tpg.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://pfa.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sxd.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qwm.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yxz.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ace.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://qhl.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://xju.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://ocq.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wcr.gotoacloud.top

TS:   // 同 JS
来源：http://nrv.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://msq.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rcg.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://odd.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://vpd.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://ptb.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://hcm.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hnh.nwbrower.top

JS:   async function f() { await g(); }
来源：http://hxf.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qix.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vga.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kfd.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://yya.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://lnz.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://mab.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://upg.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ety.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://rlz.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://rov.gaohongyu789.top


<!-- 参考信息 -->