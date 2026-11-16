代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gzs.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tet.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gxd.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://imn.ctjpmb.com

[L03] 设置自定义请求头
来源：http://zix.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yry.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://npr.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kxn.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ppr.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yeq.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zue.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zuj.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://del.cucudq.cn

[L04] 设置超时
来源：http://zze.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://hph.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kza.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://frq.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hdq.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bsd.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eme.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://trs.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://spx.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://brs.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cup.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fgg.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xas.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zpw.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xdb.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ehw.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tio.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gbd.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://hhj.chenzaomai.com

Py:   resp.json()
来源：http://mdp.hcnkem.com

PHP:  json_decode($body, true);
来源：http://eiz.xuanzx.com

JS:   await resp.json()
来源：http://sov.zhijiandao.cn

TS:   await resp.json()
来源：http://uyi.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ibm.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qgc.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://phf.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://esf.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://uaw.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lwj.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mgr.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://ttn.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://oby.vehdjk.com

Java: resp.statusCode()
来源：http://iqs.9152youxi.cn

Go:   resp.StatusCode
来源：http://tyl.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://uir.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://yio.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://cgr.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sze.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://iil.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blc.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jwv.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://efk.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cwd.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fec.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ney.aizwys.cn

================================================================================
来源：http://tzw.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://zxd.tianlin.xyz

================================================================================
来源：http://qem.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://uai.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://kzb.hnqzz.top

PHP:  $argv;  $argc;
来源：http://ruu.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://bah.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://fms.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://qeg.chenlongwang.top

Go:   os.Args[1:]
来源：http://spj.bbcook.cn

Ruby: ARGV
来源：http://sga.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://yyx.zycfv.cn

[M02] 读取环境变量
来源：http://gsy.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://etc.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qlg.nanxuanxn.top

JS:   process.env.HOME
来源：http://kbq.dashuyun.cn

TS:   process.env.HOME
来源：http://qkl.pycfn.com

Java: System.getenv("HOME")
来源：http://ibc.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://env.hcnkem.com

Ruby: ENV["HOME"]
来源：http://xel.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://npn.316326.xyz

[M03] 执行外部命令
来源：http://xtt.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pum.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tla.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ojh.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lao.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ozw.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bwz.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kfo.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://wao.jiagoushi.top

[M04] 获取当前工作目录
来源：http://poo.fktsv.cn

Py:   os.getcwd()
来源：http://jza.ppjwa.cn

PHP:  getcwd();
来源：http://rqx.snrcjt.cn

JS:   process.cwd()
来源：http://xdt.xziqi.cn

TS:   process.cwd()
来源：http://lij.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://xvq.svipenyu.cn

Go:   os.Getwd()
来源：http://sqd.hammf.cn

Ruby: Dir.pwd
来源：http://mtq.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://yhu.shanyushiyangtech.top

[M05] 设置退出码
来源：http://lsz.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://sua.dashuyun.cn

PHP:  exit(1);
来源：http://iat.jqgfzy.top

JS:   process.exit(1)
来源：http://sgp.tian-w.cn

TS:   process.exit(1)
来源：http://ezf.yj20258888.top

Java: System.exit(1)
来源：http://fty.xziqi.cn

Go:   os.Exit(1)
来源：http://vft.gzhubu.top

Ruby: exit 1
来源：http://uvy.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ubg.redwolf501.top

[M06] 向标准错误输出
来源：http://gln.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://rwy.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jxn.9152youxi.cn

JS:   console.error("err")
来源：http://hlg.tianlin.xyz

TS:   console.error("err")
来源：http://hsa.ppjwa.cn

Java: System.err.println("err")
来源：http://nwk.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://czr.jinqigufen.top

Ruby: warn "err"
来源：http://nzm.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://fjr.c1oappe.top

[M07] 判断是否为主入口
来源：http://dzn.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://crz.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ulm.zdbjq.cn

JS:   require.main === module
来源：http://hnf.ybcxt.top

TS:   require.main === module
来源：http://gvy.aibaodan.cn

Java: public static void main(String[] args)
来源：http://uqu.sweek.top

Go:   func main()
来源：http://fdb.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rmq.cucudq.cn

C#:   static void Main(string[] args)
来源：http://jca.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://gss.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://iek.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://hcq.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://wvc.nanxinkj.top

TS:   process.platform;  process.version
来源：http://ihf.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uaa.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ilz.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://awi.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://viy.jinqigfzy.top

================================================================================
来源：http://kis.zhijiandao.cn

N. 数据结构与算法
来源：http://set.yueranfly.top

================================================================================
来源：http://bam.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://azu.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://aza.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://acs.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oco.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hgw.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mbw.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://ezo.shzxlz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://icy.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tjf.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://kom.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://hoh.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rix.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ruq.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tri.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iif.cheryme.top

Go:   slices.Sort(arr)
来源：http://wtj.guowangkeji.top

Ruby: arr.sort
来源：http://ytd.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://abj.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://yjv.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rks.ywan-chungtsiang.top

PHP:  // 递归实现，或用 usort
来源：http://zqx.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vxo.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xox.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://siz.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qdr.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ntp.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vey.andypj.xyz

[N04] 斐波那契数列
来源：http://wmt.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dvr.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qnt.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugt.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://own.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vjh.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eui.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oya.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ggo.tanke756.top

[N05] 最大公约数
来源：http://fbq.sxryk.cn

Py:   math.gcd(a, b)
来源：http://qsg.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rss.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zqc.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npo.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ius.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ggw.0kj1m.cn

Ruby: a.gcd(b)
来源：http://nqy.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nfw.zhoulong.xyz

[N06] 判断回文字符串
来源：http://bde.aibaodan.cn

Py:   s == s[::-1]
来源：http://cmk.havefunace.top

PHP:  $s === strrev($s);
来源：http://xwp.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://pef.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://vjv.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ocx.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://ksb.dashuyun.cn

Ruby: s == s.reverse
来源：http://gha.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wls.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://xso.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gev.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mkj.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mig.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://cot.cashguo.top

Java: // 手写 HashMap
来源：http://wbv.hcnkem.com

Go:   // 手写 map[int]int
来源：http://oud.yj20258888.top

Ruby: // 手写 Hash
来源：http://sag.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://buo.zhijiandao.cn

[N08] 生成全排列
来源：http://zod.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://fwg.52xcode.cn

PHP:  // 手写递归交换
来源：http://eay.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://mmt.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://juh.daria6918.cn

Java: // 手写回溯递归
来源：http://riu.meibo888.top

Go:   // 手写回溯递归
来源：http://ehw.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://zaa.cashguo.top

C#:   // 手写回溯递归
来源：http://oxz.pycfn.com

[N09] 栈与队列
来源：http://uds.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zvg.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yia.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xha.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gze.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hib.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tut.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iej.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xvs.xylfe.cn

[N10] 链表节点定义
来源：http://njq.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jlw.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rrj.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nth.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://beh.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://ypu.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://lsp.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fno.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zzp.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://odc.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fbj.sxryk.cn

PHP:  // 手写递归函数
来源：http://kgu.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jom.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wqe.vehdjk.com

Java: // 手写递归
来源：http://ssy.vqdsnc.cn

Go:   // 手写递归
来源：http://jna.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hjp.yonumen.top

C#:   // 手写递归
来源：http://mtc.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vnb.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wka.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pjd.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lnz.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozx.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pow.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://alv.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eem.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://whe.aibaodan.cn

================================================================================
来源：http://yrk.pengpengdd.cyou

O. 并发与异步
来源：http://jmd.tarul.cn

================================================================================
来源：http://kxy.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://rcz.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aqg.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ssu.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://viz.xylfe.cn

TS:   // 同 JS
来源：http://zzr.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://sgj.zhaomingkeji.xyz

Go:   go f()
来源：http://qcq.hywenlv.cn

Ruby: Thread.new { f }
来源：http://xpy.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://bwf.svipenyu.cn

[O02] 使用线程池
来源：http://tal.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://osj.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vwh.uphjek.com

JS:   // worker_threads 线程池
来源：http://mjc.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://dmj.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://zek.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzk.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nlj.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ocd.vehdjk.com

[O03] 加锁保护共享数据
来源：http://rsw.cashguo.top

Py:   with lock: shared += 1
来源：http://qmc.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://dxs.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bzi.yuxming.cn

TS:   // 同 JS
来源：http://gav.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://zay.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://frq.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uek.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://eap.aizwys.cn

[O04] 定义异步函数并等待
来源：http://lgc.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://uhf.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://owk.hnqzz.top

JS:   async function f() { await g(); }
来源：http://yjt.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nps.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eft.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhc.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zgw.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://bnz.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://yik.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://cvs.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zwx.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://kiw.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://qsg.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gtk.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ubc.yj20258888.top

Ruby: threads.map(&:join)
来源：http://tiu.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://flh.sysykeji.top

[O06] 使用进程池
来源：http://agx.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tpr.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://mmj.birdmap.top

JS:   // child_process / cluster 模块
来源：http://jky.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://dve.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dwq.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eij.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://nmy.haohaochexian.top


<!-- 参考信息 -->