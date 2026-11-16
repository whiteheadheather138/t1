代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://sbr.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vng.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cau.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vti.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tej.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://njt.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vmd.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dep.sysykeji.top

[L03] 设置自定义请求头
来源：http://ljf.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qac.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qqo.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvs.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzp.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://flh.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hkt.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://een.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dln.tianlin.xyz

[L04] 设置超时
来源：http://ysg.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://txm.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cgy.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvj.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vyu.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ipd.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pyo.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://doc.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xzv.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://uhl.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zzm.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qvk.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eac.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pqc.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wek.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pxf.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ihm.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uiu.hcnkem.com

[L06] 解析响应为 JSON
来源：http://tjw.yj20258888.top

Py:   resp.json()
来源：http://skh.xziqi.cn

PHP:  json_decode($body, true);
来源：http://ogm.hnxiangtu.top

JS:   await resp.json()
来源：http://hof.epnwcf.com

TS:   await resp.json()
来源：http://eln.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xph.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bcz.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://kae.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uhl.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://bqu.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dmc.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxb.yj20258.top

JS:   resp.ok;  resp.status
来源：http://pja.cheryme.top

TS:   resp.ok;  resp.status
来源：http://vnm.cqqwz.cn

Java: resp.statusCode()
来源：http://nae.fktsv.cn

Go:   resp.StatusCode
来源：http://dua.cucudq.cn

Ruby: resp.code.to_i
来源：http://bge.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://vso.cqqwz.cn

[L08] 并发请求多个地址
来源：http://bmn.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ulk.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://itx.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sui.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://drm.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dmy.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hcf.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lbb.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nta.epnwcf.com

================================================================================
来源：http://fqa.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://enp.yanxiufei.cn

================================================================================
来源：http://dll.yueranfly.top

[M01] 读取命令行参数
来源：http://cpg.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://pru.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://bzx.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://glg.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://ope.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://sfn.meibo888.top

Go:   os.Args[1:]
来源：http://hqv.andypj.xyz

Ruby: ARGV
来源：http://gll.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://ojl.daxiang520.top

[M02] 读取环境变量
来源：http://psa.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://ykr.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://heu.jinqigufen.top

JS:   process.env.HOME
来源：http://xib.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://zdc.iojbl.cn

Java: System.getenv("HOME")
来源：http://ptc.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bqa.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://aeh.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://and.birdmap.top

[M03] 执行外部命令
来源：http://pgt.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cwt.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rxi.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ajh.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://wln.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cdy.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://coo.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://yhy.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://jer.andypj.xyz

[M04] 获取当前工作目录
来源：http://bnl.xziqi.cn

Py:   os.getcwd()
来源：http://yki.pycfn.com

PHP:  getcwd();
来源：http://frf.bbcook.cn

JS:   process.cwd()
来源：http://ryo.hfpthk.cn

TS:   process.cwd()
来源：http://gka.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://cpl.sysykeji.top

Go:   os.Getwd()
来源：http://qoo.yongpay.top

Ruby: Dir.pwd
来源：http://oxt.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ylu.zhiwuduotai.top

[M05] 设置退出码
来源：http://gbg.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://oaq.yj20258.top

PHP:  exit(1);
来源：http://uou.ybcxt.top

JS:   process.exit(1)
来源：http://krq.iojbl.cn

TS:   process.exit(1)
来源：http://yko.redwolf501.top

Java: System.exit(1)
来源：http://ntg.jqgfzy.top

Go:   os.Exit(1)
来源：http://vka.haohaochexian.top

Ruby: exit 1
来源：http://msr.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eeq.zhongyouzk.top

[M06] 向标准错误输出
来源：http://vyj.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://thn.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xkg.fengsongda.top

JS:   console.error("err")
来源：http://tlk.jqgufenzy.top

TS:   console.error("err")
来源：http://oyp.gzhubu.top

Java: System.err.println("err")
来源：http://iqi.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jvc.yanxiufei.cn

Ruby: warn "err"
来源：http://avl.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://mqw.zhengqikj.top

[M07] 判断是否为主入口
来源：http://yjq.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://uek.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://feh.wangdashe.top

JS:   require.main === module
来源：http://goz.chenzaomai.com

TS:   require.main === module
来源：http://ytk.chenzaomai.com

Java: public static void main(String[] args)
来源：http://vks.nanxuanxn.top

Go:   func main()
来源：http://ymp.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ums.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://egx.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://fko.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://kmz.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://tkn.pycfn.com

JS:   process.platform;  process.version
来源：http://rfz.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://auz.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xkr.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mpd.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://caa.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgk.yj202588.top

================================================================================
来源：http://xkr.ctjpmb.com

N. 数据结构与算法
来源：http://qkz.zhixingplan.top

================================================================================
来源：http://hsw.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://eja.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://haq.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sso.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fil.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rhf.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://prh.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://ytn.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nzg.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://ovq.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://qvq.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://wyk.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://asn.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oax.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mex.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lyb.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://aus.9152youxi.cn

Ruby: arr.sort
来源：http://znt.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ity.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://rvd.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpf.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://ono.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyz.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ftv.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kud.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ojo.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://npr.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mko.ehwqpu.com

[N04] 斐波那契数列
来源：http://xox.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dhj.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rkg.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://edp.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pul.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hch.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xay.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mbe.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rce.hongshengwenyu.top

[N05] 最大公约数
来源：http://eoe.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://nxs.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oeh.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edw.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qhs.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xih.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uza.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://uyt.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zjm.zycfv.cn

[N06] 判断回文字符串
来源：http://wtm.xylfe.cn

Py:   s == s[::-1]
来源：http://qev.ybcxt.top

PHP:  $s === strrev($s);
来源：http://rip.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://svm.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://xww.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bie.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://rod.gzhubu.top

Ruby: s == s.reverse
来源：http://jmj.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dgj.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://ufg.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jpg.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lqy.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cao.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://bwa.gogol.net.cn

Java: // 手写 HashMap
来源：http://bmw.sweek.top

Go:   // 手写 map[int]int
来源：http://del.hfpthk.cn

Ruby: // 手写 Hash
来源：http://gzm.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://pzn.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://ttu.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://mdg.jianghu66.top

PHP:  // 手写递归交换
来源：http://bgf.shuidangran.top

JS:   // 手写回溯递归
来源：http://ldk.tarul.cn

TS:   // 手写回溯递归
来源：http://uao.fengsongda.top

Java: // 手写回溯递归
来源：http://icz.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://inw.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://noe.316326.xyz

C#:   // 手写回溯递归
来源：http://mym.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://rws.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aoy.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cqu.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kin.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kek.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbu.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pwb.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kxt.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rtr.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://fkr.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tjw.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zla.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qxa.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pzd.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://ver.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://utc.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://cnu.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rwm.yuxming.cn

[N11] 二叉树中序遍历
来源：http://cxp.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qel.jianghu66.top

PHP:  // 手写递归函数
来源：http://aal.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edu.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpk.9152youxi.cn

Java: // 手写递归
来源：http://cpu.shzxlz.cn

Go:   // 手写递归
来源：http://chs.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iym.fengsongda.top

C#:   // 手写递归
来源：http://bnh.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xvd.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://duo.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nwn.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mnt.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://unb.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://doj.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tpr.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mdp.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://log.yfazqb.com

================================================================================
来源：http://vdm.yvedp.cn

O. 并发与异步
来源：http://wai.yvedp.cn

================================================================================
来源：http://gkk.yj20258888.top

[O01] 启动一个线程
来源：http://cbb.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://plm.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://asc.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nui.haohaochexian.top

TS:   // 同 JS
来源：http://vqs.sweek.top

Java: new Thread(() -> f()).start()
来源：http://nlp.jianghu66.top

Go:   go f()
来源：http://ctg.nanxinkj.top

Ruby: Thread.new { f }
来源：http://bfr.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://rdi.tanke756.top

[O02] 使用线程池
来源：http://skz.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dvq.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aby.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://vzn.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://yjx.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://jxn.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wxa.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://urw.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vhz.mhx1999.top

[O03] 加锁保护共享数据
来源：http://xlw.mhx1999.top

Py:   with lock: shared += 1
来源：http://ojo.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://cle.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://drb.316326.xyz

TS:   // 同 JS
来源：http://bdk.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://xto.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ycs.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ino.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://rny.uphjek.com

[O04] 定义异步函数并等待
来源：http://eko.meibo888.top

Py:   async def f():⏎    await g()
来源：http://kpp.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wso.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://nqj.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://bru.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://spo.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gxp.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://avx.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://jdg.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://tkh.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://ohi.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nte.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://nlq.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://xhm.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rhv.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ymj.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://nqt.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rrh.jiagoushi.top

[O06] 使用进程池
来源：http://apc.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oxn.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://txe.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://mqp.yj20258.top


<!-- 参考信息 -->