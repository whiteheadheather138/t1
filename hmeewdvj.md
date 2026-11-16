代发 wailian999

[L03] 设置自定义请求头
来源：http://qeu.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://apt.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pyy.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://koa.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mpf.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bwe.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pbf.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ait.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ptr.yongpay.top

[L04] 设置超时
来源：http://zwl.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://nkn.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zaw.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uui.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jay.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eem.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zbo.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mow.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lfa.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://kid.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hrn.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uye.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://seo.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://byh.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eig.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qmx.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zcf.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cit.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://hge.cucudq.cn

Py:   resp.json()
来源：http://eud.fktsv.cn

PHP:  json_decode($body, true);
来源：http://bmj.hesvh.cn

JS:   await resp.json()
来源：http://wsl.yvedp.cn

TS:   await resp.json()
来源：http://cnn.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://umn.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vzh.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://som.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dcx.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://snf.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pir.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zoo.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://ade.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://odf.zhijiandao.cn

Java: resp.statusCode()
来源：http://xzi.meibo888.top

Go:   resp.StatusCode
来源：http://csp.bbcook.cn

Ruby: resp.code.to_i
来源：http://lic.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://prq.zdbjq.cn

[L08] 并发请求多个地址
来源：http://mnq.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kcn.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://gto.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olm.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mkc.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://isg.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xrs.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gsu.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ufj.daria6918.cn

================================================================================
来源：http://lcv.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://rhh.daria6918.cn

================================================================================
来源：http://lwu.gotoacloud.top

[M01] 读取命令行参数
来源：http://wwr.fktsv.cn

Py:   sys.argv[1:]
来源：http://vmf.ybcxt.top

PHP:  $argv;  $argc;
来源：http://trn.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://zyn.jianghu66.top

TS:   process.argv.slice(2)
来源：http://ptk.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://asd.snrcjt.cn

Go:   os.Args[1:]
来源：http://hik.yanxiufei.cn

Ruby: ARGV
来源：http://moi.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://sca.xuetiantiany.cn

[M02] 读取环境变量
来源：http://nbq.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://aqw.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://phz.yvedp.cn

JS:   process.env.HOME
来源：http://eiq.xylfe.cn

TS:   process.env.HOME
来源：http://nfv.iojbl.cn

Java: System.getenv("HOME")
来源：http://ctq.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ofn.yonumen.top

Ruby: ENV["HOME"]
来源：http://wws.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ogq.zdqjudy.top

[M03] 执行外部命令
来源：http://nte.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qio.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ojc.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zto.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fvm.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aqv.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fuv.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xnq.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://wky.fzhhl.top

[M04] 获取当前工作目录
来源：http://ymb.cucudq.cn

Py:   os.getcwd()
来源：http://brg.yj202588.top

PHP:  getcwd();
来源：http://nna.daxiang520.top

JS:   process.cwd()
来源：http://dsj.9152youxi.cn

TS:   process.cwd()
来源：http://sem.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://mhv.yj202588.top

Go:   os.Getwd()
来源：http://lfv.jqgfzy.top

Ruby: Dir.pwd
来源：http://ooa.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://pyb.pengpengdd.cyou

[M05] 设置退出码
来源：http://ggk.uphjek.com

Py:   sys.exit(1)
来源：http://dfm.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://ztm.ivvv.top

JS:   process.exit(1)
来源：http://eno.kuanghao11.cn

TS:   process.exit(1)
来源：http://jhj.hnqzz.top

Java: System.exit(1)
来源：http://kjo.yfazqb.com

Go:   os.Exit(1)
来源：http://xdx.snrcjt.cn

Ruby: exit 1
来源：http://ulz.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cps.hfpthk.cn

[M06] 向标准错误输出
来源：http://jkw.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://lqq.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://noe.yj202588.top

JS:   console.error("err")
来源：http://ahk.cucudq.cn

TS:   console.error("err")
来源：http://sck.shangyingyoupin.top

Java: System.err.println("err")
来源：http://qqe.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xyj.wangdashe.top

Ruby: warn "err"
来源：http://gbe.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://nzd.mhx1999.top

[M07] 判断是否为主入口
来源：http://bnm.316326.xyz

Py:   if __name__ == "__main__":
来源：http://fit.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hpg.sxryk.cn

JS:   require.main === module
来源：http://eim.xinyue.icu

TS:   require.main === module
来源：http://kpa.epnwcf.com

Java: public static void main(String[] args)
来源：http://ibk.9152youxi.cn

Go:   func main()
来源：http://qbb.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oam.yongpay.top

C#:   static void Main(string[] args)
来源：http://egu.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://ewa.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://vdw.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://tgk.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://vpa.iojbl.cn

TS:   process.platform;  process.version
来源：http://kmk.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tdq.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xtq.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qmb.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qkv.hnqzz.top

================================================================================
来源：http://mto.chenzaomai.com

N. 数据结构与算法
来源：http://lvy.pengpengdd.cyou

================================================================================
来源：http://qse.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://wnh.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hpn.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zsy.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rxq.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bgr.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://thh.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://ndq.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wya.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://ayg.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://jlk.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://dbk.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qgk.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://tkz.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dlb.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ien.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://kkh.hammf.cn

Ruby: arr.sort
来源：http://nhr.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sai.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://pet.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://whe.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://tsa.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fzx.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eht.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dcz.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mod.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kxp.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://qug.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://jlv.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hxs.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ccb.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nit.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lsz.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://upa.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mhc.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sqr.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://unu.dianchejie.cn

[N05] 最大公约数
来源：http://gsu.birdmap.top

Py:   math.gcd(a, b)
来源：http://uqm.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dlw.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jea.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mcv.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czq.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avv.cdnleiting.top

Ruby: a.gcd(b)
来源：http://dep.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dfp.hysaishi.cn

[N06] 判断回文字符串
来源：http://ezk.jiagoushi.top

Py:   s == s[::-1]
来源：http://ppm.hesvh.cn

PHP:  $s === strrev($s);
来源：http://tms.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://hud.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://wuj.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bwi.ivvv.top

Go:   // 双指针从两端比较
来源：http://jad.zycfv.cn

Ruby: s == s.reverse
来源：http://kxd.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://twp.sweek.top

[N07] 两数之和（返回下标）
来源：http://xgd.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kxg.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hjn.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sis.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://scv.zhoulong.xyz

Java: // 手写 HashMap
来源：http://vrx.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://umy.guannengcc.top

Ruby: // 手写 Hash
来源：http://hkc.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://oob.wangshuangyany.cn

[N08] 生成全排列
来源：http://cfc.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://qqa.yj202588.top

PHP:  // 手写递归交换
来源：http://amf.yfazqb.com

JS:   // 手写回溯递归
来源：http://egx.zhengqikj.top

TS:   // 手写回溯递归
来源：http://ubm.cashguo.top

Java: // 手写回溯递归
来源：http://xue.nwbrower.top

Go:   // 手写回溯递归
来源：http://hiv.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://vqg.chenlongwang.top

C#:   // 手写回溯递归
来源：http://yks.fzhhl.top

[N09] 栈与队列
来源：http://mgt.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xcp.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bjm.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ihm.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ptm.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vzs.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qff.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://htt.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvn.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://kfj.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fxc.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://mfc.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pms.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ipk.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://lky.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://nva.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lup.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yad.xziqi.cn

[N11] 二叉树中序遍历
来源：http://cnk.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bke.kuanghao11.cn

PHP:  // 手写递归函数
来源：http://mjs.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wej.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jxe.sxryk.cn

Java: // 手写递归
来源：http://fiw.0kj1m.cn

Go:   // 手写递归
来源：http://rdq.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://buv.daria6918.cn

C#:   // 手写递归
来源：http://ytu.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ywy.yj202588.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jfr.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rpn.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xai.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hyh.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jpo.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dko.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ple.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://csz.zhixingplan.top

================================================================================
来源：http://nbw.yueranfly.top

O. 并发与异步
来源：http://nak.ivvv.top

================================================================================
来源：http://cvh.chenjidiqi.icu

[O01] 启动一个线程
来源：http://kzx.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wpz.jlsjyb.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://usx.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pin.jlsjyb.cn

TS:   // 同 JS
来源：http://qiw.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://sox.52xcode.cn

Go:   go f()
来源：http://mkr.tian-w.cn

Ruby: Thread.new { f }
来源：http://fsj.yj20258888.top

C#:   Task.Run(() => F());
来源：http://zpf.pengpengdd.cyou

[O02] 使用线程池
来源：http://aga.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kfb.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aox.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://zmt.bjfxy.top

TS:   // worker_threads 线程池
来源：http://cho.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://iqy.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gfd.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://djy.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uom.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://trh.hywenlv.cn

Py:   with lock: shared += 1
来源：http://nwh.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://glz.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ysg.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://fmc.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://djv.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aux.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fnj.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://asz.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://dhe.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://rwd.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iks.bbcook.cn

JS:   async function f() { await g(); }
来源：http://rng.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ych.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cex.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ert.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://uij.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://oxt.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://lpb.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://exb.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://agf.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://ykz.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://yuc.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://heo.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fao.dianchejie.cn

Ruby: threads.map(&:join)
来源：http://jgv.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kaf.hongshengwenyu.top

[O06] 使用进程池
来源：http://pyu.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gvw.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vxi.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://thb.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://djm.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kfj.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fqy.fanxiaobao.xyz

Ruby: // fork 块
来源：http://asx.jinqigfzy.top

C#:   Parallel.For
来源：http://lfl.52xcode.cn

================================================================================
来源：http://vlc.aizwys.cn

P. 常用工具函数
来源：http://vhn.yonumen.top

================================================================================
来源：http://rkx.bjfxy.top


<!-- 参考信息 -->