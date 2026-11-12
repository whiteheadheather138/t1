代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://fyb.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zpy.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usu.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bag.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kwx.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kcn.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fnk.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ejq.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://ypj.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aqm.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xni.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hph.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://guc.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxj.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rjw.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jsp.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hya.xuanzx.com

[L04] 设置超时
来源：http://qjj.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://ody.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://irg.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tpn.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mrn.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yzq.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pes.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oqe.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oif.redwolf501.top

[L05] 上传文件（multipart）
来源：http://icv.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jtj.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pwx.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lqm.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ccm.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rym.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fhs.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oht.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gbf.hnqzz.top

[L06] 解析响应为 JSON
来源：http://yan.andypj.xyz

Py:   resp.json()
来源：http://mdl.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://jao.snrcjt.cn

JS:   await resp.json()
来源：http://bjf.ctjpmb.com

TS:   await resp.json()
来源：http://ozt.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://scs.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kxw.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://mqi.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jyt.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://yke.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ttp.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://izj.tanke756.top

JS:   resp.ok;  resp.status
来源：http://jms.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://idx.bjfxy.top

Java: resp.statusCode()
来源：http://iga.cucudq.cn

Go:   resp.StatusCode
来源：http://vla.redwolf501.top

Ruby: resp.code.to_i
来源：http://tzw.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://ola.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://czz.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rcb.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://rdx.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dpg.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iiu.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qvr.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hvl.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://byo.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pyx.guowangkeji.top

================================================================================
来源：http://ikk.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://lap.tian-w.cn

================================================================================
来源：http://xmb.cqqwz.cn

[M01] 读取命令行参数
来源：http://xds.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://tmy.yfazqb.com

PHP:  $argv;  $argc;
来源：http://rfi.cheryme.top

JS:   process.argv.slice(2)
来源：http://aya.cucudq.cn

TS:   process.argv.slice(2)
来源：http://xss.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://kjv.guannengcc.top

Go:   os.Args[1:]
来源：http://xid.daxiang520.top

Ruby: ARGV
来源：http://fgx.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://jhe.yuanzhike.top

[M02] 读取环境变量
来源：http://ezd.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://qfo.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iph.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://sdw.316326.xyz

TS:   process.env.HOME
来源：http://uvm.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://pib.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tqq.sysykeji.top

Ruby: ENV["HOME"]
来源：http://aza.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pfc.sjlbkw.cn

[M03] 执行外部命令
来源：http://abe.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vbz.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zwi.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://baq.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://skk.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yul.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qbs.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://urv.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://bab.yuanzhike.top

[M04] 获取当前工作目录
来源：http://vnf.shuidangran.top

Py:   os.getcwd()
来源：http://tuc.iojbl.cn

PHP:  getcwd();
来源：http://fls.cashguo.top

JS:   process.cwd()
来源：http://kcn.epnwcf.com

TS:   process.cwd()
来源：http://bfv.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://qeu.nanxinkj.top

Go:   os.Getwd()
来源：http://pcu.zhengqikj.top

Ruby: Dir.pwd
来源：http://ypr.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://unx.fktsv.cn

[M05] 设置退出码
来源：http://nsw.tianlin.xyz

Py:   sys.exit(1)
来源：http://okl.uphjek.com

PHP:  exit(1);
来源：http://efc.tian-w.cn

JS:   process.exit(1)
来源：http://yvl.bjfxy.top

TS:   process.exit(1)
来源：http://tnd.yangfankeji.com

Java: System.exit(1)
来源：http://tfc.ybcxt.top

Go:   os.Exit(1)
来源：http://ifk.fehbvm.com

Ruby: exit 1
来源：http://ypu.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cni.jianghu66.top

[M06] 向标准错误输出
来源：http://kjl.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://yek.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ksj.jianghu66.top

JS:   console.error("err")
来源：http://you.hcnkem.com

TS:   console.error("err")
来源：http://sta.nanxinkj.top

Java: System.err.println("err")
来源：http://nse.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fhg.dashuyun.cn

Ruby: warn "err"
来源：http://gnw.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://vni.aibaodan.cn

[M07] 判断是否为主入口
来源：http://xuy.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://vqb.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://knr.sjlbkw.cn

JS:   require.main === module
来源：http://kou.9152youxi.cn

TS:   require.main === module
来源：http://wkz.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://lho.sysykeji.top

Go:   func main()
来源：http://dja.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fvo.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://nkz.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://zci.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://nbf.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://ctt.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://lya.pycfn.com

TS:   process.platform;  process.version
来源：http://hti.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lcw.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ftl.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpc.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://egj.zhiwuduotai.top

================================================================================
来源：http://tvi.sysykeji.top

N. 数据结构与算法
来源：http://nfe.yangfankeji.com

================================================================================
来源：http://leq.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://mmm.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rve.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gkr.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sml.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vkb.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://djy.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://qjr.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cod.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://rno.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://wix.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://lub.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bwr.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ums.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ywj.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ylx.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://yym.daria6918.cn

Ruby: arr.sort
来源：http://wbd.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hlt.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://kbg.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rmp.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://cfi.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://slf.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qcx.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://srk.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uoo.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yrc.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vve.hesvh.cn

[N04] 斐波那契数列
来源：http://biy.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ljq.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rkl.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dnx.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qmh.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qlz.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://edn.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nmv.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bry.daxiang520.top

[N05] 最大公约数
来源：http://yud.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://yhu.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yhj.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wxi.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zeh.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czd.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://obg.svipenyu.cn

Ruby: a.gcd(b)
来源：http://wqf.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lbe.pycfn.com

[N06] 判断回文字符串
来源：http://ggq.nwbrower.top

Py:   s == s[::-1]
来源：http://ofo.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://mlq.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://dwe.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://rji.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tfm.zycfv.cn

Go:   // 双指针从两端比较
来源：http://qxd.jinqigufen.top

Ruby: s == s.reverse
来源：http://vnx.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ilb.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://lls.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vka.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://acj.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mio.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://xpl.kuanghao11.cn

Java: // 手写 HashMap
来源：http://mmt.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://vbg.cdnleiting.top

Ruby: // 手写 Hash
来源：http://ttn.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://bym.epnwcf.com

[N08] 生成全排列
来源：http://kst.tarul.cn

Py:   itertools.permutations(arr)
来源：http://fau.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://nyc.nanxinkj.top

JS:   // 手写回溯递归
来源：http://myf.guannengcc.top

TS:   // 手写回溯递归
来源：http://zgv.yj20258.top

Java: // 手写回溯递归
来源：http://gqe.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://stu.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://wiw.yj20258888.top

C#:   // 手写回溯递归
来源：http://otr.sxryk.cn

[N09] 栈与队列
来源：http://ifl.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qpu.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ynh.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jxh.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://avn.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gew.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jwb.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hqh.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdi.jlsjyb.cn

[N10] 链表节点定义
来源：http://rgh.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rat.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mra.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mcc.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zdf.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://gys.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://nzf.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rjc.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://psb.bbcook.cn

[N11] 二叉树中序遍历
来源：http://bpj.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://chq.cqqwz.cn

PHP:  // 手写递归函数
来源：http://pbt.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://smk.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czs.nanxuanxn.top

Java: // 手写递归
来源：http://xbw.ydjk.org.cn

Go:   // 手写递归
来源：http://evh.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fvd.kuanghao11.cn

C#:   // 手写递归
来源：http://gyu.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gdb.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ofc.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gas.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vcy.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ouv.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oeu.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xxd.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ybg.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tor.shanyushiyangkeji.top

================================================================================
来源：http://ang.tanke756.top

O. 并发与异步
来源：http://zlw.ctjpmb.com

================================================================================
来源：http://spa.zycfv.cn

[O01] 启动一个线程
来源：http://nrn.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oxh.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tup.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oqe.guowangkeji.top

TS:   // 同 JS
来源：http://zss.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://ibj.fktsv.cn

Go:   go f()
来源：http://jpm.316326.xyz

Ruby: Thread.new { f }
来源：http://ixb.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://sjb.sufxvd.cn

[O02] 使用线程池
来源：http://eaj.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cqd.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kel.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://gxa.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://lat.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dhr.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fmo.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kqy.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hqz.bjfxy.top

[O03] 加锁保护共享数据
来源：http://rme.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://nig.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://btv.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iat.uphjek.com

TS:   // 同 JS
来源：http://thc.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://lrf.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qxx.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tqu.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://upz.vehdjk.com

[O04] 定义异步函数并等待
来源：http://frt.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://ybk.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xcp.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://djl.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://mem.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ekh.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ivl.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://qsw.meibo888.top

C#:   async Task F() { await G(); }
来源：http://tkg.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://dpy.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://emq.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aqz.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://dpf.meibo888.top

TS:   await Promise.all(tasks)
来源：http://rjf.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ltc.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iuq.meibo888.top

Ruby: threads.map(&:join)
来源：http://kav.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tbl.jiagoushi.top

[O06] 使用进程池
来源：http://umj.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wew.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://sqr.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://qiw.tarul.cn


<!-- 参考信息 -->