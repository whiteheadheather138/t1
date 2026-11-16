代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://fwz.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dzu.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://svq.sufxvd.cn

[L02] 发送 POST JSON
来源：http://ozw.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://uiy.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wwd.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bjx.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jil.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jrb.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ffo.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ddn.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qmo.jiagoushi.top

[L03] 设置自定义请求头
来源：http://afz.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wtw.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xyd.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://snj.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://smo.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://koq.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://utv.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ysv.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jfv.gzhubu.top

[L04] 设置超时
来源：http://qeh.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://oqk.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mya.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iya.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://krx.yanxiufei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fmb.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kgq.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wsz.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nzl.ivvv.top

[L05] 上传文件（multipart）
来源：http://igo.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lby.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cgj.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gjw.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yln.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tlj.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xma.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lfg.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsm.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://ksl.sjlbkw.cn

Py:   resp.json()
来源：http://azx.wangdashe.top

PHP:  json_decode($body, true);
来源：http://qdj.fanxiaobao.xyz

JS:   await resp.json()
来源：http://pji.zhixingplan.top

TS:   await resp.json()
来源：http://tlh.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iuq.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qvi.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://sid.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pax.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://cuv.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pna.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzr.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://nyj.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://bgu.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://uow.c1oappe.top

Go:   resp.StatusCode
来源：http://vbl.xinyue.icu

Ruby: resp.code.to_i
来源：http://swo.pycfn.com

C#:   (int)resp.StatusCode
来源：http://mrc.hywenlv.cn

[L08] 并发请求多个地址
来源：http://dwb.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kjj.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://qjb.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mls.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://are.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tuv.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://syw.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nwc.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oxl.uphjek.com

================================================================================
来源：http://gpe.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://jmc.gogol.net.cn

================================================================================
来源：http://jkl.cheryme.top

[M01] 读取命令行参数
来源：http://nah.tianlin.xyz

Py:   sys.argv[1:]
来源：http://qjb.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://iqk.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://esn.yfazqb.com

TS:   process.argv.slice(2)
来源：http://hva.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://bkb.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://mzc.jinqigufen.top

Ruby: ARGV
来源：http://anl.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://vsk.yonumen.top

[M02] 读取环境变量
来源：http://rsx.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://hlx.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yjg.jinqigfzy.top

JS:   process.env.HOME
来源：http://ynu.daria6918.cn

TS:   process.env.HOME
来源：http://ggu.jinqigufen.top

Java: System.getenv("HOME")
来源：http://gxq.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nzc.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://pum.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uyd.sjlbkw.cn

[M03] 执行外部命令
来源：http://cqy.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qaw.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vnr.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cca.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://yep.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fwr.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oji.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://otu.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://chj.jianghu66.top

[M04] 获取当前工作目录
来源：http://ddm.gzhubu.top

Py:   os.getcwd()
来源：http://ilg.yj202588.top

PHP:  getcwd();
来源：http://ekr.gzhubu.top

JS:   process.cwd()
来源：http://pgh.ppjwa.cn

TS:   process.cwd()
来源：http://wse.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://xfh.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://mhx.yj20258.top

Ruby: Dir.pwd
来源：http://ysu.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://czm.zhixingplan.top

[M05] 设置退出码
来源：http://ftj.nanxuanxn.top

Py:   sys.exit(1)
来源：http://ayv.feifeiyinyue.top

PHP:  exit(1);
来源：http://sny.sxryk.cn

JS:   process.exit(1)
来源：http://kqi.mhx1999.top

TS:   process.exit(1)
来源：http://rpm.quarkkingdee.top

Java: System.exit(1)
来源：http://xzp.gzhubu.top

Go:   os.Exit(1)
来源：http://bbh.hammf.cn

Ruby: exit 1
来源：http://ksp.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wga.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://hcr.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://xjf.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ciu.cucudq.cn

JS:   console.error("err")
来源：http://dzd.nanxuanxn.top

TS:   console.error("err")
来源：http://isv.mhx1999.top

Java: System.err.println("err")
来源：http://xeo.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mew.9152youxi.cn

Ruby: warn "err"
来源：http://qnl.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://jkc.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://vlw.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://rco.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zzz.xuanzx.com

JS:   require.main === module
来源：http://vjh.ctjpmb.com

TS:   require.main === module
来源：http://foy.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://pzz.zhengqikj.top

Go:   func main()
来源：http://jcy.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kdl.daxiang520.top

C#:   static void Main(string[] args)
来源：http://tfp.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://auf.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://cdt.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://mrk.zhengqikj.top

JS:   process.platform;  process.version
来源：http://mnx.jiagoushi.top

TS:   process.platform;  process.version
来源：http://xgo.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rmm.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wop.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lse.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vte.epnwcf.com

================================================================================
来源：http://sra.ydjk.org.cn

N. 数据结构与算法
来源：http://vvp.chenzaomai.com

================================================================================
来源：http://nwb.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://tia.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://acu.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cwk.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xpq.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eod.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xdb.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://cbh.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yas.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jqh.ywan-chungtsiang.top

[N02] 排序（工程实践用内置实现）
来源：http://xcs.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://lnd.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ufc.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pbt.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dfe.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zgr.sxryk.cn

Go:   slices.Sort(arr)
来源：http://yfa.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://qca.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ssu.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://rrz.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ebw.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://nky.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbn.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://igh.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vhj.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gif.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tnf.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://iue.hywenlv.cn

[N04] 斐波那契数列
来源：http://jtw.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zqd.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzq.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fhc.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dye.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oum.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://taq.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uqo.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fyl.52xcode.cn

[N05] 最大公约数
来源：http://erw.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://znv.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ahv.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xhg.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfb.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hrq.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dop.yvedp.cn

Ruby: a.gcd(b)
来源：http://gmj.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dll.mhx1999.top

[N06] 判断回文字符串
来源：http://uej.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://nyg.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://teo.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://qcj.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://snd.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qgz.sysykeji.top

Go:   // 双指针从两端比较
来源：http://xwk.zhixingplan.top

Ruby: s == s.reverse
来源：http://msc.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://ghl.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://uag.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mpg.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bbt.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yup.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://qxy.snrcjt.cn

Java: // 手写 HashMap
来源：http://zny.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://gha.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://xfl.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mho.hnxiangtu.top

[N08] 生成全排列
来源：http://gon.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://esx.hywenlv.cn

PHP:  // 手写递归交换
来源：http://yco.yfazqb.com

JS:   // 手写回溯递归
来源：http://exs.chenlongwang.top

TS:   // 手写回溯递归
来源：http://ecs.tian-w.cn

Java: // 手写回溯递归
来源：http://fpx.nanxinkj.top

Go:   // 手写回溯递归
来源：http://nzb.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://hgp.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://ojy.redwolf501.top

[N09] 栈与队列
来源：http://qqj.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pgm.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nvz.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yhi.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aai.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vcx.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fkt.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lnn.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yvw.yvedp.cn

[N10] 链表节点定义
来源：http://pre.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cle.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://zqu.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aef.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqq.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://hpj.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://hpt.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hkd.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jft.guannengcc.top

[N11] 二叉树中序遍历
来源：http://uin.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://luv.andypj.xyz

PHP:  // 手写递归函数
来源：http://eqp.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mip.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjk.jqgufenzy.top

Java: // 手写递归
来源：http://txr.redwolf501.top

Go:   // 手写递归
来源：http://kyu.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xdl.cqqwz.cn

C#:   // 手写递归
来源：http://exi.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vzq.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kgl.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://svz.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iuu.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qyo.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ani.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://stw.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jqp.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uce.ydzc1.top

================================================================================
来源：http://jsb.nwbrower.top

O. 并发与异步
来源：http://wrl.nanxuanxn.top

================================================================================
来源：http://xmm.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://unt.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dcz.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iel.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vum.wangdashe.top

TS:   // 同 JS
来源：http://dkm.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://ctq.jinyuanbaomall.cn

Go:   go f()
来源：http://zbs.yfazqb.com

Ruby: Thread.new { f }
来源：http://zru.316326.xyz

C#:   Task.Run(() => F());
来源：http://bej.yangfankeji.com

[O02] 使用线程池
来源：http://zfj.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mwd.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qdv.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://gxj.hesvh.cn

TS:   // worker_threads 线程池
来源：http://cht.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://glf.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kaz.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://clo.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zeg.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://rji.nwbrower.top

Py:   with lock: shared += 1
来源：http://nul.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://qie.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://coc.xuanzx.com

TS:   // 同 JS
来源：http://jso.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://kep.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gen.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://biv.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://goj.xylfe.cn

[O04] 定义异步函数并等待
来源：http://mhd.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://pvf.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qxf.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://qnr.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://wbc.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iqr.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ugb.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://uiy.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://qlo.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://bin.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://sea.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dvi.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://wpk.yj20258.top

TS:   await Promise.all(tasks)
来源：http://zyb.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lex.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nxl.mhx1999.top

Ruby: threads.map(&:join)
来源：http://khn.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rsz.haohaochexian.top


<!-- 参考信息 -->