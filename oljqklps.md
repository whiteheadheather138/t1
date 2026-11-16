代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ukg.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xlm.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ghy.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nio.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://fon.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://abz.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uln.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://srj.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggl.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vyw.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://syy.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xxp.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cwk.zdbjq.cn

[L04] 设置超时
来源：http://jxy.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://lde.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nuz.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dja.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glk.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xgv.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pbx.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lko.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xpy.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://pca.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uyp.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cfw.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tbq.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jqb.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cys.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ftu.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oqr.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://apz.hammf.cn

[L06] 解析响应为 JSON
来源：http://pzl.aibaodan.cn

Py:   resp.json()
来源：http://ipg.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://lsv.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://syx.9152youxi.cn

TS:   await resp.json()
来源：http://bql.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lsv.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nje.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://nkr.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qoo.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://hez.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ddb.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://obe.cashguo.top

JS:   resp.ok;  resp.status
来源：http://tfg.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://lqd.jyoumei.cn

Java: resp.statusCode()
来源：http://ixu.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://koe.chenlongwang.top

Ruby: resp.code.to_i
来源：http://itk.yonumen.top

C#:   (int)resp.StatusCode
来源：http://gxm.yangfankeji.com

[L08] 并发请求多个地址
来源：http://whr.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iav.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://zvy.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgk.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhx.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gbs.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bgl.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qxf.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jfz.316326.xyz

================================================================================
来源：http://zdh.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://xyj.jqgufenzy.top

================================================================================
来源：http://njq.redwolf501.top

[M01] 读取命令行参数
来源：http://kpv.aizwys.cn

Py:   sys.argv[1:]
来源：http://xic.fzhhl.top

PHP:  $argv;  $argc;
来源：http://qgd.yongpay.top

JS:   process.argv.slice(2)
来源：http://uwv.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://eve.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://lnr.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://xtp.jinyuanbaomall.cn

Ruby: ARGV
来源：http://zty.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://obq.pengpengdd.cyou

[M02] 读取环境变量
来源：http://snr.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://wyq.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://you.fengsongda.top

JS:   process.env.HOME
来源：http://foj.yuanzhike.top

TS:   process.env.HOME
来源：http://wyi.hfpthk.cn

Java: System.getenv("HOME")
来源：http://jpv.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jlf.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://hrq.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gdw.xziqi.cn

[M03] 执行外部命令
来源：http://uze.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://skn.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nnd.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://glr.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fzz.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pwb.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dkj.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lmb.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://hmu.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://zyz.jiagoushi.top

Py:   os.getcwd()
来源：http://yxg.zhengqikj.top

PHP:  getcwd();
来源：http://cxj.gotoacloud.top

JS:   process.cwd()
来源：http://akz.hywenlv.cn

TS:   process.cwd()
来源：http://iff.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://hpr.zycfv.cn

Go:   os.Getwd()
来源：http://pjl.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://bsc.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zxl.yj20258888.top

[M05] 设置退出码
来源：http://khb.sufxvd.cn

Py:   sys.exit(1)
来源：http://lgw.sxryk.cn

PHP:  exit(1);
来源：http://awc.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://phv.uphjek.com

TS:   process.exit(1)
来源：http://hml.jinghuilouyu.cn

Java: System.exit(1)
来源：http://fdd.yuanzhike.top

Go:   os.Exit(1)
来源：http://yus.tianlin.xyz

Ruby: exit 1
来源：http://pqc.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://guh.daria6918.cn

[M06] 向标准错误输出
来源：http://uek.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://nrg.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qkb.yonumen.top

JS:   console.error("err")
来源：http://hrj.andypj.xyz

TS:   console.error("err")
来源：http://wun.52xcode.cn

Java: System.err.println("err")
来源：http://iev.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vkr.vehdjk.com

Ruby: warn "err"
来源：http://qzu.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://tbh.ctjpmb.com

[M07] 判断是否为主入口
来源：http://axg.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://vsm.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://csl.xuetiantiany.cn

JS:   require.main === module
来源：http://lyc.epnwcf.com

TS:   require.main === module
来源：http://fxa.cheryme.top

Java: public static void main(String[] args)
来源：http://stw.cucudq.cn

Go:   func main()
来源：http://viz.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wne.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://qhi.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://ksz.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://yfs.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ayh.uphjek.com

JS:   process.platform;  process.version
来源：http://wwp.52xcode.cn

TS:   process.platform;  process.version
来源：http://lhd.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jvk.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jzj.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ybg.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://bbd.svipenyu.cn

================================================================================
来源：http://gtm.pengpengdd.cyou

N. 数据结构与算法
来源：http://amb.jlsjyb.cn

================================================================================
来源：http://qcc.ivvv.top

[N01] 二分查找（有序数组）
来源：http://dto.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qxh.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oms.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tml.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bdk.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rro.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://mmy.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eig.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://kyr.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://tfe.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://eqd.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vqz.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uta.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zbl.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://umq.yuxming.cn

Go:   slices.Sort(arr)
来源：http://msm.gaohongyu789.top

Ruby: arr.sort
来源：http://kqj.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mzr.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://ajg.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qvz.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://pto.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sub.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://msh.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wfp.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bat.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://puf.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://djt.havefunace.top

[N04] 斐波那契数列
来源：http://vqq.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fau.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zvi.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dhv.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dke.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fqq.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dfe.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vkv.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kci.zhijiandao.cn

[N05] 最大公约数
来源：http://jne.daxiang520.top

Py:   math.gcd(a, b)
来源：http://emk.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://owh.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qqb.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sni.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nzb.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zgp.dianchejie.cn

Ruby: a.gcd(b)
来源：http://egn.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dfy.yueranfly.top

[N06] 判断回文字符串
来源：http://rth.gaohongyu789.top

Py:   s == s[::-1]
来源：http://tbt.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://esu.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://uqa.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://nec.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kuk.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://mqa.zhengqikj.top

Ruby: s == s.reverse
来源：http://ylj.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://jog.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://chv.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bjz.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fbw.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://byl.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://ncn.hammf.cn

Java: // 手写 HashMap
来源：http://edg.xziqi.cn

Go:   // 手写 map[int]int
来源：http://klj.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://yij.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://wkt.cqqwz.cn

[N08] 生成全排列
来源：http://cfq.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://rsf.iojbl.cn

PHP:  // 手写递归交换
来源：http://qtc.yongpay.top

JS:   // 手写回溯递归
来源：http://afg.yongpay.top

TS:   // 手写回溯递归
来源：http://iev.cashguo.top

Java: // 手写回溯递归
来源：http://mdm.havefunace.top

Go:   // 手写回溯递归
来源：http://jxq.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://hfd.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://fjw.chenzaomai.com

[N09] 栈与队列
来源：http://qlq.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pju.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ihx.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gfw.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xld.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kfb.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pni.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zyk.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ztf.ivvv.top

[N10] 链表节点定义
来源：http://wpl.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tmy.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://swc.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ggp.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ptt.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://omc.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cnx.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gxk.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nri.vehdjk.com

[N11] 二叉树中序遍历
来源：http://twe.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wdy.fzhhl.top

PHP:  // 手写递归函数
来源：http://wbw.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lbn.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfc.gotoacloud.top

Java: // 手写递归
来源：http://rqn.yj20258888.top

Go:   // 手写递归
来源：http://gei.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lip.zhoulong.xyz

C#:   // 手写递归
来源：http://lvl.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pzt.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xas.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zbg.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qai.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eme.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ndg.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aff.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://abp.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://quj.tian-w.cn

================================================================================
来源：http://mfq.cashguo.top

O. 并发与异步
来源：http://egy.9152youxi.cn

================================================================================
来源：http://lof.guowangkeji.top

[O01] 启动一个线程
来源：http://cep.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pfu.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rrc.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://idq.cheryme.top

TS:   // 同 JS
来源：http://gkx.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://ljj.smart0.xyz

Go:   go f()
来源：http://sut.ydzc1.top

Ruby: Thread.new { f }
来源：http://moa.yonumen.top

C#:   Task.Run(() => F());
来源：http://whq.birdmap.top

[O02] 使用线程池
来源：http://etc.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://azn.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ikm.ivvv.top

JS:   // worker_threads 线程池
来源：http://eel.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://ibo.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://jzk.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mty.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rgr.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://trs.meibo888.top

[O03] 加锁保护共享数据
来源：http://qmx.guannengcc.top

Py:   with lock: shared += 1
来源：http://awg.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://gxu.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hoc.shangyingyoupin.top

TS:   // 同 JS
来源：http://acz.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://mlj.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jqf.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://qhw.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://lmy.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://wyl.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://qhj.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ycx.wangdashe.top

JS:   async function f() { await g(); }
来源：http://wpd.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://alc.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kgc.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gol.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://uel.birdmap.top

C#:   async Task F() { await G(); }
来源：http://zzp.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://dyq.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://lvn.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://upp.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://dmw.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://cgy.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://srd.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bvt.andypj.xyz

Ruby: threads.map(&:join)
来源：http://slp.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://qmd.ivvv.top

[O06] 使用进程池
来源：http://rqa.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ppi.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ppu.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://opp.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://dch.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cne.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://amf.jinqigufen.top

Ruby: // fork 块
来源：http://sui.xingfuxueyuan.xyz


<!-- 参考信息 -->