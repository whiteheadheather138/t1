代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://inv.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cdp.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sxc.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://svu.sufxvd.cn

[L03] 设置自定义请求头
来源：http://gdc.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://isq.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://toq.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qto.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uoq.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://odb.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rfk.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zqe.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cxt.zhixingplan.top

[L04] 设置超时
来源：http://spz.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://ayu.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iff.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azd.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vgi.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ttx.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://urh.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wwp.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qur.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://ovr.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://miq.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nnm.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vdh.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tat.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://avz.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qac.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gyi.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://phz.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://dws.gogol.net.cn

Py:   resp.json()
来源：http://yjb.ydzc1.top

PHP:  json_decode($body, true);
来源：http://vqd.sweek.top

JS:   await resp.json()
来源：http://xsd.daria6918.cn

TS:   await resp.json()
来源：http://jfs.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mgo.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fvl.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://uym.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jdf.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://vxg.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mkm.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gqj.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://iiu.sweek.top

TS:   resp.ok;  resp.status
来源：http://hru.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://nmn.aibaodan.cn

Go:   resp.StatusCode
来源：http://xpd.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://bez.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://gbn.snrcjt.cn

[L08] 并发请求多个地址
来源：http://ggd.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cnr.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://vdj.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ner.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fcm.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fpv.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://woq.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://itc.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vkl.jianghu66.top

================================================================================
来源：http://fkp.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://wru.fengsongda.top

================================================================================
来源：http://nmi.yongpay.top

[M01] 读取命令行参数
来源：http://ifo.birdmap.top

Py:   sys.argv[1:]
来源：http://zlq.hnqzz.top

PHP:  $argv;  $argc;
来源：http://kvf.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://zjx.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://mky.cashguo.top

Java: args 数组（main 方法参数）
来源：http://gey.yueranfly.top

Go:   os.Args[1:]
来源：http://rnd.cashguo.top

Ruby: ARGV
来源：http://ors.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://ohv.bbcook.cn

[M02] 读取环境变量
来源：http://zlj.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://chj.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ybe.cashguo.top

JS:   process.env.HOME
来源：http://qrs.tanke756.top

TS:   process.env.HOME
来源：http://apy.fktsv.cn

Java: System.getenv("HOME")
来源：http://wkp.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nxx.cheryme.top

Ruby: ENV["HOME"]
来源：http://dwt.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lpc.yvedp.cn

[M03] 执行外部命令
来源：http://pjr.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cxh.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cey.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zwc.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://shx.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bdi.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aky.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kbp.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://ymx.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://slc.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://jup.c1oappe.top

PHP:  getcwd();
来源：http://omy.gaohongyu789.top

JS:   process.cwd()
来源：http://gxb.hcnkem.com

TS:   process.cwd()
来源：http://fts.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://kub.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://usk.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://kuv.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://vou.gzhubu.top

[M05] 设置退出码
来源：http://goe.fzhhl.top

Py:   sys.exit(1)
来源：http://fgp.yueranfly.top

PHP:  exit(1);
来源：http://efo.ybcxt.top

JS:   process.exit(1)
来源：http://vki.cqqwz.cn

TS:   process.exit(1)
来源：http://itv.gogol.net.cn

Java: System.exit(1)
来源：http://kco.yfazqb.com

Go:   os.Exit(1)
来源：http://bcg.zhongyouzk.top

Ruby: exit 1
来源：http://vum.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pif.birdmap.top

[M06] 向标准错误输出
来源：http://yvr.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://gvl.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://des.aibaodan.cn

JS:   console.error("err")
来源：http://uaw.yfazqb.com

TS:   console.error("err")
来源：http://xfo.smart0.xyz

Java: System.err.println("err")
来源：http://dxg.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nmp.pengpengdd.cyou

Ruby: warn "err"
来源：http://yob.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://oks.bjfxy.top

[M07] 判断是否为主入口
来源：http://evi.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://ich.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ids.hnxiangtu.top

JS:   require.main === module
来源：http://eyl.xziqi.cn

TS:   require.main === module
来源：http://mfy.epnwcf.com

Java: public static void main(String[] args)
来源：http://hvn.ydzc1.top

Go:   func main()
来源：http://dlj.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fej.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://wjm.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://cun.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://unw.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://krf.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://ted.shzxlz.cn

TS:   process.platform;  process.version
来源：http://rsc.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aag.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wtr.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bqr.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cuz.cqqwz.cn

================================================================================
来源：http://lzd.yonumen.top

N. 数据结构与算法
来源：http://vek.tian-w.cn

================================================================================
来源：http://mef.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://yfg.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ghi.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yjm.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cyz.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbd.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://crd.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://hwu.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://oyu.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://nhy.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://tap.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://hwp.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xjc.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uab.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xli.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kxe.hnqzz.top

Go:   slices.Sort(arr)
来源：http://pdw.gogol.net.cn

Ruby: arr.sort
来源：http://olg.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://wyu.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://tmy.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mci.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://kkj.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tix.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://adl.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rfu.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eoe.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ejv.dianchejie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://alc.yfazqb.com

[N04] 斐波那契数列
来源：http://fxy.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ihx.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mim.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ism.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qtl.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fcz.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://okq.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://odu.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uwa.dashuyun.cn

[N05] 最大公约数
来源：http://ygd.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://ueo.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ymp.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wht.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgs.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pjz.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qvn.birdmap.top

Ruby: a.gcd(b)
来源：http://hjn.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rsw.guannengcc.top

[N06] 判断回文字符串
来源：http://oua.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://gys.hnqzz.top

PHP:  $s === strrev($s);
来源：http://khu.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://soq.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://lys.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rxx.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://vub.bjfxy.top

Ruby: s == s.reverse
来源：http://gcn.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lue.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://nag.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://djv.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cep.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mgm.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://rtl.quarkkingdee.top

Java: // 手写 HashMap
来源：http://gyq.yuxming.cn

Go:   // 手写 map[int]int
来源：http://cse.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://cyz.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lsb.yonumen.top

[N08] 生成全排列
来源：http://cpr.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://mmb.iojbl.cn

PHP:  // 手写递归交换
来源：http://tqw.guannengcc.top

JS:   // 手写回溯递归
来源：http://qjx.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://agi.yangfankeji.com

Java: // 手写回溯递归
来源：http://cps.ivvv.top

Go:   // 手写回溯递归
来源：http://ldn.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://qad.daria6918.cn

C#:   // 手写回溯递归
来源：http://hgr.chenjidiqi.icu

[N09] 栈与队列
来源：http://tei.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ywb.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tjk.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vbd.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gil.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pij.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gye.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bff.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hmf.nanxuanxn.top

[N10] 链表节点定义
来源：http://gnl.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kwf.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qsr.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tyt.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hee.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://mxc.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://cht.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ymq.tian-w.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ntt.havefunace.top

[N11] 二叉树中序遍历
来源：http://szn.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://exu.zhixingplan.top

PHP:  // 手写递归函数
来源：http://uan.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://krh.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mdm.tarul.cn

Java: // 手写递归
来源：http://exe.yvedp.cn

Go:   // 手写递归
来源：http://zhv.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://prn.yj202588.top

C#:   // 手写递归
来源：http://uvv.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://key.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xln.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tsl.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fwm.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bmk.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://upd.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://odf.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uis.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zta.yvedp.cn

================================================================================
来源：http://irp.yanxiufei.cn

O. 并发与异步
来源：http://mln.chenzaomai.com

================================================================================
来源：http://wdw.zhiwuduotai.top

[O01] 启动一个线程
来源：http://tto.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dfy.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nwt.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://loz.nwbrower.top

TS:   // 同 JS
来源：http://xjv.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://kcn.haohaochexian.top

Go:   go f()
来源：http://nko.cucudq.cn

Ruby: Thread.new { f }
来源：http://yov.smart0.xyz

C#:   Task.Run(() => F());
来源：http://wds.vqdsnc.cn

[O02] 使用线程池
来源：http://opc.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cao.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qbr.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://nwn.vehdjk.com

TS:   // worker_threads 线程池
来源：http://oyp.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://rug.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://icw.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eyl.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pvu.fehbvm.com

[O03] 加锁保护共享数据
来源：http://adt.hnqzz.top

Py:   with lock: shared += 1
来源：http://nbs.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://bky.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rne.yanxiufei.cn

TS:   // 同 JS
来源：http://dey.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://wce.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ngn.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://tam.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://fhq.316326.xyz

[O04] 定义异步函数并等待
来源：http://qtc.tanke756.top

Py:   async def f():⏎    await g()
来源：http://mhq.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kyq.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://wdr.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://oxq.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://atr.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oir.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://ugx.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://hck.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://hdm.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://vdx.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vkm.tarul.cn

JS:   await Promise.all(tasks)
来源：http://yhy.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://vwc.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ikl.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zkj.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://cbj.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ilu.smart0.xyz

[O06] 使用进程池
来源：http://vhe.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ibt.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nbf.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://lnb.yj20258.top

TS:   // child_process / cluster 模块
来源：http://lpe.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zbs.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vnc.epnwcf.com

Ruby: // fork 块
来源：http://kqn.tian-w.cn


<!-- 参考信息 -->