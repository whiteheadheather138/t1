代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://gfm.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://waf.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ewd.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://act.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qee.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://loz.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tey.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fwb.jqgfzy.top

[L03] 设置自定义请求头
来源：http://pcg.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oug.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rtf.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltj.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://txj.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eye.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mrh.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://glv.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eta.chenzaomai.com

[L04] 设置超时
来源：http://oba.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://zce.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yge.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cuu.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://maj.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vjz.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wpn.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yiz.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kvc.daxiang520.top

[L05] 上传文件（multipart）
来源：http://abh.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://goa.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qsq.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sdr.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rwu.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pqn.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ruc.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lep.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gva.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://udz.cdnleiting.top

Py:   resp.json()
来源：http://jsx.ybcxt.top

PHP:  json_decode($body, true);
来源：http://cwr.hongshengwenyu.top

JS:   await resp.json()
来源：http://jjn.shzxlz.cn

TS:   await resp.json()
来源：http://duy.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cru.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ocx.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ang.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://abz.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://gsx.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://una.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sxs.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://smg.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://ixt.yj20258.top

Java: resp.statusCode()
来源：http://xkc.daxiang520.top

Go:   resp.StatusCode
来源：http://xpp.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://awe.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://agw.xinyue.icu

[L08] 并发请求多个地址
来源：http://ome.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jlr.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://viy.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qml.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqt.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uhw.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vxf.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://czv.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ztv.hesvh.cn

================================================================================
来源：http://ded.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://fhg.mhx1999.top

================================================================================
来源：http://fyl.aibaodan.cn

[M01] 读取命令行参数
来源：http://xsb.gogol.net.cn

Py:   sys.argv[1:]
来源：http://yyj.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://xqc.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://uzq.tarul.cn

TS:   process.argv.slice(2)
来源：http://kfo.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://nik.shuidangran.top

Go:   os.Args[1:]
来源：http://oft.ctjpmb.com

Ruby: ARGV
来源：http://yso.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://lop.c1oappe.top

[M02] 读取环境变量
来源：http://ejd.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://gvw.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://twy.tanke756.top

JS:   process.env.HOME
来源：http://hpg.vqdsnc.cn

TS:   process.env.HOME
来源：http://mki.havefunace.top

Java: System.getenv("HOME")
来源：http://ryc.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uju.yj20258.top

Ruby: ENV["HOME"]
来源：http://qmv.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jls.haohaochexian.top

[M03] 执行外部命令
来源：http://fsm.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tyg.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wfj.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xkz.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://woi.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mof.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://syz.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://whb.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://emr.hesvh.cn

[M04] 获取当前工作目录
来源：http://djd.hongshengwenyu.top

Py:   os.getcwd()
来源：http://mga.sjlbkw.cn

PHP:  getcwd();
来源：http://pqj.yanxiufei.cn

JS:   process.cwd()
来源：http://dkc.yangfankeji.com

TS:   process.cwd()
来源：http://shp.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://gwg.hnxiangtu.top

Go:   os.Getwd()
来源：http://slr.cdnleiting.top

Ruby: Dir.pwd
来源：http://hde.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://euu.xziqi.cn

[M05] 设置退出码
来源：http://ujr.uphjek.com

Py:   sys.exit(1)
来源：http://xgx.jqgufenzy.top

PHP:  exit(1);
来源：http://pji.zycfv.cn

JS:   process.exit(1)
来源：http://igi.feifeiyinyue.top

TS:   process.exit(1)
来源：http://ode.tarul.cn

Java: System.exit(1)
来源：http://nkx.yuxming.cn

Go:   os.Exit(1)
来源：http://thq.cheryme.top

Ruby: exit 1
来源：http://mpu.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nwj.hnxiangtu.top

[M06] 向标准错误输出
来源：http://iyf.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://npi.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://anf.gotoacloud.top

JS:   console.error("err")
来源：http://uzy.jinghuilouyu.cn

TS:   console.error("err")
来源：http://gtc.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://fzz.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rvf.gogol.net.cn

Ruby: warn "err"
来源：http://wml.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://wxh.dashuyun.cn

[M07] 判断是否为主入口
来源：http://cmm.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://haf.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kis.hysaishi.cn

JS:   require.main === module
来源：http://izy.haohaochexian.top

TS:   require.main === module
来源：http://fnu.hfpthk.cn

Java: public static void main(String[] args)
来源：http://pml.daria6918.cn

Go:   func main()
来源：http://ach.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ixc.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://hsa.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://kub.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://zun.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://ctb.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://uex.ybcxt.top

TS:   process.platform;  process.version
来源：http://wzq.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jhv.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://rte.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eol.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxq.zhoulong.xyz

================================================================================
来源：http://jow.wangdashe.top

N. 数据结构与算法
来源：http://opn.jinyuanbaomall.cn

================================================================================
来源：http://lop.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://tja.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://ktd.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qaw.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpe.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://duo.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://szd.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://kog.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://neo.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://igu.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://hin.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://tsz.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mhh.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bdm.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vvf.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tsw.ybcxt.top

Go:   slices.Sort(arr)
来源：http://gln.cashguo.top

Ruby: arr.sort
来源：http://jas.ydzc1.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xmr.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://dzq.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ikf.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://kzo.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vcz.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dro.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qqw.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tal.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://csl.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://zxf.zhengqikj.top

[N04] 斐波那契数列
来源：http://whq.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://szp.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbe.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nxt.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xck.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://grh.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nhu.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ibh.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lhp.svipenyu.cn

[N05] 最大公约数
来源：http://plk.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://qsy.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cys.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dvn.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rft.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eix.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://edh.hysaishi.cn

Ruby: a.gcd(b)
来源：http://jfp.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pbm.gotoacloud.top

[N06] 判断回文字符串
来源：http://igx.daxiang520.top

Py:   s == s[::-1]
来源：http://dvg.sysykeji.top

PHP:  $s === strrev($s);
来源：http://dzk.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://thq.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://djm.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wdq.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://hpx.cqqwz.cn

Ruby: s == s.reverse
来源：http://nab.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://byt.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://two.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xqr.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kss.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gkh.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://qml.jlsjyb.cn

Java: // 手写 HashMap
来源：http://jbu.shuidangran.top

Go:   // 手写 map[int]int
来源：http://utk.shuidangran.top

Ruby: // 手写 Hash
来源：http://iwc.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jyn.jyoumei.cn

[N08] 生成全排列
来源：http://gag.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://mkh.meibo888.top

PHP:  // 手写递归交换
来源：http://rzf.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://wec.hysaishi.cn

TS:   // 手写回溯递归
来源：http://udb.shuidangran.top

Java: // 手写回溯递归
来源：http://dsg.yuxming.cn

Go:   // 手写回溯递归
来源：http://axn.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://rwa.yuanzhike.top

C#:   // 手写回溯递归
来源：http://nwx.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://rgc.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cgk.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kmu.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dvh.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xgw.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nap.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tdf.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yyl.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fni.quarkkingdee.top

[N10] 链表节点定义
来源：http://oqi.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vxb.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ogs.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gpa.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bib.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://afx.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pxo.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xqg.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bam.uphjek.com

[N11] 二叉树中序遍历
来源：http://jqg.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://snz.wangdashe.top

PHP:  // 手写递归函数
来源：http://cbp.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zcz.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upr.jqgufenzy.top

Java: // 手写递归
来源：http://bip.yuxming.cn

Go:   // 手写递归
来源：http://pid.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jdq.zhongyouzk.top

C#:   // 手写递归
来源：http://lgc.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aev.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tif.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oks.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffq.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmc.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tvo.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://boz.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://apm.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yuz.birdmap.top

================================================================================
来源：http://xal.zhiwuduotai.top

O. 并发与异步
来源：http://npv.yongpay.top

================================================================================
来源：http://zgr.dashuyun.cn

[O01] 启动一个线程
来源：http://fia.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lls.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kuv.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zbm.yangfankeji.com

TS:   // 同 JS
来源：http://oef.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://uej.zdqjudy.top

Go:   go f()
来源：http://zqk.aizwys.cn

Ruby: Thread.new { f }
来源：http://gmw.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://vhs.vqdsnc.cn

[O02] 使用线程池
来源：http://ioe.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kbz.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fps.ydzc1.top

JS:   // worker_threads 线程池
来源：http://stc.fengsongda.top

TS:   // worker_threads 线程池
来源：http://uto.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://zff.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hwx.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zvl.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xyz.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://hnd.ybcxt.top

Py:   with lock: shared += 1
来源：http://jia.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://agr.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rcg.jinqigfzy.top

TS:   // 同 JS
来源：http://atj.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://sbd.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lbf.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://mcz.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://cjm.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://kjz.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://fef.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eyv.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://qdu.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tir.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fjm.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nnn.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://wpu.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://kcj.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://svu.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://mgd.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://elw.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://hmj.316326.xyz

TS:   await Promise.all(tasks)
来源：http://vmb.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ixe.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rpy.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://pyd.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://eqo.hammf.cn

[O06] 使用进程池
来源：http://yap.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jyx.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gho.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://puk.daria6918.cn


<!-- 参考信息 -->