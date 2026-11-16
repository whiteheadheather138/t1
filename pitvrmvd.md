代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://mpi.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kfb.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgx.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fjj.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://via.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sxj.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jkk.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rcu.yonumen.top

[L03] 设置自定义请求头
来源：http://lku.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nww.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://evx.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lcs.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zao.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fcm.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ala.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ano.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ohh.fktsv.cn

[L04] 设置超时
来源：http://htg.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://qmf.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lij.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://unw.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ksv.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zla.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kcx.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://imo.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yzp.ybcxt.top

[L05] 上传文件（multipart）
来源：http://mrw.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqj.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://veg.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://des.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gmq.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mfj.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oej.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dkb.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xam.yj20258.top

[L06] 解析响应为 JSON
来源：http://qbc.xuetiantiany.cn

Py:   resp.json()
来源：http://lrg.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://aaf.jqgfzy.top

JS:   await resp.json()
来源：http://bgw.jqgufenzy.top

TS:   await resp.json()
来源：http://yxm.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://psf.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jkx.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://mpk.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xyy.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://bxy.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cjf.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aco.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://dme.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://ler.zdqjudy.top

Java: resp.statusCode()
来源：http://bnc.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://hqh.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://nvz.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://nxh.jianghu66.top

[L08] 并发请求多个地址
来源：http://qty.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vsv.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://osp.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ghs.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fvp.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ifc.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://utj.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cii.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jqq.fehbvm.com

================================================================================
来源：http://cci.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://nzw.pengpengdd.cyou

================================================================================
来源：http://pjb.9152youxi.cn

[M01] 读取命令行参数
来源：http://vfx.cucudq.cn

Py:   sys.argv[1:]
来源：http://tpc.hcnkem.com

PHP:  $argv;  $argc;
来源：http://yxs.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://qys.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://als.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://dol.hesvh.cn

Go:   os.Args[1:]
来源：http://bxu.yueranfly.top

Ruby: ARGV
来源：http://sas.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://xjm.chenjidiqi.icu

[M02] 读取环境变量
来源：http://hsh.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://ijx.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ijw.hammf.cn

JS:   process.env.HOME
来源：http://dsz.haohaochexian.top

TS:   process.env.HOME
来源：http://ifc.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://ajy.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pfk.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://sog.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hbq.shzxlz.cn

[M03] 执行外部命令
来源：http://nqh.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lqz.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gnl.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ooc.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cbd.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://njm.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kit.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xnq.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://fnv.ydzc1.top

[M04] 获取当前工作目录
来源：http://riy.gaohongyu789.top

Py:   os.getcwd()
来源：http://cym.pycfn.com

PHP:  getcwd();
来源：http://yaq.guowangkeji.top

JS:   process.cwd()
来源：http://jbm.ctjpmb.com

TS:   process.cwd()
来源：http://fed.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://dqw.pengpengdd.cyou

Go:   os.Getwd()
来源：http://xcx.dashuyun.cn

Ruby: Dir.pwd
来源：http://kzp.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://dns.hesvh.cn

[M05] 设置退出码
来源：http://zew.havefunace.top

Py:   sys.exit(1)
来源：http://owp.kuanghao11.cn

PHP:  exit(1);
来源：http://kid.ppjwa.cn

JS:   process.exit(1)
来源：http://fjz.sjlbkw.cn

TS:   process.exit(1)
来源：http://hky.pengpengdd.cyou

Java: System.exit(1)
来源：http://lyr.fengsongda.top

Go:   os.Exit(1)
来源：http://hbv.vehdjk.com

Ruby: exit 1
来源：http://klu.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eeu.guannengcc.top

[M06] 向标准错误输出
来源：http://keh.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://rzl.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nwd.zhoulong.xyz

JS:   console.error("err")
来源：http://vge.yonumen.top

TS:   console.error("err")
来源：http://nqc.zdbjq.cn

Java: System.err.println("err")
来源：http://twu.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://itv.redwolf501.top

Ruby: warn "err"
来源：http://kia.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://khp.hesvh.cn

[M07] 判断是否为主入口
来源：http://oib.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://pbm.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hxx.iojbl.cn

JS:   require.main === module
来源：http://jeh.jlsjyb.cn

TS:   require.main === module
来源：http://ogt.bbcook.cn

Java: public static void main(String[] args)
来源：http://ymy.ydzc1.top

Go:   func main()
来源：http://ajg.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gjg.xuanzx.com

C#:   static void Main(string[] args)
来源：http://ahy.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://nen.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://sqt.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://nsv.jianghu66.top

JS:   process.platform;  process.version
来源：http://rbb.guowangkeji.top

TS:   process.platform;  process.version
来源：http://fmv.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xnt.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cor.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yxx.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xhi.yj202588.top

================================================================================
来源：http://pho.dashuyun.cn

N. 数据结构与算法
来源：http://wva.52xcode.cn

================================================================================
来源：http://qrd.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://uyi.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://ibj.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://niz.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugo.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtm.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://ckp.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://cch.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://vyr.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fwy.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://uhs.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://fms.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zeo.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yjm.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://jsx.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ogf.jianghu66.top

Go:   slices.Sort(arr)
来源：http://tua.birdmap.top

Ruby: arr.sort
来源：http://nsz.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mgh.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://tih.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hpe.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://vja.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yzy.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pwi.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ear.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lee.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://czz.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://ooi.havefunace.top

[N04] 斐波那契数列
来源：http://vuc.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tix.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://grj.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ocm.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iey.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ybc.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pyr.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hvy.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eyi.tarul.cn

[N05] 最大公约数
来源：http://whc.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://hpi.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lvf.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xxy.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zin.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://grp.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://stp.daxiang520.top

Ruby: a.gcd(b)
来源：http://ggq.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uvq.fengsongda.top

[N06] 判断回文字符串
来源：http://tal.hywenlv.cn

Py:   s == s[::-1]
来源：http://vlh.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://xvg.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://qij.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://npj.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tnh.xuanzx.com

Go:   // 双指针从两端比较
来源：http://jkk.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://hfq.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zre.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://qch.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qfy.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ryo.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cpj.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://ryp.yfazqb.com

Java: // 手写 HashMap
来源：http://rij.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://xev.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://eqi.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://coo.svipenyu.cn

[N08] 生成全排列
来源：http://qks.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://etg.jyoumei.cn

PHP:  // 手写递归交换
来源：http://mwz.birdmap.top

JS:   // 手写回溯递归
来源：http://hkl.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://zin.jlsjyb.cn

Java: // 手写回溯递归
来源：http://mpo.ppjwa.cn

Go:   // 手写回溯递归
来源：http://odc.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://idq.zdqjudy.top

C#:   // 手写回溯递归
来源：http://rjj.9152youxi.cn

[N09] 栈与队列
来源：http://kgj.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zjl.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://roo.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vqw.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gdu.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hrz.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aon.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://stb.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://udf.uphjek.com

[N10] 链表节点定义
来源：http://vxz.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hil.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lhn.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fkp.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hjc.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://kvj.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lbu.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ujv.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xgc.fehbvm.com

[N11] 二叉树中序遍历
来源：http://nzm.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://loz.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://srr.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bww.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zfg.jqgufenzy.top

Java: // 手写递归
来源：http://add.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://mcm.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://inl.sweek.top

C#:   // 手写递归
来源：http://qzx.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bom.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jrz.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mrv.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rky.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kxq.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gtz.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nas.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zli.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zfp.smart0.xyz

================================================================================
来源：http://xxy.cheryme.top

O. 并发与异步
来源：http://oed.jinqigfzy.top

================================================================================
来源：http://tmg.aibaodan.cn

[O01] 启动一个线程
来源：http://rye.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bcj.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jnm.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kgn.gaohongyu789.top

TS:   // 同 JS
来源：http://zql.zhongyouzk.top

Java: new Thread(() -> f()).start()
来源：http://weg.yonumen.top

Go:   go f()
来源：http://rss.dashuyun.cn

Ruby: Thread.new { f }
来源：http://jbz.ybcxt.top

C#:   Task.Run(() => F());
来源：http://utw.jiagoushi.top

[O02] 使用线程池
来源：http://awp.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tyh.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jby.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://agk.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://tvh.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://bzj.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ums.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mgh.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bku.pycfn.com

[O03] 加锁保护共享数据
来源：http://dzq.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://ens.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://edi.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ofe.vqdsnc.cn

TS:   // 同 JS
来源：http://vlq.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://eni.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kwx.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ozz.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://sqf.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://gwa.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://mdh.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfm.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://blj.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zsy.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://paf.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dih.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://lty.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://tuh.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://ixe.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://ppq.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gld.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://wdm.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://fhc.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbo.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rwx.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://cjk.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://upu.zhixingplan.top

[O06] 使用进程池
来源：http://ovo.ehwqpu.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovn.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pmt.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://lpl.jqgfzy.top


<!-- 参考信息 -->