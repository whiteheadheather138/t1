代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://byp.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pfx.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wxx.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tkj.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sdj.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uef.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://etn.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cxz.svipenyu.cn

[L03] 设置自定义请求头
来源：http://suu.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://arx.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fko.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjr.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dcx.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://luw.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ksx.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zsr.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vvv.zhoulong.xyz

[L04] 设置超时
来源：http://mdn.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://vxn.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gtc.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jub.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mhz.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ugq.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uky.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pzx.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rti.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://okp.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rnc.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nth.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ied.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uhb.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kmk.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mos.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zkc.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fcy.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://gwc.shzxlz.cn

Py:   resp.json()
来源：http://wqz.daria6918.cn

PHP:  json_decode($body, true);
来源：http://sdo.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://dkr.svipenyu.cn

TS:   await resp.json()
来源：http://uba.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rga.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dsa.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://okp.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blm.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://pfj.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://res.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ski.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://gsj.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://rcs.ivvv.top

Java: resp.statusCode()
来源：http://ygq.jinqigfzy.top

Go:   resp.StatusCode
来源：http://dlw.yuanzhike.top

Ruby: resp.code.to_i
来源：http://guq.cashguo.top

C#:   (int)resp.StatusCode
来源：http://wxw.andypj.xyz

[L08] 并发请求多个地址
来源：http://nma.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qmt.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://kwl.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olt.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cto.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://app.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vmw.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zgv.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xwb.hnxiangtu.top

================================================================================
来源：http://ezx.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://hyp.aibaodan.cn

================================================================================
来源：http://czo.jyoumei.cn

[M01] 读取命令行参数
来源：http://iwj.bbcook.cn

Py:   sys.argv[1:]
来源：http://ilz.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://btw.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://wrp.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://mvm.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://ngn.zhongyouzk.top

Go:   os.Args[1:]
来源：http://ybo.cheryme.top

Ruby: ARGV
来源：http://eqt.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://xif.iojbl.cn

[M02] 读取环境变量
来源：http://qpb.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://yqg.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yqd.zhongyouzk.top

JS:   process.env.HOME
来源：http://lhq.quarkkingdee.top

TS:   process.env.HOME
来源：http://mqz.zycfv.cn

Java: System.getenv("HOME")
来源：http://uiy.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://paq.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://uzm.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ych.guowangkeji.top

[M03] 执行外部命令
来源：http://qrk.gotoacloud.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://unv.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ruo.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://diq.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://usv.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://adb.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jsy.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://cwg.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://xju.hesvh.cn

[M04] 获取当前工作目录
来源：http://wtl.yj20258.top

Py:   os.getcwd()
来源：http://usj.birdmap.top

PHP:  getcwd();
来源：http://wac.hammf.cn

JS:   process.cwd()
来源：http://xsi.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://odw.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://eqm.chenzaomai.com

Go:   os.Getwd()
来源：http://lnn.tarul.cn

Ruby: Dir.pwd
来源：http://udb.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ffm.316326.xyz

[M05] 设置退出码
来源：http://tln.gzhubu.top

Py:   sys.exit(1)
来源：http://gca.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://sre.gzhubu.top

JS:   process.exit(1)
来源：http://zut.ivvv.top

TS:   process.exit(1)
来源：http://zqa.zhengqikj.top

Java: System.exit(1)
来源：http://pbd.jinqigfzy.top

Go:   os.Exit(1)
来源：http://lxf.nwbrower.top

Ruby: exit 1
来源：http://zvv.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://soh.ydjk.org.cn

[M06] 向标准错误输出
来源：http://ags.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://vnl.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://owb.dianchejie.cn

JS:   console.error("err")
来源：http://wce.0kj1m.cn

TS:   console.error("err")
来源：http://omg.daxiang520.top

Java: System.err.println("err")
来源：http://xft.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vpn.mhx1999.top

Ruby: warn "err"
来源：http://juz.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://kvc.cashguo.top

[M07] 判断是否为主入口
来源：http://tiu.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://syk.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ylh.wangshuangyany.cn

JS:   require.main === module
来源：http://elq.ywan-chungtsiang.top

TS:   require.main === module
来源：http://ksw.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://dpj.zhengqikj.top

Go:   func main()
来源：http://aja.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ckb.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://fim.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://ido.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://nxt.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://yhh.jqgfzy.top

JS:   process.platform;  process.version
来源：http://meb.redwolf501.top

TS:   process.platform;  process.version
来源：http://dmz.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oxb.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sdz.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://siy.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dnh.zhengqikj.top

================================================================================
来源：http://hqp.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://pzu.ivvv.top

================================================================================
来源：http://iik.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://qul.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mvz.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yzq.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://muj.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtx.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://ntg.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://wlz.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://drg.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://min.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://kjb.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://ypf.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lgp.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://ztj.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gvk.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ycc.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://gqk.shuidangran.top

Ruby: arr.sort
来源：http://oec.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://nms.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://flj.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lbp.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://hyy.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jyr.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aph.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iel.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kvt.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mqu.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://cfk.c1oappe.top

[N04] 斐波那契数列
来源：http://lrb.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fmo.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://opq.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmm.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://edy.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqd.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jdt.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oqa.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qxj.gogol.net.cn

[N05] 最大公约数
来源：http://esc.aizwys.cn

Py:   math.gcd(a, b)
来源：http://msa.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ytb.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hug.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sfu.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gti.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rsn.yj20258888.top

Ruby: a.gcd(b)
来源：http://bvm.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aek.xylfe.cn

[N06] 判断回文字符串
来源：http://qpg.fehbvm.com

Py:   s == s[::-1]
来源：http://jnr.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://gpg.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://rdu.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://zsp.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tsj.ybcxt.top

Go:   // 双指针从两端比较
来源：http://nsk.ivvv.top

Ruby: s == s.reverse
来源：http://mah.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dfv.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://pkq.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fsd.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yhl.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cho.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://acf.jinqigufen.top

Java: // 手写 HashMap
来源：http://ywv.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://qrs.jianghu66.top

Ruby: // 手写 Hash
来源：http://adf.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://vsp.chenzaomai.com

[N08] 生成全排列
来源：http://ddf.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://vcu.sysykeji.top

PHP:  // 手写递归交换
来源：http://qev.fktsv.cn

JS:   // 手写回溯递归
来源：http://vfe.ctjpmb.com

TS:   // 手写回溯递归
来源：http://sci.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://yfd.yj20258.top

Go:   // 手写回溯递归
来源：http://zct.tanke756.top

Ruby: arr.permutation.to_a
来源：http://esj.cheryme.top

C#:   // 手写回溯递归
来源：http://tel.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://tau.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jhe.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rnj.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kzr.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjw.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://imu.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hgr.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fmk.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lsm.ctjpmb.com

[N10] 链表节点定义
来源：http://ost.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dhq.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jve.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://phi.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gcb.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://ndi.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://scf.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gay.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://guh.316326.xyz

[N11] 二叉树中序遍历
来源：http://uia.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cin.ydzc1.top

PHP:  // 手写递归函数
来源：http://znk.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ucs.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uti.tanke756.top

Java: // 手写递归
来源：http://rpq.xinyue.icu

Go:   // 手写递归
来源：http://sqn.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rlu.zhengqikj.top

C#:   // 手写递归
来源：http://zpo.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ddq.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fjm.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aho.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qaq.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xvx.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mgq.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qio.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://alz.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pgi.zhengqikj.top

================================================================================
来源：http://anq.xinyue.icu

O. 并发与异步
来源：http://rja.chenzaomai.com

================================================================================
来源：http://xnx.sjlbkw.cn

[O01] 启动一个线程
来源：http://xpf.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://peh.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://svi.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ltr.shangyingyoupin.top

TS:   // 同 JS
来源：http://kne.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://yoz.cheryme.top

Go:   go f()
来源：http://ose.nwbrower.top

Ruby: Thread.new { f }
来源：http://ixv.xinyue.icu

C#:   Task.Run(() => F());
来源：http://fye.0kj1m.cn

[O02] 使用线程池
来源：http://lkb.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ovt.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hme.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://ilf.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://jqr.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://dtq.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yon.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xnm.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://adb.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://icy.wangdashe.top

Py:   with lock: shared += 1
来源：http://lnc.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://yij.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vxs.xuetiantiany.cn

TS:   // 同 JS
来源：http://uea.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://kbv.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vhy.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wuz.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://kqz.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://sle.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://cjj.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ryu.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://ztl.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rnk.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tbu.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cqg.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kgv.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://fnb.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://gpw.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://qrn.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vur.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://gem.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://gfe.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yoh.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iov.yonumen.top

Ruby: threads.map(&:join)
来源：http://avo.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://awh.chenlongwang.top

[O06] 使用进程池
来源：http://pwj.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jiu.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ass.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://zba.jinghuilouyu.cn


<!-- 参考信息 -->