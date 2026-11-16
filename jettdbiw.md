代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hzu.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uik.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ouk.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xwy.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gxx.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xkp.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cje.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ogm.ydzc1.top

[L03] 设置自定义请求头
来源：http://iow.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dan.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aje.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sbb.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://axg.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cvz.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mgw.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jzx.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ofw.gotoacloud.top

[L04] 设置超时
来源：http://vdq.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://lmg.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mst.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjs.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejv.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fxu.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qlc.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cao.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqk.bbcook.cn

[L05] 上传文件（multipart）
来源：http://nbr.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vus.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jta.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://njo.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lhh.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tpl.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pwl.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nro.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yzm.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://jid.jinqigfzy.top

Py:   resp.json()
来源：http://gmd.yj20258.top

PHP:  json_decode($body, true);
来源：http://dui.yj202588.top

JS:   await resp.json()
来源：http://vjy.svipenyu.cn

TS:   await resp.json()
来源：http://kkx.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sip.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://koq.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://hki.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wro.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://grq.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vzc.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kow.sweek.top

JS:   resp.ok;  resp.status
来源：http://dlw.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://xuh.316326.xyz

Java: resp.statusCode()
来源：http://ljp.kuanghao11.cn

Go:   resp.StatusCode
来源：http://cks.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://aei.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://xel.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://neu.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nhw.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://pgc.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mel.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smx.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mkz.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rvs.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://der.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ptx.fengsongda.top

================================================================================
来源：http://iyk.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://yaj.chenlongwang.top

================================================================================
来源：http://njg.gogol.net.cn

[M01] 读取命令行参数
来源：http://spm.hywenlv.cn

Py:   sys.argv[1:]
来源：http://mzu.aizwys.cn

PHP:  $argv;  $argc;
来源：http://xql.yuxming.cn

JS:   process.argv.slice(2)
来源：http://cky.cucudq.cn

TS:   process.argv.slice(2)
来源：http://crn.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://qff.daxiang520.top

Go:   os.Args[1:]
来源：http://bbi.havefunace.top

Ruby: ARGV
来源：http://cub.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://epx.hysaishi.cn

[M02] 读取环境变量
来源：http://thx.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://eeh.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cbb.andypj.xyz

JS:   process.env.HOME
来源：http://yno.ydjk.org.cn

TS:   process.env.HOME
来源：http://drb.yfazqb.com

Java: System.getenv("HOME")
来源：http://hfz.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mdr.yfazqb.com

Ruby: ENV["HOME"]
来源：http://gne.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cwl.aizwys.cn

[M03] 执行外部命令
来源：http://iqx.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tty.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tzt.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uyy.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wse.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://isc.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aly.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cvd.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://dqt.havefunace.top

[M04] 获取当前工作目录
来源：http://ubc.xuetiantiany.cn

Py:   os.getcwd()
来源：http://xpc.ctjpmb.com

PHP:  getcwd();
来源：http://ogg.jianghu66.top

JS:   process.cwd()
来源：http://edb.yvedp.cn

TS:   process.cwd()
来源：http://lwj.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://mpl.ctjpmb.com

Go:   os.Getwd()
来源：http://oil.cqqwz.cn

Ruby: Dir.pwd
来源：http://fgx.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xwd.guannengcc.top

[M05] 设置退出码
来源：http://qal.tarul.cn

Py:   sys.exit(1)
来源：http://ywc.sufxvd.cn

PHP:  exit(1);
来源：http://ciq.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://mfa.52xcode.cn

TS:   process.exit(1)
来源：http://kta.zdbjq.cn

Java: System.exit(1)
来源：http://tad.jiagoushi.top

Go:   os.Exit(1)
来源：http://rxa.ivvv.top

Ruby: exit 1
来源：http://vhh.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zjv.hnqzz.top

[M06] 向标准错误输出
来源：http://sym.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://stz.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sjo.aizwys.cn

JS:   console.error("err")
来源：http://ocf.c1oappe.top

TS:   console.error("err")
来源：http://dyc.haohaochexian.top

Java: System.err.println("err")
来源：http://pxa.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://abz.jinghuilouyu.cn

Ruby: warn "err"
来源：http://lci.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://dzg.andypj.xyz

[M07] 判断是否为主入口
来源：http://avb.yonumen.top

Py:   if __name__ == "__main__":
来源：http://tlp.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jcp.svipenyu.cn

JS:   require.main === module
来源：http://ult.zhixingplan.top

TS:   require.main === module
来源：http://bad.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://dng.zhongyouzk.top

Go:   func main()
来源：http://qcv.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://opi.yonumen.top

C#:   static void Main(string[] args)
来源：http://ylh.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://gpx.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://xdf.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://fhs.ehwqpu.com

JS:   process.platform;  process.version
来源：http://nuw.yangfankeji.com

TS:   process.platform;  process.version
来源：http://lqq.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yut.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://gat.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rzc.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ywn.bbcook.cn

================================================================================
来源：http://itp.jyoumei.cn

N. 数据结构与算法
来源：http://uik.tianlin.xyz

================================================================================
来源：http://glz.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://amz.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://glt.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rbm.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ykw.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kvf.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://fnb.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://six.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fwf.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://sfa.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://oce.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://bmu.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yat.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vug.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://nfu.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://err.andypj.xyz

Go:   slices.Sort(arr)
来源：http://gdm.9152youxi.cn

Ruby: arr.sort
来源：http://cdi.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://omi.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://ljo.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bbv.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://qdl.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bud.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdw.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bpm.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ejf.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uud.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jar.ybcxt.top

[N04] 斐波那契数列
来源：http://utk.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uhc.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://byc.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wnb.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gfx.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qqw.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wfe.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zaf.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rnv.jinqigufen.top

[N05] 最大公约数
来源：http://wai.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://fec.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ujt.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asz.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://voq.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qdd.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lyc.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://vmw.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gyz.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://lgf.hcnkem.com

Py:   s == s[::-1]
来源：http://pfi.yonumen.top

PHP:  $s === strrev($s);
来源：http://hga.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://dqb.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://rqp.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dsj.guannengcc.top

Go:   // 双指针从两端比较
来源：http://jxg.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://pyk.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jgs.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://jhv.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wjd.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oic.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nrp.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://uyh.zhixingplan.top

Java: // 手写 HashMap
来源：http://zdi.sxryk.cn

Go:   // 手写 map[int]int
来源：http://ihs.yj20258888.top

Ruby: // 手写 Hash
来源：http://zig.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zpz.xylfe.cn

[N08] 生成全排列
来源：http://spu.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://fls.daxiang520.top

PHP:  // 手写递归交换
来源：http://ceo.ybcxt.top

JS:   // 手写回溯递归
来源：http://uit.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://yac.ydzc1.top

Java: // 手写回溯递归
来源：http://ehr.birdmap.top

Go:   // 手写回溯递归
来源：http://bvf.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://qjj.aizwys.cn

C#:   // 手写回溯递归
来源：http://eke.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://hlx.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uxz.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://osd.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ooo.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tad.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://raf.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ubu.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tla.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ipw.yangfankeji.com

[N10] 链表节点定义
来源：http://jic.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tbr.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qic.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mti.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://haf.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://txy.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://pgf.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qaq.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tsn.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://dpt.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://edx.nwbrower.top

PHP:  // 手写递归函数
来源：http://lpj.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zge.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yin.yanxiufei.cn

Java: // 手写递归
来源：http://eal.ppjwa.cn

Go:   // 手写递归
来源：http://sas.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gsr.shangyingyoupin.top

C#:   // 手写递归
来源：http://jac.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gox.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oyc.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ndc.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofx.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mbm.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://laz.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://siz.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://etr.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://amn.snrcjt.cn

================================================================================
来源：http://nzi.ehwqpu.com

O. 并发与异步
来源：http://pqv.ydjk.org.cn

================================================================================
来源：http://jpk.quarkkingdee.top

[O01] 启动一个线程
来源：http://tel.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://crx.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jqc.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ifq.pycfn.com

TS:   // 同 JS
来源：http://upb.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://itv.sufxvd.cn

Go:   go f()
来源：http://vxb.ybcxt.top

Ruby: Thread.new { f }
来源：http://bui.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://ega.sysykeji.top

[O02] 使用线程池
来源：http://tnf.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mdd.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ujr.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://ian.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://dlq.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aak.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://geg.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lvp.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qyc.bbcook.cn

[O03] 加锁保护共享数据
来源：http://cum.snrcjt.cn

Py:   with lock: shared += 1
来源：http://zwf.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zlq.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wnl.nanxinkj.top

TS:   // 同 JS
来源：http://fge.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://ljd.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wqe.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://huv.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://oqz.pycfn.com

[O04] 定义异步函数并等待
来源：http://hkr.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://rnu.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dby.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://vxu.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jza.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://phn.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyq.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://sha.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://gbk.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://aog.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://hrl.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jkk.sweek.top

JS:   await Promise.all(tasks)
来源：http://siu.tanke756.top

TS:   await Promise.all(tasks)
来源：http://gjc.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jid.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rig.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://yxb.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rut.zdqjudy.top

[O06] 使用进程池
来源：http://lvk.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rfg.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gwk.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://byw.birdmap.top


<!-- 参考信息 -->