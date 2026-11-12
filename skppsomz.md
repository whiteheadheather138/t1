代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://mua.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xml.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bmc.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wtt.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fxo.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pxq.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wtu.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rwj.redwolf501.top

[L03] 设置自定义请求头
来源：http://tyo.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xrp.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pjn.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://utr.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ieh.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tdm.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ssq.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pgg.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://saw.daxiang520.top

[L04] 设置超时
来源：http://ilq.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://abc.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://umk.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qiv.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://phs.kuanghao11.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nmr.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fzq.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aqi.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pvn.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://vfg.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qqv.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://efu.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ymn.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://anr.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ioi.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bgd.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dyx.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zwb.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://nua.jqgfzy.top

Py:   resp.json()
来源：http://emv.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://ufr.hnqzz.top

JS:   await resp.json()
来源：http://ahq.yonumen.top

TS:   await resp.json()
来源：http://orl.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eim.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://trr.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://cyv.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://thd.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://jsa.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wmb.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gdw.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://gnw.birdmap.top

TS:   resp.ok;  resp.status
来源：http://mrc.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://fgk.hywenlv.cn

Go:   resp.StatusCode
来源：http://gnr.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://njq.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://dri.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://upu.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lzi.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://kks.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vuh.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjm.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://prh.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nvz.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ear.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ori.c1oappe.top

================================================================================
来源：http://oxb.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://dtc.0kj1m.cn

================================================================================
来源：http://xlg.pycfn.com

[M01] 读取命令行参数
来源：http://kog.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://zmq.yj20258888.top

PHP:  $argv;  $argc;
来源：http://vbc.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://ivi.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://lnv.yongpay.top

Java: args 数组（main 方法参数）
来源：http://eka.zhengqikj.top

Go:   os.Args[1:]
来源：http://raf.cdnleiting.top

Ruby: ARGV
来源：http://hfb.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://mln.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://wgs.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://ldz.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://csh.meibo888.top

JS:   process.env.HOME
来源：http://lpf.quarkkingdee.top

TS:   process.env.HOME
来源：http://mxh.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://zqa.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://smy.cashguo.top

Ruby: ENV["HOME"]
来源：http://xiu.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tin.xinyue.icu

[M03] 执行外部命令
来源：http://piq.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pjb.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://shi.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hfp.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://mug.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fgw.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gpg.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xhy.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://bqm.ivvv.top

[M04] 获取当前工作目录
来源：http://ver.yj20258888.top

Py:   os.getcwd()
来源：http://ebq.tian-w.cn

PHP:  getcwd();
来源：http://sbp.hnqzz.top

JS:   process.cwd()
来源：http://qfo.shangyingyoupin.top

TS:   process.cwd()
来源：http://kwv.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://rch.hnqzz.top

Go:   os.Getwd()
来源：http://dmi.zhijiandao.cn

Ruby: Dir.pwd
来源：http://kmg.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://lle.dashuyun.cn

[M05] 设置退出码
来源：http://xzx.svipenyu.cn

Py:   sys.exit(1)
来源：http://gkx.fktsv.cn

PHP:  exit(1);
来源：http://lrr.yanxiufei.cn

JS:   process.exit(1)
来源：http://rsh.zycfv.cn

TS:   process.exit(1)
来源：http://yko.chenjidiqi.icu

Java: System.exit(1)
来源：http://cxm.yj202588.top

Go:   os.Exit(1)
来源：http://akv.pengpengdd.cyou

Ruby: exit 1
来源：http://rfx.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bay.yj202588.top

[M06] 向标准错误输出
来源：http://ugg.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://hvf.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iex.jinqigufen.top

JS:   console.error("err")
来源：http://xus.yuxming.cn

TS:   console.error("err")
来源：http://zpz.xuanzx.com

Java: System.err.println("err")
来源：http://jnj.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tbl.cheryme.top

Ruby: warn "err"
来源：http://vmg.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://lkz.hammf.cn

[M07] 判断是否为主入口
来源：http://ggw.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://xla.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pda.cashguo.top

JS:   require.main === module
来源：http://aqq.shangyingyoupin.top

TS:   require.main === module
来源：http://bix.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://let.ybcxt.top

Go:   func main()
来源：http://pln.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hcu.nwbrower.top

C#:   static void Main(string[] args)
来源：http://apg.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://qrz.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://vrb.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://ymq.yvedp.cn

JS:   process.platform;  process.version
来源：http://ict.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://xbm.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pye.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://tuy.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ybv.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://viv.cdnleiting.top

================================================================================
来源：http://olm.yj20258.top

N. 数据结构与算法
来源：http://rsg.pycfn.com

================================================================================
来源：http://fbk.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://izu.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://cee.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ldg.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://itk.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wvp.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://dvv.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://oph.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nud.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nzo.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://mvp.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://usf.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ttm.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gux.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eyw.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfk.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://qbe.zhixingplan.top

Ruby: arr.sort
来源：http://ksv.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kkj.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://aqo.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://man.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://jqs.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uio.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pzk.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tkn.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lhg.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ann.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zhv.0kj1m.cn

[N04] 斐波那契数列
来源：http://fhv.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aqf.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vwc.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://beu.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cda.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qyr.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dol.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gbl.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vlf.shangyingyoupin.top

[N05] 最大公约数
来源：http://ksb.hnqzz.top

Py:   math.gcd(a, b)
来源：http://pav.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vew.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zbg.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dip.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lsy.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dqt.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://ihs.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wpc.hesvh.cn

[N06] 判断回文字符串
来源：http://glv.316326.xyz

Py:   s == s[::-1]
来源：http://hsa.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://tyl.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://ork.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://fpr.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://suz.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://tps.nwbrower.top

Ruby: s == s.reverse
来源：http://bgv.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tzj.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://gki.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qfa.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tkc.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yeb.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://hoj.yanxiufei.cn

Java: // 手写 HashMap
来源：http://lnb.yj20258888.top

Go:   // 手写 map[int]int
来源：http://qxc.tianlin.xyz

Ruby: // 手写 Hash
来源：http://llc.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://vqt.gogol.net.cn

[N08] 生成全排列
来源：http://fzj.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://epn.hfpthk.cn

PHP:  // 手写递归交换
来源：http://czw.ybcxt.top

JS:   // 手写回溯递归
来源：http://hpm.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://fuy.gzhubu.top

Java: // 手写回溯递归
来源：http://wgv.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://vhy.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://wns.havefunace.top

C#:   // 手写回溯递归
来源：http://lvy.zhengqikj.top

[N09] 栈与队列
来源：http://qgy.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://igu.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wms.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ajv.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yeg.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ksj.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wtf.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ddj.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nnn.jqgfzy.top

[N10] 链表节点定义
来源：http://fok.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ebp.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gzg.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cnc.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pnm.birdmap.top

Java: class Node { int v; Node next; }
来源：http://gtj.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://uei.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://itl.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://umu.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://aie.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kki.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://gtt.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rat.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://raq.xylfe.cn

Java: // 手写递归
来源：http://mlr.vehdjk.com

Go:   // 手写递归
来源：http://mvp.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gae.tanke756.top

C#:   // 手写递归
来源：http://chb.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dws.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wuf.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://agz.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbi.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xlt.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://utm.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jqw.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://utx.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dqd.nwbrower.top

================================================================================
来源：http://fot.yj20258888.top

O. 并发与异步
来源：http://iku.guannengcc.top

================================================================================
来源：http://inr.bbcook.cn

[O01] 启动一个线程
来源：http://dvx.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sgw.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gje.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://obc.smart0.xyz

TS:   // 同 JS
来源：http://izx.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://ehq.birdmap.top

Go:   go f()
来源：http://amy.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://iht.tarul.cn

C#:   Task.Run(() => F());
来源：http://faa.chenjidiqi.icu

[O02] 使用线程池
来源：http://jlq.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ilk.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gsh.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://bkd.ydzc1.top

TS:   // worker_threads 线程池
来源：http://eaw.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://qxl.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bcu.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rvm.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oyi.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://mfz.ybcxt.top

Py:   with lock: shared += 1
来源：http://vvy.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://hyl.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uyu.sysykeji.top

TS:   // 同 JS
来源：http://nhj.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://ebh.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xbh.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ckl.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://qoz.c1oappe.top

[O04] 定义异步函数并等待
来源：http://gwa.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://tam.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ixk.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://jrs.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gvq.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vzc.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ara.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://rof.cheryme.top

C#:   async Task F() { await G(); }
来源：http://jlt.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://hzq.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://tba.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gbj.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://rnw.yj20258.top

TS:   await Promise.all(tasks)
来源：http://wfc.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oqi.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uxp.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://nib.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vbu.birdmap.top

[O06] 使用进程池
来源：http://pci.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://soy.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://rke.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://qon.mhx1999.top


<!-- 参考信息 -->