代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctm.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vwz.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pkj.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lek.gzhubu.top

[L03] 设置自定义请求头
来源：http://ldu.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dmy.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ztp.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yav.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jag.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zan.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yao.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ung.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ljz.cdnleiting.top

[L04] 设置超时
来源：http://mvl.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://wmp.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yrs.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hac.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpl.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dyh.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cop.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sfz.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zzl.yueranfly.top

[L05] 上传文件（multipart）
来源：http://ilb.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://adf.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nmg.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bju.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://deq.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xqu.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qac.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bng.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://krj.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://vyu.jinqigfzy.top

Py:   resp.json()
来源：http://vdu.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://lbn.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://hbb.meibo888.top

TS:   await resp.json()
来源：http://slp.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kdm.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vrz.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://tqd.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vms.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://jtd.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vcb.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cxa.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://qdi.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://ysl.haohaochexian.top

Java: resp.statusCode()
来源：http://eyn.chenzaomai.com

Go:   resp.StatusCode
来源：http://qad.zhengqikj.top

Ruby: resp.code.to_i
来源：http://urq.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://vtf.hfpthk.cn

[L08] 并发请求多个地址
来源：http://jmi.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wmq.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://nfc.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vfk.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wkt.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pqj.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://byx.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ztw.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gff.nwbrower.top

================================================================================
来源：http://pav.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://ulm.vehdjk.com

================================================================================
来源：http://wmw.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://bwo.yonumen.top

Py:   sys.argv[1:]
来源：http://emo.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://mbe.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://epq.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://mwx.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://adw.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://ggo.shanyushiyangkeji.top

Ruby: ARGV
来源：http://agw.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://cug.jinqigfzy.top

[M02] 读取环境变量
来源：http://tjx.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://hxf.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wss.iojbl.cn

JS:   process.env.HOME
来源：http://fju.ivvv.top

TS:   process.env.HOME
来源：http://bfb.jinqigufen.top

Java: System.getenv("HOME")
来源：http://yci.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xtk.aizwys.cn

Ruby: ENV["HOME"]
来源：http://ueq.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://thm.bbcook.cn

[M03] 执行外部命令
来源：http://ogx.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cfz.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jqh.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yxb.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://gjb.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wco.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xkm.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://ezs.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://xxe.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://sfm.bjfxy.top

Py:   os.getcwd()
来源：http://jfv.sjlbkw.cn

PHP:  getcwd();
来源：http://ahz.kuanghao11.cn

JS:   process.cwd()
来源：http://lgi.hnxiangtu.top

TS:   process.cwd()
来源：http://kuf.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://gbe.aibaodan.cn

Go:   os.Getwd()
来源：http://ugg.ehwqpu.com

Ruby: Dir.pwd
来源：http://mdq.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ykx.vqdsnc.cn

[M05] 设置退出码
来源：http://rvi.kuanghao11.cn

Py:   sys.exit(1)
来源：http://gcv.cheryme.top

PHP:  exit(1);
来源：http://kne.zhongyouzk.top

JS:   process.exit(1)
来源：http://zfb.yj20258888.top

TS:   process.exit(1)
来源：http://riz.epnwcf.com

Java: System.exit(1)
来源：http://pwq.hfpthk.cn

Go:   os.Exit(1)
来源：http://paa.ybcxt.top

Ruby: exit 1
来源：http://slg.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://phi.tanke756.top

[M06] 向标准错误输出
来源：http://kjy.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://cxo.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://scz.ppjwa.cn

JS:   console.error("err")
来源：http://vxp.shzxlz.cn

TS:   console.error("err")
来源：http://mxc.hnxiangtu.top

Java: System.err.println("err")
来源：http://plq.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lpl.hywenlv.cn

Ruby: warn "err"
来源：http://dtp.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://yco.andypj.xyz

[M07] 判断是否为主入口
来源：http://fva.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://cir.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dwc.cucudq.cn

JS:   require.main === module
来源：http://jyk.ybcxt.top

TS:   require.main === module
来源：http://fti.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://lfl.jiagoushi.top

Go:   func main()
来源：http://xoq.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rdp.hammf.cn

C#:   static void Main(string[] args)
来源：http://wja.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://mfi.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://mbf.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://rqa.yueranfly.top

JS:   process.platform;  process.version
来源：http://jwb.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://bih.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpq.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tgg.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nuw.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nal.chenzaomai.com

================================================================================
来源：http://tle.tanke756.top

N. 数据结构与算法
来源：http://osc.zhiwuduotai.top

================================================================================
来源：http://dux.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://kho.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://arq.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ibb.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ntu.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zbx.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qqq.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://iwf.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://imw.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ujq.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://anr.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://zeo.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vbu.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bxb.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vfs.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://voy.yongpay.top

Go:   slices.Sort(arr)
来源：http://pkg.quarkkingdee.top

Ruby: arr.sort
来源：http://gbl.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://gep.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://gyw.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oby.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://sqg.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxq.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ajy.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kip.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jnb.quarkkingdee.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vas.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://odu.tanke756.top

[N04] 斐波那契数列
来源：http://lvy.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yfo.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pxj.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivx.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://src.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ved.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jin.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lqt.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nad.xziqi.cn

[N05] 最大公约数
来源：http://lwz.pycfn.com

Py:   math.gcd(a, b)
来源：http://fsd.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vxn.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wdl.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vxt.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://drk.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uwa.sysykeji.top

Ruby: a.gcd(b)
来源：http://fol.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://buw.redwolf501.top

[N06] 判断回文字符串
来源：http://xtn.jyoumei.cn

Py:   s == s[::-1]
来源：http://lel.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://wlj.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://ezi.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://ttf.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kue.epnwcf.com

Go:   // 双指针从两端比较
来源：http://xzz.yvedp.cn

Ruby: s == s.reverse
来源：http://jne.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vmy.pycfn.com

[N07] 两数之和（返回下标）
来源：http://hoy.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qho.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://knh.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zsq.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://psp.zdbjq.cn

Java: // 手写 HashMap
来源：http://gaa.bjfxy.top

Go:   // 手写 map[int]int
来源：http://zar.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://egq.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nbq.pycfn.com

[N08] 生成全排列
来源：http://qhr.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://mdd.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://dla.tianlin.xyz

JS:   // 手写回溯递归
来源：http://abq.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://rqb.hnqzz.top

Java: // 手写回溯递归
来源：http://kkw.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://dcq.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://xqv.bbcook.cn

C#:   // 手写回溯递归
来源：http://mfo.shangyingyoupin.top

[N09] 栈与队列
来源：http://jie.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dqd.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://que.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jnt.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kek.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://krc.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dwx.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aap.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfh.andypj.xyz

[N10] 链表节点定义
来源：http://mwv.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hkl.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jxb.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dtb.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://izx.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://mkc.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://afx.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://geh.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ccn.fehbvm.com

[N11] 二叉树中序遍历
来源：http://jsc.sysykeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qsq.chenzaomai.com

PHP:  // 手写递归函数
来源：http://lwr.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzm.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tuu.yangfankeji.com

Java: // 手写递归
来源：http://luk.xuetiantiany.cn

Go:   // 手写递归
来源：http://ujk.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://svu.xylfe.cn

C#:   // 手写递归
来源：http://whc.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mrq.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cus.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ghx.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pbm.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://giv.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://can.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hzk.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cwl.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bzm.cheryme.top

================================================================================
来源：http://dnj.chenjidiqi.icu

O. 并发与异步
来源：http://yha.uphjek.com

================================================================================
来源：http://abn.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://igt.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dgi.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vtz.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://krz.feifeiyinyue.top

TS:   // 同 JS
来源：http://gvn.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://big.yueranfly.top

Go:   go f()
来源：http://wha.jyoumei.cn

Ruby: Thread.new { f }
来源：http://asq.cheryme.top

C#:   Task.Run(() => F());
来源：http://wwo.bjfxy.top

[O02] 使用线程池
来源：http://xan.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://buy.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aox.sysykeji.top

JS:   // worker_threads 线程池
来源：http://fcd.hnqzz.top

TS:   // worker_threads 线程池
来源：http://lwx.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://yum.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://joy.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qio.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yzy.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://qni.svipenyu.cn

Py:   with lock: shared += 1
来源：http://jbf.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://kes.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eml.xziqi.cn

TS:   // 同 JS
来源：http://irj.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://myw.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tqh.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://woe.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://qow.316326.xyz

[O04] 定义异步函数并等待
来源：http://jwx.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://nwe.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhj.pycfn.com

JS:   async function f() { await g(); }
来源：http://cdh.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qhr.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xcm.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wen.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sxl.uphjek.com

C#:   async Task F() { await G(); }
来源：http://air.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://ngs.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://ziv.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://daf.316326.xyz

JS:   await Promise.all(tasks)
来源：http://bow.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://mjr.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wyb.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://szv.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://hvk.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kgm.dashuyun.cn

[O06] 使用进程池
来源：http://uhj.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xrl.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rby.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://pxw.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://wlm.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bpr.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mlf.zdbjq.cn

Ruby: // fork 块
来源：http://mcb.yfazqb.com


<!-- 参考信息 -->