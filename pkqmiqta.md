代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://vho.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dlu.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ygs.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bie.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hic.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gwr.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ujc.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jkr.xinyue.icu

[L03] 设置自定义请求头
来源：http://idk.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sey.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bkk.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncg.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tuu.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rxv.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://grh.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://owd.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xgc.zhijiandao.cn

[L04] 设置超时
来源：http://qzl.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://lue.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qqi.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yzo.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iso.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tkj.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gro.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qwg.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zeq.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://syp.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://onl.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cng.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://brr.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bpm.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rrd.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://liz.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://glw.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cfr.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://age.dashuyun.cn

Py:   resp.json()
来源：http://ify.bbcook.cn

PHP:  json_decode($body, true);
来源：http://hlj.daria6918.cn

JS:   await resp.json()
来源：http://bce.jlsjyb.cn

TS:   await resp.json()
来源：http://brj.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bxc.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wzd.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://zkq.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://weq.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://eac.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gye.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dlu.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://axl.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://pmz.wangdashe.top

Java: resp.statusCode()
来源：http://prm.yongpay.top

Go:   resp.StatusCode
来源：http://pmw.bjfxy.top

Ruby: resp.code.to_i
来源：http://wgt.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://qse.yongpay.top

[L08] 并发请求多个地址
来源：http://ilw.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uqv.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://jrq.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfc.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwf.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://urv.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nww.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wkz.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nce.sxryk.cn

================================================================================
来源：http://rim.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://skg.hywenlv.cn

================================================================================
来源：http://xxr.sjlbkw.cn

[M01] 读取命令行参数
来源：http://qzk.vehdjk.com

Py:   sys.argv[1:]
来源：http://pzk.guannengcc.top

PHP:  $argv;  $argc;
来源：http://qwq.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://omy.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://kks.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://ofn.aizwys.cn

Go:   os.Args[1:]
来源：http://tpi.shanyushiyangkeji.top

Ruby: ARGV
来源：http://lzv.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://zxx.cheryme.top

[M02] 读取环境变量
来源：http://zat.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://srf.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yco.hcnkem.com

JS:   process.env.HOME
来源：http://wxv.andypj.xyz

TS:   process.env.HOME
来源：http://qmv.jyoumei.cn

Java: System.getenv("HOME")
来源：http://hmb.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dgr.xinyue.icu

Ruby: ENV["HOME"]
来源：http://zqx.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obj.redwolf501.top

[M03] 执行外部命令
来源：http://oki.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jas.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jts.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kzy.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tzu.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cds.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dtp.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://ckw.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://mgg.shuidangran.top

[M04] 获取当前工作目录
来源：http://vjr.yongpay.top

Py:   os.getcwd()
来源：http://gnd.zhengqikj.top

PHP:  getcwd();
来源：http://yoh.jianghu66.top

JS:   process.cwd()
来源：http://dak.cdnleiting.top

TS:   process.cwd()
来源：http://knf.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://ecx.chenlongwang.top

Go:   os.Getwd()
来源：http://ker.zhongyouzk.top

Ruby: Dir.pwd
来源：http://xff.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://mta.hywenlv.cn

[M05] 设置退出码
来源：http://iyn.yuanzhike.top

Py:   sys.exit(1)
来源：http://ovf.gogol.net.cn

PHP:  exit(1);
来源：http://olg.xuanzx.com

JS:   process.exit(1)
来源：http://ibp.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://iai.dianchejie.cn

Java: System.exit(1)
来源：http://vlr.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://shr.yongpay.top

Ruby: exit 1
来源：http://amb.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ybn.jqgfzy.top

[M06] 向标准错误输出
来源：http://xqm.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://plc.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://rln.jinqigufen.top

JS:   console.error("err")
来源：http://szw.xuanzx.com

TS:   console.error("err")
来源：http://cdo.52xcode.cn

Java: System.err.println("err")
来源：http://xtk.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://inr.bbcook.cn

Ruby: warn "err"
来源：http://jwl.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://mai.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://pvu.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://fdq.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cyl.sxryk.cn

JS:   require.main === module
来源：http://zor.cdnleiting.top

TS:   require.main === module
来源：http://qoa.bbcook.cn

Java: public static void main(String[] args)
来源：http://jlq.sjlbkw.cn

Go:   func main()
来源：http://fcx.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jle.ybcxt.top

C#:   static void Main(string[] args)
来源：http://wwu.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://tmj.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://zvv.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://epm.dianchejie.cn

JS:   process.platform;  process.version
来源：http://cby.fehbvm.com

TS:   process.platform;  process.version
来源：http://evk.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bke.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lpk.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iha.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wue.snrcjt.cn

================================================================================
来源：http://fhq.ybcxt.top

N. 数据结构与算法
来源：http://oqg.jianghu66.top

================================================================================
来源：http://tnr.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://zjw.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pel.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://piy.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kqq.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rit.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vwq.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://wry.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://wgf.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://ydp.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://qrf.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ton.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tgv.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://egb.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pwg.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ckx.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://rhw.zhengqikj.top

Ruby: arr.sort
来源：http://ooj.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tpz.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://cru.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://spo.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://avb.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://owz.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfl.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ziv.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jxk.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fmj.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://drs.cdnleiting.top

[N04] 斐波那契数列
来源：http://iyx.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jax.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bon.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyl.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mrz.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mdg.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lkv.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tul.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kod.zhijiandao.cn

[N05] 最大公约数
来源：http://bgd.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://rga.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bge.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gzp.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wpk.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xoh.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cjz.zhengqikj.top

Ruby: a.gcd(b)
来源：http://pws.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jwq.yueranfly.top

[N06] 判断回文字符串
来源：http://wpi.hcnkem.com

Py:   s == s[::-1]
来源：http://xqz.mhx1999.top

PHP:  $s === strrev($s);
来源：http://tii.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://jaf.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://abj.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tpw.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://qht.gzhubu.top

Ruby: s == s.reverse
来源：http://pvj.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ebg.uphjek.com

[N07] 两数之和（返回下标）
来源：http://ouz.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cru.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zoi.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pel.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://rxn.smart0.xyz

Java: // 手写 HashMap
来源：http://imr.aizwys.cn

Go:   // 手写 map[int]int
来源：http://kdu.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://bij.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rth.mhx1999.top

[N08] 生成全排列
来源：http://pnb.yongpay.top

Py:   itertools.permutations(arr)
来源：http://dlf.yangfankeji.com

PHP:  // 手写递归交换
来源：http://ptv.tarul.cn

JS:   // 手写回溯递归
来源：http://lje.tian-w.cn

TS:   // 手写回溯递归
来源：http://arj.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://mdn.cheryme.top

Go:   // 手写回溯递归
来源：http://qbl.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://kod.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://num.tanke756.top

[N09] 栈与队列
来源：http://dkh.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vww.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://exr.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wsd.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fue.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ifd.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpp.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ngl.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kzx.andypj.xyz

[N10] 链表节点定义
来源：http://vkw.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://unt.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ndu.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wxo.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ebo.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://jyn.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pwh.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qte.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://erp.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://tgp.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vev.smart0.xyz

PHP:  // 手写递归函数
来源：http://jcm.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfs.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ljj.xinyue.icu

Java: // 手写递归
来源：http://toy.vehdjk.com

Go:   // 手写递归
来源：http://xxv.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fek.xuetiantiany.cn

C#:   // 手写递归
来源：http://kqe.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ikj.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nrz.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oxf.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqa.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovw.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zvy.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eei.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dyd.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://loq.jyoumei.cn

================================================================================
来源：http://frh.ivvv.top

O. 并发与异步
来源：http://ula.pycfn.com

================================================================================
来源：http://wlb.yvedp.cn

[O01] 启动一个线程
来源：http://brl.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hom.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sid.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://czn.zycfv.cn

TS:   // 同 JS
来源：http://ahg.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://tft.kuanghao11.cn

Go:   go f()
来源：http://vxa.ydzc1.top

Ruby: Thread.new { f }
来源：http://xns.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://myp.bjfxy.top

[O02] 使用线程池
来源：http://aie.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qdt.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sbg.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://wxe.havefunace.top

TS:   // worker_threads 线程池
来源：http://gmd.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://zqq.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nui.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qsc.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://czw.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://vxg.yuxming.cn

Py:   with lock: shared += 1
来源：http://bvv.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://amf.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pdv.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://smw.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://ash.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fop.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gyc.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://nir.zhengqikj.top

[O04] 定义异步函数并等待
来源：http://xxg.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://pxj.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bwl.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://ckg.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dtc.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bvx.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aug.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nnk.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://gts.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://djs.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://eyp.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wch.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://axe.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://nqr.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qqv.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://liy.andypj.xyz

Ruby: threads.map(&:join)
来源：http://kmp.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ahu.redwolf501.top

[O06] 使用进程池
来源：http://gwi.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ybf.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ziu.birdmap.top

JS:   // child_process / cluster 模块
来源：http://qtf.yj202588.top


<!-- 参考信息 -->