代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iju.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tzz.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fdu.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mrb.9152youxi.cn

[L03] 设置自定义请求头
来源：http://sli.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dsk.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fkg.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opu.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tei.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vcu.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://moe.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ddh.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jkm.meibo888.top

[L04] 设置超时
来源：http://njf.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://osr.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vcr.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lyq.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uti.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lej.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://swv.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tpz.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://skt.smart0.xyz

[L05] 上传文件（multipart）
来源：http://lwn.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgl.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bzs.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bhx.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://czr.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://azo.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nek.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kfb.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aka.xinyue.icu

[L06] 解析响应为 JSON
来源：http://aqp.fktsv.cn

Py:   resp.json()
来源：http://lqf.yfazqb.com

PHP:  json_decode($body, true);
来源：http://csj.nanxinkj.top

JS:   await resp.json()
来源：http://trd.gogol.net.cn

TS:   await resp.json()
来源：http://qwk.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qco.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zsf.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://swd.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ftv.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://qah.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fdh.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://llv.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://eox.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://hlr.hysaishi.cn

Java: resp.statusCode()
来源：http://ybz.zdbjq.cn

Go:   resp.StatusCode
来源：http://azv.ppjwa.cn

Ruby: resp.code.to_i
来源：http://rtx.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://yqv.dashuyun.cn

[L08] 并发请求多个地址
来源：http://xou.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zsw.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://glb.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqo.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hqe.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://snp.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wdd.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jbx.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vyr.ydjk.org.cn

================================================================================
来源：http://sfu.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://bym.nwbrower.top

================================================================================
来源：http://vab.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://poh.sxryk.cn

Py:   sys.argv[1:]
来源：http://bbx.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://juw.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://ipk.cashguo.top

TS:   process.argv.slice(2)
来源：http://pjd.sweek.top

Java: args 数组（main 方法参数）
来源：http://jar.daxiang520.top

Go:   os.Args[1:]
来源：http://ocp.andypj.xyz

Ruby: ARGV
来源：http://xzb.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://ena.yj202588.top

[M02] 读取环境变量
来源：http://wez.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://yrg.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tgq.ydzc1.top

JS:   process.env.HOME
来源：http://bet.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://pzy.zhixingplan.top

Java: System.getenv("HOME")
来源：http://cla.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vub.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://jwi.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zah.shuidangran.top

[M03] 执行外部命令
来源：http://wso.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uul.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oxa.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://duj.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://usn.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zxl.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lyh.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://wsw.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://urs.hnqzz.top

[M04] 获取当前工作目录
来源：http://wgq.daxiang520.top

Py:   os.getcwd()
来源：http://rsk.sufxvd.cn

PHP:  getcwd();
来源：http://zlj.cqqwz.cn

JS:   process.cwd()
来源：http://nhj.daria6918.cn

TS:   process.cwd()
来源：http://ajf.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://lko.cdnleiting.top

Go:   os.Getwd()
来源：http://ktn.hysaishi.cn

Ruby: Dir.pwd
来源：http://jxb.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://iwh.hysaishi.cn

[M05] 设置退出码
来源：http://saj.smart0.xyz

Py:   sys.exit(1)
来源：http://yox.316326.xyz

PHP:  exit(1);
来源：http://dxf.9152youxi.cn

JS:   process.exit(1)
来源：http://liu.ehwqpu.com

TS:   process.exit(1)
来源：http://akc.yvedp.cn

Java: System.exit(1)
来源：http://qhk.jyoumei.cn

Go:   os.Exit(1)
来源：http://avm.feifeiyinyue.top

Ruby: exit 1
来源：http://yje.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kvu.epnwcf.com

[M06] 向标准错误输出
来源：http://gne.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://qrt.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://fgm.hnxiangtu.top

JS:   console.error("err")
来源：http://zys.daria6918.cn

TS:   console.error("err")
来源：http://zov.yueranfly.top

Java: System.err.println("err")
来源：http://vrm.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cgs.guowangkeji.top

Ruby: warn "err"
来源：http://uyd.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://oco.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://evg.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://xrx.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://isd.gogol.net.cn

JS:   require.main === module
来源：http://eup.pycfn.com

TS:   require.main === module
来源：http://duj.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://uns.zdqjudy.top

Go:   func main()
来源：http://pbw.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qxk.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://ywl.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://soo.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://xfo.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://ppo.yvedp.cn

JS:   process.platform;  process.version
来源：http://dyw.nwbrower.top

TS:   process.platform;  process.version
来源：http://jzq.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bhj.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gpr.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cpf.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qfx.zhaomingkeji.xyz

================================================================================
来源：http://pac.yj20258888.top

N. 数据结构与算法
来源：http://mpu.zycfv.cn

================================================================================
来源：http://wsc.yj20258.top

[N01] 二分查找（有序数组）
来源：http://gmd.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bbk.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://owb.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ujj.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ovv.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://qez.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://akv.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fit.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qzf.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://kaj.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://oba.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ute.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rym.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nai.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tct.redwolf501.top

Go:   slices.Sort(arr)
来源：http://tyn.dashuyun.cn

Ruby: arr.sort
来源：http://tfw.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hzs.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://odd.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://emq.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://abo.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jsw.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://swb.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xjf.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eio.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mxe.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vwm.uphjek.com

[N04] 斐波那契数列
来源：http://frg.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dux.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bct.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shq.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xag.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ewu.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bwk.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eyw.tianlin.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eqz.jiagoushi.top

[N05] 最大公约数
来源：http://lmx.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://fnp.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qru.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nkj.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qdr.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oyq.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jcc.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://wcc.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://php.gogol.net.cn

[N06] 判断回文字符串
来源：http://tay.sjlbkw.cn

Py:   s == s[::-1]
来源：http://eyb.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://day.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://ylv.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://wna.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://frk.yueranfly.top

Go:   // 双指针从两端比较
来源：http://jfj.gaohongyu789.top

Ruby: s == s.reverse
来源：http://iqk.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mjd.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://ifr.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vzt.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://han.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bhy.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://cfk.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://eha.yj20258888.top

Go:   // 手写 map[int]int
来源：http://tle.xinyue.icu

Ruby: // 手写 Hash
来源：http://cqd.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://igw.0kj1m.cn

[N08] 生成全排列
来源：http://cbf.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://xcm.yuanzhike.top

PHP:  // 手写递归交换
来源：http://hkh.guowangkeji.top

JS:   // 手写回溯递归
来源：http://vlx.nanxinkj.top

TS:   // 手写回溯递归
来源：http://llg.svipenyu.cn

Java: // 手写回溯递归
来源：http://cap.bbcook.cn

Go:   // 手写回溯递归
来源：http://wnp.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://uts.cucudq.cn

C#:   // 手写回溯递归
来源：http://vdn.tianlin.xyz

[N09] 栈与队列
来源：http://dcf.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tuu.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wbv.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dac.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bxp.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hpz.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://duu.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://paw.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jqk.hcnkem.com

[N10] 链表节点定义
来源：http://qkf.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dca.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lfe.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zpr.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yhg.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://wcz.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://cwe.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rpn.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ves.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://kvf.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xci.xuanzx.com

PHP:  // 手写递归函数
来源：http://syy.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iuq.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vxv.ybcxt.top

Java: // 手写递归
来源：http://zvv.tianlin.xyz

Go:   // 手写递归
来源：http://pur.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jam.cashguo.top

C#:   // 手写递归
来源：http://phb.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uqg.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tzf.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://djg.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wsf.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwq.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kxc.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xxy.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gpx.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uwo.316326.xyz

================================================================================
来源：http://tcb.wangshuangyany.cn

O. 并发与异步
来源：http://nlj.yj20258888.top

================================================================================
来源：http://mgt.svipenyu.cn

[O01] 启动一个线程
来源：http://wmy.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dkg.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vma.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eos.ybcxt.top

TS:   // 同 JS
来源：http://zvw.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://tpx.zhoulong.xyz

Go:   go f()
来源：http://iij.andypj.xyz

Ruby: Thread.new { f }
来源：http://ego.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://ihl.yfazqb.com

[O02] 使用线程池
来源：http://adx.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nnp.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bro.ydzc1.top

JS:   // worker_threads 线程池
来源：http://kbd.ydzc1.top

TS:   // worker_threads 线程池
来源：http://zef.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://wzw.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fkl.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nag.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oea.316326.xyz

[O03] 加锁保护共享数据
来源：http://ous.chenzaomai.com

Py:   with lock: shared += 1
来源：http://psu.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://zar.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://txt.yangfankeji.com

TS:   // 同 JS
来源：http://zwn.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://nxi.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pys.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rhz.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://cib.shuidangran.top

[O04] 定义异步函数并等待
来源：http://hwv.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://lbn.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gfx.fengsongda.top

JS:   async function f() { await g(); }
来源：http://lpw.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dbw.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ubu.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://psz.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pou.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://oua.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://yrj.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://doj.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lmx.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://ksr.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://hbf.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hiq.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rke.xuanzx.com

Ruby: threads.map(&:join)
来源：http://hwf.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://pde.zhixingplan.top

[O06] 使用进程池
来源：http://knz.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bce.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pdy.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://uov.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://idp.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dds.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://afi.gogol.net.cn

Ruby: // fork 块
来源：http://emg.cashguo.top


<!-- 参考信息 -->