代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sok.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gxs.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wmy.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jwa.iojbl.cn

[L03] 设置自定义请求头
来源：http://bqy.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kpw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bnh.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cav.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kfb.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vjc.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nlj.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://elz.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zfr.zhijiandao.cn

[L04] 设置超时
来源：http://jiy.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://inc.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ikq.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rvg.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgi.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ffg.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://myh.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xfp.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zur.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://gws.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uzf.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dnt.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qxb.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gfn.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mnm.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqn.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lep.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lhq.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://riq.hesvh.cn

Py:   resp.json()
来源：http://gip.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://jvp.aizwys.cn

JS:   await resp.json()
来源：http://klz.yuanzhike.top

TS:   await resp.json()
来源：http://fcc.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lfq.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://avd.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://qzu.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ciw.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://bbv.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dnb.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ggo.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://bbi.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://slr.hywenlv.cn

Java: resp.statusCode()
来源：http://nbf.yueranfly.top

Go:   resp.StatusCode
来源：http://tnf.bjfxy.top

Ruby: resp.code.to_i
来源：http://nfn.cheryme.top

C#:   (int)resp.StatusCode
来源：http://ffy.hnqzz.top

[L08] 并发请求多个地址
来源：http://ein.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dwp.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://kpk.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qsr.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zri.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bbw.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lms.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nhr.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://htj.hcnkem.com

================================================================================
来源：http://xnf.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://lnw.pycfn.com

================================================================================
来源：http://usd.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://vqt.guowangkeji.top

Py:   sys.argv[1:]
来源：http://swg.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://ain.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://lsg.tian-w.cn

TS:   process.argv.slice(2)
来源：http://nmi.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://uwl.9152youxi.cn

Go:   os.Args[1:]
来源：http://bhu.svipenyu.cn

Ruby: ARGV
来源：http://ijw.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://xwo.gaohongyu789.top

[M02] 读取环境变量
来源：http://nqv.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://gou.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ewm.yangfankeji.com

JS:   process.env.HOME
来源：http://hdt.cucudq.cn

TS:   process.env.HOME
来源：http://qef.hesvh.cn

Java: System.getenv("HOME")
来源：http://ygl.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iob.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://opl.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fxl.zhengqikj.top

[M03] 执行外部命令
来源：http://vui.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hfz.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yrx.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://fgw.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zlw.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mlu.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uht.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://uqc.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://ucg.aibaodan.cn

[M04] 获取当前工作目录
来源：http://akj.redwolf501.top

Py:   os.getcwd()
来源：http://atx.tarul.cn

PHP:  getcwd();
来源：http://ytk.jinqigfzy.top

JS:   process.cwd()
来源：http://leb.yonumen.top

TS:   process.cwd()
来源：http://vnq.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://clr.wangshuangyany.cn

Go:   os.Getwd()
来源：http://gcr.daria6918.cn

Ruby: Dir.pwd
来源：http://ddw.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://qte.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://eyo.zycfv.cn

Py:   sys.exit(1)
来源：http://voz.shuidangran.top

PHP:  exit(1);
来源：http://koh.aibaodan.cn

JS:   process.exit(1)
来源：http://hvd.yj202588.top

TS:   process.exit(1)
来源：http://qhg.meibo888.top

Java: System.exit(1)
来源：http://gbx.xuanzx.com

Go:   os.Exit(1)
来源：http://vka.zdbjq.cn

Ruby: exit 1
来源：http://nxz.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aei.cashguo.top

[M06] 向标准错误输出
来源：http://gcx.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://ken.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://zyc.jiagoushi.top

JS:   console.error("err")
来源：http://yhx.xinyue.icu

TS:   console.error("err")
来源：http://nhn.smart0.xyz

Java: System.err.println("err")
来源：http://zfp.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zkv.fehbvm.com

Ruby: warn "err"
来源：http://kdu.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://lwn.iojbl.cn

[M07] 判断是否为主入口
来源：http://mex.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://bmn.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bsl.yj20258.top

JS:   require.main === module
来源：http://now.xziqi.cn

TS:   require.main === module
来源：http://pyo.iojbl.cn

Java: public static void main(String[] args)
来源：http://fcs.gogol.net.cn

Go:   func main()
来源：http://nyk.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gna.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://sva.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://ycv.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://ibn.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://tef.shuidangran.top

JS:   process.platform;  process.version
来源：http://gzv.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://yde.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vjk.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://oyc.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wzq.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://gbm.kuanghao11.cn

================================================================================
来源：http://iif.yangfankeji.com

N. 数据结构与算法
来源：http://tqe.xziqi.cn

================================================================================
来源：http://pqd.yonumen.top

[N01] 二分查找（有序数组）
来源：http://cgr.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://qbi.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fbw.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://usq.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://olo.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nci.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://zio.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cyg.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://rgb.fzhhl.top

[N02] 排序（工程实践用内置实现）
来源：http://ivv.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://hho.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gtn.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ckx.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://udu.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bsy.tanke756.top

Go:   slices.Sort(arr)
来源：http://rto.jinqigfzy.top

Ruby: arr.sort
来源：http://oug.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://onv.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://gie.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lte.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://flg.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wja.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bvc.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://esc.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fyw.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kos.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://pop.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://vlk.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bzr.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qra.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgj.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mcw.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nyn.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qxb.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mrf.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tee.zhijiandao.cn

[N05] 最大公约数
来源：http://qcx.yonumen.top

Py:   math.gcd(a, b)
来源：http://gye.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zoo.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ecv.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tkq.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dkb.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://anr.xylfe.cn

Ruby: a.gcd(b)
来源：http://mqh.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://exw.yvedp.cn

[N06] 判断回文字符串
来源：http://dlk.daxiang520.top

Py:   s == s[::-1]
来源：http://zjx.vehdjk.com

PHP:  $s === strrev($s);
来源：http://xtc.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://efn.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://ybm.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jfn.guannengcc.top

Go:   // 双指针从两端比较
来源：http://qnh.wangdashe.top

Ruby: s == s.reverse
来源：http://oos.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fzf.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://qzk.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydo.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hce.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://zue.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://ftl.xuanzx.com

Java: // 手写 HashMap
来源：http://lsh.xinyue.icu

Go:   // 手写 map[int]int
来源：http://scw.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://uir.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://dym.jqgufenzy.top

[N08] 生成全排列
来源：http://ums.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://pph.nanxinkj.top

PHP:  // 手写递归交换
来源：http://naf.sufxvd.cn

JS:   // 手写回溯递归
来源：http://zax.chenzaomai.com

TS:   // 手写回溯递归
来源：http://wyf.zhengqikj.top

Java: // 手写回溯递归
来源：http://xww.cdnleiting.top

Go:   // 手写回溯递归
来源：http://dyw.yj20258.top

Ruby: arr.permutation.to_a
来源：http://nju.gotoacloud.top

C#:   // 手写回溯递归
来源：http://rak.meibo888.top

[N09] 栈与队列
来源：http://vwv.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://img.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qud.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ssa.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lzv.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eyq.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ykj.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cxg.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ssm.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://uku.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ghn.xylfe.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nyq.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://otw.sweek.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dxf.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://pmh.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://onv.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zex.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fuf.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://lom.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fkn.shzxlz.cn

PHP:  // 手写递归函数
来源：http://fps.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zrr.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvm.9152youxi.cn

Java: // 手写递归
来源：http://wmv.bbcook.cn

Go:   // 手写递归
来源：http://kux.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqd.bjfxy.top

C#:   // 手写递归
来源：http://urq.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tqx.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qyv.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://smo.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cih.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqw.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://btg.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nxe.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xuy.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://doj.ybcxt.top

================================================================================
来源：http://ndh.fktsv.cn

O. 并发与异步
来源：http://jwd.hesvh.cn

================================================================================
来源：http://kpi.yj20258888.top

[O01] 启动一个线程
来源：http://ahc.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sfj.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vij.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hmn.ydjk.org.cn

TS:   // 同 JS
来源：http://jkg.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://rko.xziqi.cn

Go:   go f()
来源：http://odu.aizwys.cn

Ruby: Thread.new { f }
来源：http://pek.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://jsp.zhengqikj.top

[O02] 使用线程池
来源：http://tbc.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hpb.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gwx.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://gey.shuidangran.top

TS:   // worker_threads 线程池
来源：http://oos.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://zra.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cqm.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pca.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ixn.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://crx.meibo888.top

Py:   with lock: shared += 1
来源：http://cfj.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://bme.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hlu.xziqi.cn

TS:   // 同 JS
来源：http://dzw.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://ghd.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nff.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bix.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://gxk.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://qzv.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://yej.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wyu.aizwys.cn

JS:   async function f() { await g(); }
来源：http://iwd.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ill.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mrv.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dme.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://ygz.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://ciy.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://ixd.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://zow.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uxi.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://egn.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://zeu.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pom.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fqd.xylfe.cn

Ruby: threads.map(&:join)
来源：http://clw.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zmw.hesvh.cn

[O06] 使用进程池
来源：http://elf.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yjr.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dgz.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://fao.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://ivr.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zgj.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mrx.xuetiantiany.cn

Ruby: // fork 块
来源：http://bom.hysaishi.cn


<!-- 参考信息 -->