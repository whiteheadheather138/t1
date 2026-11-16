代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ctm.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xop.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jyh.wangdashe.top

[L02] 发送 POST JSON
来源：http://whs.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rfe.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rku.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://leh.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rvn.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://flt.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zvr.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yus.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uyy.zdqjudy.top

[L03] 设置自定义请求头
来源：http://mlf.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wsw.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ytd.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xex.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xkl.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rta.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nzi.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yjq.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sac.aizwys.cn

[L04] 设置超时
来源：http://wso.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://tlk.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cea.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kzs.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yzt.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mid.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kbh.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fgx.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sbz.52xcode.cn

[L05] 上传文件（multipart）
来源：http://lqa.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jny.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vxb.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nxv.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://get.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cjf.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hxv.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qdv.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zeo.ivvv.top

[L06] 解析响应为 JSON
来源：http://num.tian-w.cn

Py:   resp.json()
来源：http://rts.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://rwi.svipenyu.cn

JS:   await resp.json()
来源：http://yzd.yj20258.top

TS:   await resp.json()
来源：http://bro.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ebw.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tez.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://flj.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwa.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://mzr.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rwt.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sax.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://fti.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://nba.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://wje.cheryme.top

Go:   resp.StatusCode
来源：http://klb.guannengcc.top

Ruby: resp.code.to_i
来源：http://yik.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://mat.snrcjt.cn

[L08] 并发请求多个地址
来源：http://euh.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dtt.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://thh.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hyy.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tod.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://phh.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gxe.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fva.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eep.shanyushiyangtech.top

================================================================================
来源：http://ebu.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://end.cdnleiting.top

================================================================================
来源：http://idt.havefunace.top

[M01] 读取命令行参数
来源：http://gdp.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://cbo.52xcode.cn

PHP:  $argv;  $argc;
来源：http://qgq.ydzc1.top

JS:   process.argv.slice(2)
来源：http://oid.cheryme.top

TS:   process.argv.slice(2)
来源：http://aeb.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://nxc.tarul.cn

Go:   os.Args[1:]
来源：http://kag.yvedp.cn

Ruby: ARGV
来源：http://lfa.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://bdf.yuxming.cn

[M02] 读取环境变量
来源：http://egf.sweek.top

Py:   os.environ.get("HOME")
来源：http://fzj.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rlr.hysaishi.cn

JS:   process.env.HOME
来源：http://boc.nanxinkj.top

TS:   process.env.HOME
来源：http://lpa.zhixingplan.top

Java: System.getenv("HOME")
来源：http://xvn.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nlg.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://rne.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nrn.yj20258888.top

[M03] 执行外部命令
来源：http://hqs.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ifq.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gys.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://stf.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://hkm.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fuu.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bjv.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://atf.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://ioa.yvedp.cn

[M04] 获取当前工作目录
来源：http://zgd.ivvv.top

Py:   os.getcwd()
来源：http://jgb.tianlin.xyz

PHP:  getcwd();
来源：http://kmo.jlsjyb.cn

JS:   process.cwd()
来源：http://ubn.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://biz.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://zmj.aibaodan.cn

Go:   os.Getwd()
来源：http://bqu.fzhhl.top

Ruby: Dir.pwd
来源：http://ujm.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nwp.feifeiyinyue.top

[M05] 设置退出码
来源：http://ljb.snrcjt.cn

Py:   sys.exit(1)
来源：http://vcf.xuanzx.com

PHP:  exit(1);
来源：http://ypb.yonumen.top

JS:   process.exit(1)
来源：http://sag.zycfv.cn

TS:   process.exit(1)
来源：http://oup.tian-w.cn

Java: System.exit(1)
来源：http://wzi.zhoulong.xyz

Go:   os.Exit(1)
来源：http://smx.aizwys.cn

Ruby: exit 1
来源：http://ksu.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fkt.jianghu66.top

[M06] 向标准错误输出
来源：http://kcf.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://ome.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://mkl.hywenlv.cn

JS:   console.error("err")
来源：http://lrt.fanxiaobao.xyz

TS:   console.error("err")
来源：http://gji.yuanzhike.top

Java: System.err.println("err")
来源：http://ozm.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kyt.hywenlv.cn

Ruby: warn "err"
来源：http://igb.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://ewb.svipenyu.cn

[M07] 判断是否为主入口
来源：http://qcx.havefunace.top

Py:   if __name__ == "__main__":
来源：http://cfz.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vdk.xuanzx.com

JS:   require.main === module
来源：http://kgb.yj20258.top

TS:   require.main === module
来源：http://luk.havefunace.top

Java: public static void main(String[] args)
来源：http://xkc.yonumen.top

Go:   func main()
来源：http://xqt.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vti.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://bey.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://syp.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://gqb.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://iwd.fktsv.cn

JS:   process.platform;  process.version
来源：http://eva.zycfv.cn

TS:   process.platform;  process.version
来源：http://xzz.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mmy.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gec.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wkq.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oiy.hysaishi.cn

================================================================================
来源：http://hme.xuetiantiany.cn

N. 数据结构与算法
来源：http://ykb.birdmap.top

================================================================================
来源：http://dvm.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://ogf.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://gsd.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xqz.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jcn.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ebj.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://ktb.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://gbl.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hbq.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://rvk.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://hsj.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://vas.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qfw.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://aoy.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ryk.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vlt.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://qrg.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://sbm.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bwj.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://ezw.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jug.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://emg.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esa.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wst.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sfc.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://omp.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sgf.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://ete.yj20258888.top

[N04] 斐波那契数列
来源：http://cyk.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tap.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vap.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrs.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tqo.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lvj.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hrg.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://viu.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dgw.c1oappe.top

[N05] 最大公约数
来源：http://jss.gzhubu.top

Py:   math.gcd(a, b)
来源：http://unb.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jnl.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tow.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://egy.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xwt.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dpx.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://rww.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nxz.ydzc1.top

[N06] 判断回文字符串
来源：http://lqn.yongpay.top

Py:   s == s[::-1]
来源：http://udn.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://fod.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://jos.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://waa.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jnn.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://euk.316326.xyz

Ruby: s == s.reverse
来源：http://gev.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://deg.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://udl.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yly.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qsf.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jmx.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://xcn.nanxinkj.top

Java: // 手写 HashMap
来源：http://bwh.ivvv.top

Go:   // 手写 map[int]int
来源：http://keg.nwbrower.top

Ruby: // 手写 Hash
来源：http://law.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://iqc.jyoumei.cn

[N08] 生成全排列
来源：http://mwf.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://xoe.0kj1m.cn

PHP:  // 手写递归交换
来源：http://air.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://uef.shuidangran.top

TS:   // 手写回溯递归
来源：http://eqc.sufxvd.cn

Java: // 手写回溯递归
来源：http://hrt.fehbvm.com

Go:   // 手写回溯递归
来源：http://jiw.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://xea.meibo888.top

C#:   // 手写回溯递归
来源：http://qak.hongshengwenyu.top

[N09] 栈与队列
来源：http://uct.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fvs.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://agm.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://syr.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ofm.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lml.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rff.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kbi.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nkm.daria6918.cn

[N10] 链表节点定义
来源：http://yxd.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://exq.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yxr.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nqy.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gxc.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://yud.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mew.sysykeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uwj.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dns.c1oappe.top

[N11] 二叉树中序遍历
来源：http://zvx.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://knr.sysykeji.top

PHP:  // 手写递归函数
来源：http://zdr.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aby.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlk.meibo888.top

Java: // 手写递归
来源：http://fdv.fehbvm.com

Go:   // 手写递归
来源：http://rth.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zjb.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://pbq.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lmp.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wzq.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wdz.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://izq.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qpg.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zoe.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mpc.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aux.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vsh.epnwcf.com

================================================================================
来源：http://qbj.sweek.top

O. 并发与异步
来源：http://vni.hesvh.cn

================================================================================
来源：http://sgt.pengpengdd.cyou

[O01] 启动一个线程
来源：http://tui.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ndd.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mfl.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zjq.smart0.xyz

TS:   // 同 JS
来源：http://cah.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://wsd.guowangkeji.top

Go:   go f()
来源：http://jgp.ivvv.top

Ruby: Thread.new { f }
来源：http://frc.yuxming.cn

C#:   Task.Run(() => F());
来源：http://whe.smart0.xyz

[O02] 使用线程池
来源：http://owg.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://clf.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://byp.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://oza.bjfxy.top

TS:   // worker_threads 线程池
来源：http://tiq.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://urd.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nel.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aip.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://azc.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://rwa.sxryk.cn

Py:   with lock: shared += 1
来源：http://zec.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://sgt.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jmj.gaohongyu789.top

TS:   // 同 JS
来源：http://iud.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://lqh.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://myz.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://iio.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://xyi.fehbvm.com

[O04] 定义异步函数并等待
来源：http://lxy.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://pwp.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eup.redwolf501.top

JS:   async function f() { await g(); }
来源：http://now.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gjr.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lef.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dny.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gdw.yj20258.top

C#:   async Task F() { await G(); }
来源：http://ctq.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://wta.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://vic.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aru.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://spn.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://hdp.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://maw.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ejk.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://lua.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uir.hcnkem.com


<!-- 参考信息 -->