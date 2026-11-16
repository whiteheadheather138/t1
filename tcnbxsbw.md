代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://uxf.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qge.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdi.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wlt.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://utc.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rbe.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uqa.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lqo.aibaodan.cn

[L03] 设置自定义请求头
来源：http://vvd.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blx.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://crk.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uru.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wss.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fak.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vxc.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eav.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ixe.zhongyouzk.top

[L04] 设置超时
来源：http://ifm.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://svc.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oeb.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwb.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wyl.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lse.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uwo.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://voe.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cwf.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://hxg.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rsf.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cmb.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ief.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cuk.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qmu.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lhs.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bgo.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xnn.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://ema.xuanzx.com

Py:   resp.json()
来源：http://pcw.sysykeji.top

PHP:  json_decode($body, true);
来源：http://qns.nanxinkj.top

JS:   await resp.json()
来源：http://tdi.aizwys.cn

TS:   await resp.json()
来源：http://jsq.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jvt.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://avc.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://osj.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fhq.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://ohd.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tfd.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://exm.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://cir.yongpay.top

TS:   resp.ok;  resp.status
来源：http://oqz.yueranfly.top

Java: resp.statusCode()
来源：http://wzo.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://gce.hesvh.cn

Ruby: resp.code.to_i
来源：http://gua.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://lur.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://cvl.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pxd.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://yce.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tbw.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jew.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rya.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rxf.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kkx.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qwl.gzhubu.top

================================================================================
来源：http://wxt.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ynw.shzxlz.cn

================================================================================
来源：http://aku.jqgufenzy.top

[M01] 读取命令行参数
来源：http://qeu.hfpthk.cn

Py:   sys.argv[1:]
来源：http://gtj.epnwcf.com

PHP:  $argv;  $argc;
来源：http://qva.yj20258888.top

JS:   process.argv.slice(2)
来源：http://azz.yj202588.top

TS:   process.argv.slice(2)
来源：http://hnm.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://sfa.tarul.cn

Go:   os.Args[1:]
来源：http://aod.zhiwuduotai.top

Ruby: ARGV
来源：http://jjj.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://qhu.yanxiufei.cn

[M02] 读取环境变量
来源：http://bhn.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://sjf.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://egt.cucudq.cn

JS:   process.env.HOME
来源：http://iny.xylfe.cn

TS:   process.env.HOME
来源：http://qhu.ydzc1.top

Java: System.getenv("HOME")
来源：http://wzp.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vfp.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://iba.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ndj.yuanzhike.top

[M03] 执行外部命令
来源：http://peb.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xom.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://atx.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rsz.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gwa.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lvm.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eyi.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://dkj.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://unt.tianlin.xyz

[M04] 获取当前工作目录
来源：http://spi.fehbvm.com

Py:   os.getcwd()
来源：http://skw.cheryme.top

PHP:  getcwd();
来源：http://oiw.yj20258.top

JS:   process.cwd()
来源：http://ufh.zdqjudy.top

TS:   process.cwd()
来源：http://rji.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://trm.jianghu66.top

Go:   os.Getwd()
来源：http://dcg.quarkkingdee.top

Ruby: Dir.pwd
来源：http://vgo.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xkx.jiagoushi.top

[M05] 设置退出码
来源：http://hpu.cashguo.top

Py:   sys.exit(1)
来源：http://otc.pengpengdd.cyou

PHP:  exit(1);
来源：http://cdn.aibaodan.cn

JS:   process.exit(1)
来源：http://vya.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://dcw.guowangkeji.top

Java: System.exit(1)
来源：http://kvj.fengsongda.top

Go:   os.Exit(1)
来源：http://cuy.epnwcf.com

Ruby: exit 1
来源：http://col.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://egf.jianghu66.top

[M06] 向标准错误输出
来源：http://giz.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://vbv.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ewc.havefunace.top

JS:   console.error("err")
来源：http://lgh.chenzaomai.com

TS:   console.error("err")
来源：http://grz.dashuyun.cn

Java: System.err.println("err")
来源：http://nsx.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cip.ydzc1.top

Ruby: warn "err"
来源：http://bux.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://pbq.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://aoz.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://wge.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jqz.xylfe.cn

JS:   require.main === module
来源：http://oxf.daxiang520.top

TS:   require.main === module
来源：http://usq.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://ziz.redwolf501.top

Go:   func main()
来源：http://xze.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yen.hammf.cn

C#:   static void Main(string[] args)
来源：http://dzd.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://fue.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://vhu.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://lob.bbcook.cn

JS:   process.platform;  process.version
来源：http://kpi.tianlin.xyz

TS:   process.platform;  process.version
来源：http://dod.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xky.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jun.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xyg.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://frk.jinqigufen.top

================================================================================
来源：http://tqy.9152youxi.cn

N. 数据结构与算法
来源：http://tvr.yj202588.top

================================================================================
来源：http://rfg.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://pib.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bgj.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tot.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfe.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oga.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://wgu.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://qjt.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dhg.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xve.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://cjv.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://ykr.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://guq.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxu.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nmc.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mai.hcnkem.com

Go:   slices.Sort(arr)
来源：http://kxy.yj20258888.top

Ruby: arr.sort
来源：http://dya.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lhp.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://spo.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zds.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://tpc.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pos.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jky.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ecb.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dfz.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pir.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://tbm.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://aeo.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tyr.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nog.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fux.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vjw.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ywr.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pxs.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vom.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zzj.xylfe.cn

[N05] 最大公约数
来源：http://kaa.xziqi.cn

Py:   math.gcd(a, b)
来源：http://hve.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lra.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ktc.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ony.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ods.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iuf.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://mtq.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpt.zycfv.cn

[N06] 判断回文字符串
来源：http://jxd.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://vmj.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://bre.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://gsp.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://rrj.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tbx.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://vfi.dashuyun.cn

Ruby: s == s.reverse
来源：http://tda.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://izc.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://cxh.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wkj.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hdh.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fac.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://sew.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://khs.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://gtv.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://tcn.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jbr.smart0.xyz

[N08] 生成全排列
来源：http://uyy.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://oay.ivvv.top

PHP:  // 手写递归交换
来源：http://thx.zhixingplan.top

JS:   // 手写回溯递归
来源：http://kvw.vehdjk.com

TS:   // 手写回溯递归
来源：http://paj.jyoumei.cn

Java: // 手写回溯递归
来源：http://lbq.316326.xyz

Go:   // 手写回溯递归
来源：http://xaf.tarul.cn

Ruby: arr.permutation.to_a
来源：http://ayg.cashguo.top

C#:   // 手写回溯递归
来源：http://dfu.9152youxi.cn

[N09] 栈与队列
来源：http://svj.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gug.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mep.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nsj.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kst.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vte.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yft.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vjo.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://arp.chenlongwang.top

[N10] 链表节点定义
来源：http://wor.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pji.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://qth.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hyg.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tfs.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://bee.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iqt.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jut.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://unu.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://uwp.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qjt.9152youxi.cn

PHP:  // 手写递归函数
来源：http://mnl.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sbw.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hpj.chenlongwang.top

Java: // 手写递归
来源：http://xla.yj202588.top

Go:   // 手写递归
来源：http://rhl.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oae.gzhubu.top

C#:   // 手写递归
来源：http://vnv.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vfx.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zzz.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zck.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qxl.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xya.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://deo.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://quw.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ynk.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jwc.jinqigfzy.top

================================================================================
来源：http://jni.xuetiantiany.cn

O. 并发与异步
来源：http://kql.jinqigfzy.top

================================================================================
来源：http://jyu.hfpthk.cn

[O01] 启动一个线程
来源：http://fdh.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ucm.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bmv.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zjj.hysaishi.cn

TS:   // 同 JS
来源：http://pfj.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://hai.hnqzz.top

Go:   go f()
来源：http://rqx.ydzc1.top

Ruby: Thread.new { f }
来源：http://vmi.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://bst.zhiwuduotai.top

[O02] 使用线程池
来源：http://tnb.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nrd.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zal.yonumen.top

JS:   // worker_threads 线程池
来源：http://mhz.316326.xyz

TS:   // worker_threads 线程池
来源：http://pqt.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://elq.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iek.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pae.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jrq.52xcode.cn

[O03] 加锁保护共享数据
来源：http://cjt.haohaochexian.top

Py:   with lock: shared += 1
来源：http://jbl.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://zfx.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wry.shangyingyoupin.top

TS:   // 同 JS
来源：http://vrs.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://jqv.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ykt.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://teb.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://swm.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://bgx.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://qns.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ksr.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://qgv.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kfh.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mmp.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uwy.hongshengwenyu.top

Ruby: # 用 Fiber 或 async gem
来源：http://tqc.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://btj.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://gkx.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://dej.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wyk.tanke756.top

JS:   await Promise.all(tasks)
来源：http://ehv.ivvv.top

TS:   await Promise.all(tasks)
来源：http://lxy.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gfu.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://byy.xziqi.cn

Ruby: threads.map(&:join)
来源：http://zeq.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pkp.zhengqikj.top

[O06] 使用进程池
来源：http://lqe.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ekk.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://gxd.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://mkm.jinyuanbaomall.cn


<!-- 参考信息 -->