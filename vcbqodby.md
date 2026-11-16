代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://gtv.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qts.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bxn.tianlin.xyz

[L02] 发送 POST JSON
来源：http://iiv.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://kkq.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mxo.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jvf.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ewb.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qah.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://roo.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ukg.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://stm.ydzc1.top

[L03] 设置自定义请求头
来源：http://nqq.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qbu.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iry.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ryy.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://glz.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qcy.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://soo.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://evx.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kku.zycfv.cn

[L04] 设置超时
来源：http://umn.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://iym.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ojr.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ntr.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwo.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zqd.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xrz.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oxt.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pdc.yonumen.top

[L05] 上传文件（multipart）
来源：http://bzh.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vbk.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nmg.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fzd.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bql.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zyk.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rkb.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jcd.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nqe.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://ooh.yj20258888.top

Py:   resp.json()
来源：http://zne.tanke756.top

PHP:  json_decode($body, true);
来源：http://vfx.birdmap.top

JS:   await resp.json()
来源：http://hie.yvedp.cn

TS:   await resp.json()
来源：http://btc.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qhc.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wbz.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://nrg.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cnq.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://gyu.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wuk.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://owu.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://fzt.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://zqp.birdmap.top

Java: resp.statusCode()
来源：http://rqc.hammf.cn

Go:   resp.StatusCode
来源：http://xyi.yfazqb.com

Ruby: resp.code.to_i
来源：http://lzn.sweek.top

C#:   (int)resp.StatusCode
来源：http://znc.sufxvd.cn

[L08] 并发请求多个地址
来源：http://qey.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wlb.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://cas.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dhv.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eme.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wqu.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dwu.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://czy.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://myo.yanxiufei.cn

================================================================================
来源：http://hwa.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://jzn.cqqwz.cn

================================================================================
来源：http://ozt.yueranfly.top

[M01] 读取命令行参数
来源：http://pqs.sysykeji.top

Py:   sys.argv[1:]
来源：http://hbk.daria6918.cn

PHP:  $argv;  $argc;
来源：http://qax.bjfxy.top

JS:   process.argv.slice(2)
来源：http://kku.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://aqq.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://cnw.jqgufenzy.top

Go:   os.Args[1:]
来源：http://lhk.sxryk.cn

Ruby: ARGV
来源：http://ykx.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://fkd.jiagoushi.top

[M02] 读取环境变量
来源：http://mmy.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://nwc.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zyw.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://vag.316326.xyz

TS:   process.env.HOME
来源：http://npm.xinyue.icu

Java: System.getenv("HOME")
来源：http://zpb.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pvm.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://gqd.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iwi.nwbrower.top

[M03] 执行外部命令
来源：http://sjf.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://acn.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qht.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ifj.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mcb.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yze.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://phk.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://gzx.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://aaa.chenzaomai.com

[M04] 获取当前工作目录
来源：http://xia.svipenyu.cn

Py:   os.getcwd()
来源：http://iwu.bjfxy.top

PHP:  getcwd();
来源：http://zpu.yj202588.top

JS:   process.cwd()
来源：http://prg.hnxiangtu.top

TS:   process.cwd()
来源：http://aoh.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://qps.yfazqb.com

Go:   os.Getwd()
来源：http://rbe.zdbjq.cn

Ruby: Dir.pwd
来源：http://mbv.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://xiw.zdbjq.cn

[M05] 设置退出码
来源：http://soi.nanxinkj.top

Py:   sys.exit(1)
来源：http://hfd.jinqigfzy.top

PHP:  exit(1);
来源：http://vba.uphjek.com

JS:   process.exit(1)
来源：http://tfu.yueranfly.top

TS:   process.exit(1)
来源：http://smo.sxryk.cn

Java: System.exit(1)
来源：http://vgv.yuxming.cn

Go:   os.Exit(1)
来源：http://smk.sjlbkw.cn

Ruby: exit 1
来源：http://lue.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wxs.gogol.net.cn

[M06] 向标准错误输出
来源：http://dpj.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://ahg.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cjn.vehdjk.com

JS:   console.error("err")
来源：http://kgg.sjlbkw.cn

TS:   console.error("err")
来源：http://unb.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://vgd.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jeh.mhx1999.top

Ruby: warn "err"
来源：http://pks.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://aqx.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://rww.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://vmf.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://axs.jyoumei.cn

JS:   require.main === module
来源：http://xjs.jinqigfzy.top

TS:   require.main === module
来源：http://vap.ivvv.top

Java: public static void main(String[] args)
来源：http://ryw.hammf.cn

Go:   func main()
来源：http://lkx.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fcw.smart0.xyz

C#:   static void Main(string[] args)
来源：http://lya.sweek.top

[M08] 获取系统与运行时信息
来源：http://fak.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://wkb.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://lxa.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://wrx.yj202588.top

TS:   process.platform;  process.version
来源：http://hxv.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ryx.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yoe.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hej.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hxb.hywenlv.cn

================================================================================
来源：http://amj.uphjek.com

N. 数据结构与算法
来源：http://vta.ywan-chungtsiang.top

================================================================================
来源：http://aca.yj20258.top

[N01] 二分查找（有序数组）
来源：http://poo.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://mic.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rwy.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ffn.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbb.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://bzg.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://igq.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mbo.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://svo.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://tpl.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://dhh.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kaz.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nfk.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qhi.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mwi.pycfn.com

Go:   slices.Sort(arr)
来源：http://bnl.316326.xyz

Ruby: arr.sort
来源：http://ojk.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ews.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://tqa.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rkz.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://twe.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rya.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmu.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://szy.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pbn.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lig.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mhr.ybcxt.top

[N04] 斐波那契数列
来源：http://cwq.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ntk.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bnw.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://olj.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aka.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbo.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ela.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wzr.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://imk.zhiwuduotai.top

[N05] 最大公约数
来源：http://tsr.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://oet.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xhr.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tyn.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dkl.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xhq.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uhi.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://uqh.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ism.zhengqikj.top

[N06] 判断回文字符串
来源：http://chk.zdbjq.cn

Py:   s == s[::-1]
来源：http://ylh.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://tee.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://dbq.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://wly.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tpk.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://euf.havefunace.top

Ruby: s == s.reverse
来源：http://pav.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nxi.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://rjn.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ulg.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ovs.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qap.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://tod.birdmap.top

Java: // 手写 HashMap
来源：http://uys.tarul.cn

Go:   // 手写 map[int]int
来源：http://ntz.jinqigufen.top

Ruby: // 手写 Hash
来源：http://pgs.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://ncd.shangyingyoupin.top

[N08] 生成全排列
来源：http://pgj.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://jms.zycfv.cn

PHP:  // 手写递归交换
来源：http://vdt.haohaochexian.top

JS:   // 手写回溯递归
来源：http://jcy.xylfe.cn

TS:   // 手写回溯递归
来源：http://mzs.tarul.cn

Java: // 手写回溯递归
来源：http://tzt.birdmap.top

Go:   // 手写回溯递归
来源：http://qgg.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://ntv.cdnleiting.top

C#:   // 手写回溯递归
来源：http://epf.zycfv.cn

[N09] 栈与队列
来源：http://wjd.zdqjudy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zui.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://toc.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ijt.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uab.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zya.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gsx.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hkm.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eor.smart0.xyz

[N10] 链表节点定义
来源：http://nvm.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://llj.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://cyp.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jcy.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://knw.pycfn.com

Java: class Node { int v; Node next; }
来源：http://rrz.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://fcf.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cmf.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://evo.c1oappe.top

[N11] 二叉树中序遍历
来源：http://loa.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mck.tanke756.top

PHP:  // 手写递归函数
来源：http://kgt.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eah.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzt.yanxiufei.cn

Java: // 手写递归
来源：http://ezh.vehdjk.com

Go:   // 手写递归
来源：http://gpr.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://olf.ehwqpu.com

C#:   // 手写递归
来源：http://cih.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://axx.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://udw.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rkl.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qaq.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gwf.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ygo.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ovs.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jzs.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cah.jqgfzy.top

================================================================================
来源：http://ooz.andypj.xyz

O. 并发与异步
来源：http://fzd.guowangkeji.top

================================================================================
来源：http://xyk.zycfv.cn

[O01] 启动一个线程
来源：http://vpy.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://byr.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hna.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zub.hysaishi.cn

TS:   // 同 JS
来源：http://oqs.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://zhu.yj202588.top

Go:   go f()
来源：http://otu.birdmap.top

Ruby: Thread.new { f }
来源：http://yrc.yonumen.top

C#:   Task.Run(() => F());
来源：http://swg.zdqjudy.top

[O02] 使用线程池
来源：http://rkm.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tpj.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fqm.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://kfe.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://gwg.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://brw.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mkb.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jkx.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cww.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://jqk.cheryme.top

Py:   with lock: shared += 1
来源：http://cfa.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://mpb.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://smj.zhengqikj.top

TS:   // 同 JS
来源：http://exc.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://hmt.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nbk.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aca.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://udc.daria6918.cn

[O04] 定义异步函数并等待
来源：http://tia.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://hpk.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yqc.bbcook.cn

JS:   async function f() { await g(); }
来源：http://hak.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lbk.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mwd.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jwl.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://zfe.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://rdc.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://qkt.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://fwm.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mrx.316326.xyz

JS:   await Promise.all(tasks)
来源：http://xqe.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://otg.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dvs.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vnm.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://xoy.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rer.zhoulong.xyz


<!-- 参考信息 -->