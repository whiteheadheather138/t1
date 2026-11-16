代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://egl.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ltq.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vze.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jma.ybcxt.top

[L03] 设置自定义请求头
来源：http://agt.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xhm.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gme.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tkx.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebh.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hhi.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mmp.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ywo.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://agq.tian-w.cn

[L04] 设置超时
来源：http://nuo.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://mae.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nqc.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bys.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rov.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dzd.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbc.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kvu.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ewx.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://psm.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zvy.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mzp.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kpv.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pgb.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rpm.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wxi.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jic.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://smi.andypj.xyz

[L06] 解析响应为 JSON
来源：http://fnb.tian-w.cn

Py:   resp.json()
来源：http://rip.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://bdz.yvedp.cn

JS:   await resp.json()
来源：http://olx.gotoacloud.top

TS:   await resp.json()
来源：http://pam.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qjz.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lci.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://dcg.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rjr.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://uwr.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vsh.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfw.yj20258.top

JS:   resp.ok;  resp.status
来源：http://jah.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://mas.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://xig.ppjwa.cn

Go:   resp.StatusCode
来源：http://pme.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://zkk.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://ogm.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://vec.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ngq.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://ymu.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oss.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kpx.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mmj.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fyh.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wyw.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mjq.andypj.xyz

================================================================================
来源：http://vym.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://gmv.aizwys.cn

================================================================================
来源：http://nml.jinqigfzy.top

[M01] 读取命令行参数
来源：http://wle.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://eqf.fengsongda.top

PHP:  $argv;  $argc;
来源：http://ebs.tian-w.cn

JS:   process.argv.slice(2)
来源：http://tay.tian-w.cn

TS:   process.argv.slice(2)
来源：http://ftz.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://tgh.tarul.cn

Go:   os.Args[1:]
来源：http://piu.jinqigufen.top

Ruby: ARGV
来源：http://nrc.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://taq.fanxiaobao.xyz

[M02] 读取环境变量
来源：http://izu.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://ski.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://thn.316326.xyz

JS:   process.env.HOME
来源：http://rff.fktsv.cn

TS:   process.env.HOME
来源：http://gey.redwolf501.top

Java: System.getenv("HOME")
来源：http://zwt.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lyo.sysykeji.top

Ruby: ENV["HOME"]
来源：http://mmc.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gnm.yj20258888.top

[M03] 执行外部命令
来源：http://wim.52xcode.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oct.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://day.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qnc.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fkw.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://czd.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ync.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://jqs.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://agl.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://daj.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://ynr.nwbrower.top

PHP:  getcwd();
来源：http://hog.yonumen.top

JS:   process.cwd()
来源：http://eug.jqgufenzy.top

TS:   process.cwd()
来源：http://gba.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://dht.pycfn.com

Go:   os.Getwd()
来源：http://wqa.9152youxi.cn

Ruby: Dir.pwd
来源：http://jad.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://mje.zdqjudy.top

[M05] 设置退出码
来源：http://qop.gzhubu.top

Py:   sys.exit(1)
来源：http://nhu.chenlongwang.top

PHP:  exit(1);
来源：http://cbz.epnwcf.com

JS:   process.exit(1)
来源：http://dxh.gotoacloud.top

TS:   process.exit(1)
来源：http://ihf.9152youxi.cn

Java: System.exit(1)
来源：http://bxn.316326.xyz

Go:   os.Exit(1)
来源：http://shl.cdnleiting.top

Ruby: exit 1
来源：http://tgm.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://srn.zdbjq.cn

[M06] 向标准错误输出
来源：http://fmd.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://zwd.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tjl.zhoulong.xyz

JS:   console.error("err")
来源：http://ous.vehdjk.com

TS:   console.error("err")
来源：http://tcu.hcnkem.com

Java: System.err.println("err")
来源：http://lvg.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xzv.uphjek.com

Ruby: warn "err"
来源：http://vax.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://ufw.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://dkp.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://fdt.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgd.feifeiyinyue.top

JS:   require.main === module
来源：http://gkl.shanyushiyangkeji.top

TS:   require.main === module
来源：http://ems.cqqwz.cn

Java: public static void main(String[] args)
来源：http://ubz.zycfv.cn

Go:   func main()
来源：http://bnh.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://heb.wangdashe.top

C#:   static void Main(string[] args)
来源：http://otd.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://kid.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://dms.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://ekr.snrcjt.cn

JS:   process.platform;  process.version
来源：http://noz.ybcxt.top

TS:   process.platform;  process.version
来源：http://kit.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tym.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://wdf.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lmv.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ujm.meibo888.top

================================================================================
来源：http://evn.jinghuilouyu.cn

N. 数据结构与算法
来源：http://kjh.vehdjk.com

================================================================================
来源：http://vfm.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://yca.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://obe.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://guc.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pko.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sds.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://lhb.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://vya.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://emc.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nln.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://dsb.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://xzi.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ypu.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mvo.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nxa.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://spl.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://rvv.tianlin.xyz

Ruby: arr.sort
来源：http://oud.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pdw.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://gpb.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggi.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://vaz.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nyc.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mid.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dbo.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yca.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gsy.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://grs.jiagoushi.top

[N04] 斐波那契数列
来源：http://hvz.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://obt.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://opp.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zri.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://huj.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://itj.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iht.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ezf.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://esp.feifeiyinyue.top

[N05] 最大公约数
来源：http://agk.hammf.cn

Py:   math.gcd(a, b)
来源：http://dou.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wln.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jej.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xwm.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qld.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vqf.nwbrower.top

Ruby: a.gcd(b)
来源：http://zxa.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dax.cashguo.top

[N06] 判断回文字符串
来源：http://pmc.zhengqikj.top

Py:   s == s[::-1]
来源：http://koc.nwbrower.top

PHP:  $s === strrev($s);
来源：http://bao.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://nxz.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://vfn.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xit.zycfv.cn

Go:   // 双指针从两端比较
来源：http://vtb.gzhubu.top

Ruby: s == s.reverse
来源：http://wjj.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://wlh.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://wvq.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rmt.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pym.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://roe.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://fqa.xylfe.cn

Java: // 手写 HashMap
来源：http://gsy.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://kxy.cdnleiting.top

Ruby: // 手写 Hash
来源：http://yxz.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://onc.bjfxy.top

[N08] 生成全排列
来源：http://hjj.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://wuo.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://vvp.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://pdd.hammf.cn

TS:   // 手写回溯递归
来源：http://kxw.jinqigufen.top

Java: // 手写回溯递归
来源：http://hrn.guannengcc.top

Go:   // 手写回溯递归
来源：http://frv.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://cbl.bjfxy.top

C#:   // 手写回溯递归
来源：http://wgw.hnxiangtu.top

[N09] 栈与队列
来源：http://kar.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jph.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gyw.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kab.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zqe.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qsp.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rrl.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lrq.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nqd.zycfv.cn

[N10] 链表节点定义
来源：http://ywi.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kfw.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rzc.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyc.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qpf.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://wtr.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://utr.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ukq.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://isq.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://ljz.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uvu.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://wyd.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xtm.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uxn.gaohongyu789.top

Java: // 手写递归
来源：http://ddu.hcnkem.com

Go:   // 手写递归
来源：http://ojo.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://myk.yangfankeji.com

C#:   // 手写递归
来源：http://omn.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jem.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://arr.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yqa.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://viu.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hai.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zxd.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wes.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ukk.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dru.9152youxi.cn

================================================================================
来源：http://qvn.yonumen.top

O. 并发与异步
来源：http://pek.gotoacloud.top

================================================================================
来源：http://kgj.hnqzz.top

[O01] 启动一个线程
来源：http://bjx.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jbx.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ijh.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://phh.yanxiufei.cn

TS:   // 同 JS
来源：http://ggv.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://hjn.hfpthk.cn

Go:   go f()
来源：http://yfv.sysykeji.top

Ruby: Thread.new { f }
来源：http://lqs.yfazqb.com

C#:   Task.Run(() => F());
来源：http://lzp.fengsongda.top

[O02] 使用线程池
来源：http://bci.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yli.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xqs.epnwcf.com

JS:   // worker_threads 线程池
来源：http://mot.yueranfly.top

TS:   // worker_threads 线程池
来源：http://hkv.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nsc.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gfc.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gid.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lpn.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://krz.yangfankeji.com

Py:   with lock: shared += 1
来源：http://zdr.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://vdh.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ylj.svipenyu.cn

TS:   // 同 JS
来源：http://zzw.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://ptn.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hsi.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndg.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://rwn.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://vyz.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://cgz.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jft.yongpay.top

JS:   async function f() { await g(); }
来源：http://ewj.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ujw.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ovv.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vju.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://zvq.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://ijk.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://cdu.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://wdh.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://von.cheryme.top

JS:   await Promise.all(tasks)
来源：http://rzk.meibo888.top

TS:   await Promise.all(tasks)
来源：http://kjz.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xne.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jns.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://via.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dyg.iojbl.cn

[O06] 使用进程池
来源：http://nfx.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hye.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://avb.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://lvz.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://yab.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kyn.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ukd.haohaochexian.top

Ruby: // fork 块
来源：http://pqg.cdnleiting.top


<!-- 参考信息 -->