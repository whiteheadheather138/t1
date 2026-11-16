代发 wailian999

Go:   encoding/gob
来源：http://vhm.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://qyi.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://clz.tanke756.top

================================================================================
来源：http://mcl.zhijiandao.cn

L. 网络请求
来源：http://jsg.nanxinkj.top

================================================================================
来源：http://buu.jqgfzy.top

[L01] 发送 GET 请求
来源：http://ykj.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ygp.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yjp.nwbrower.top

JS:   await fetch(url)
来源：http://gow.jiagoushi.top

TS:   await fetch(url)
来源：http://kop.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xul.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://bdl.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jui.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ziy.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://jjb.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xqi.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kaf.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgh.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sda.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ffn.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nfy.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ega.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://efw.meibo888.top

[L03] 设置自定义请求头
来源：http://pbi.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rlr.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vog.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ddk.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pib.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hcd.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://snm.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ohw.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uxu.zdqjudy.top

[L04] 设置超时
来源：http://moy.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://asn.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://szo.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yna.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://myw.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vri.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lnx.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwm.tarul.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rjr.aizwys.cn

[L05] 上传文件（multipart）
来源：http://bfs.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uxv.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://our.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://egm.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://usp.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uiq.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cjh.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xqv.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kym.ydzc1.top

[L06] 解析响应为 JSON
来源：http://mma.sufxvd.cn

Py:   resp.json()
来源：http://qcb.hesvh.cn

PHP:  json_decode($body, true);
来源：http://fmm.shanyushiyangtech.top

JS:   await resp.json()
来源：http://hee.jinqigufen.top

TS:   await resp.json()
来源：http://gup.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tpp.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bkw.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://bav.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bxa.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://enm.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vlo.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qdg.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://yxz.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://oty.zdbjq.cn

Java: resp.statusCode()
来源：http://vjx.cashguo.top

Go:   resp.StatusCode
来源：http://qqu.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://lgg.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://rcw.tanke756.top

[L08] 并发请求多个地址
来源：http://nlc.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://abt.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://lch.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ctn.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ref.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://znh.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://itj.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://khp.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kit.xziqi.cn

================================================================================
来源：http://ebs.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://ksn.epnwcf.com

================================================================================
来源：http://kth.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://zpc.yonumen.top

Py:   sys.argv[1:]
来源：http://trv.bbcook.cn

PHP:  $argv;  $argc;
来源：http://mzg.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://fot.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://qav.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://lob.bjfxy.top

Go:   os.Args[1:]
来源：http://tjh.ctjpmb.com

Ruby: ARGV
来源：http://bqy.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://kkh.gaohongyu789.top

[M02] 读取环境变量
来源：http://wrb.tanke756.top

Py:   os.environ.get("HOME")
来源：http://yqt.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ptb.shangyingyoupin.top

JS:   process.env.HOME
来源：http://heg.yvedp.cn

TS:   process.env.HOME
来源：http://gwz.gzhubu.top

Java: System.getenv("HOME")
来源：http://dwg.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hoo.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://vax.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mfr.snrcjt.cn

[M03] 执行外部命令
来源：http://yia.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ven.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jfi.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://qka.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lyn.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://irg.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nyc.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mkm.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://hmt.meibo888.top

[M04] 获取当前工作目录
来源：http://tow.0kj1m.cn

Py:   os.getcwd()
来源：http://tgu.jlsjyb.cn

PHP:  getcwd();
来源：http://dgl.kuanghao11.cn

JS:   process.cwd()
来源：http://qew.vqdsnc.cn

TS:   process.cwd()
来源：http://lqh.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://irv.haohaochexian.top

Go:   os.Getwd()
来源：http://hjh.0kj1m.cn

Ruby: Dir.pwd
来源：http://aff.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://jxh.meibo888.top

[M05] 设置退出码
来源：http://vvv.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://wxu.yueranfly.top

PHP:  exit(1);
来源：http://avk.sysykeji.top

JS:   process.exit(1)
来源：http://juc.pycfn.com

TS:   process.exit(1)
来源：http://qme.uphjek.com

Java: System.exit(1)
来源：http://tkz.nwbrower.top

Go:   os.Exit(1)
来源：http://eyt.hammf.cn

Ruby: exit 1
来源：http://kdq.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://onp.svipenyu.cn

[M06] 向标准错误输出
来源：http://dpq.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://rtj.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ffr.yvedp.cn

JS:   console.error("err")
来源：http://ndf.zdqjudy.top

TS:   console.error("err")
来源：http://wgz.yonumen.top

Java: System.err.println("err")
来源：http://aiu.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sxz.zhixingplan.top

Ruby: warn "err"
来源：http://xxy.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://igi.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://gqh.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://big.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tkp.daxiang520.top

JS:   require.main === module
来源：http://qqd.c1oappe.top

TS:   require.main === module
来源：http://hyq.dianchejie.cn

Java: public static void main(String[] args)
来源：http://gmv.kuanghao11.cn

Go:   func main()
来源：http://oxu.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xlu.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://lyl.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://zvj.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://ikv.fengsongda.top

PHP:  PHP_OS;  phpversion();
来源：http://syh.cashguo.top

JS:   process.platform;  process.version
来源：http://rqa.zhengqikj.top

TS:   process.platform;  process.version
来源：http://rop.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qyw.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://woj.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rxs.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jrm.fengsongda.top

================================================================================
来源：http://gfl.yanxiufei.cn

N. 数据结构与算法
来源：http://mjf.yongpay.top

================================================================================
来源：http://mzv.sweek.top

[N01] 二分查找（有序数组）
来源：http://pca.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tpa.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xas.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qxe.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dvl.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://gds.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://ciu.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://esu.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://ssq.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://syu.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://cgq.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nqa.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ozx.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lna.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jal.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://zgi.nanxuanxn.top

Ruby: arr.sort
来源：http://fbs.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ktj.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://rlz.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aks.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://wrf.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://khf.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qky.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wwu.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lip.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://byv.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://fpu.zdqjudy.top

[N04] 斐波那契数列
来源：http://uef.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tku.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gje.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eab.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpn.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gkc.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uqf.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uca.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bge.sufxvd.cn

[N05] 最大公约数
来源：http://sxu.smart0.xyz

Py:   math.gcd(a, b)
来源：http://obz.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tsh.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqn.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://poe.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wyy.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://moo.bbcook.cn

Ruby: a.gcd(b)
来源：http://mch.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ozh.zdbjq.cn

[N06] 判断回文字符串
来源：http://war.tarul.cn

Py:   s == s[::-1]
来源：http://xdx.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://wtp.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://tws.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://sej.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lze.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://rbw.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://htg.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ifc.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://dnc.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ewp.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://akq.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iio.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://zph.svipenyu.cn

Java: // 手写 HashMap
来源：http://bav.hesvh.cn

Go:   // 手写 map[int]int
来源：http://shj.yfazqb.com

Ruby: // 手写 Hash
来源：http://fyh.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ewu.hammf.cn

[N08] 生成全排列
来源：http://uyw.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://gzy.ctjpmb.com

PHP:  // 手写递归交换
来源：http://jzg.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://hsi.hesvh.cn

TS:   // 手写回溯递归
来源：http://hoc.zycfv.cn

Java: // 手写回溯递归
来源：http://qkl.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://iav.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://xkg.hfpthk.cn

C#:   // 手写回溯递归
来源：http://trk.ydjk.org.cn

[N09] 栈与队列
来源：http://pyq.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gkh.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ggf.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gum.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://weu.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dro.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qnm.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sqc.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qce.hesvh.cn

[N10] 链表节点定义
来源：http://yhw.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://run.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vcm.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bhj.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eep.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://fbr.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iyt.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hnu.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nqs.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://ton.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dto.svipenyu.cn

PHP:  // 手写递归函数
来源：http://fcx.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pov.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://smx.guowangkeji.top

Java: // 手写递归
来源：http://yhu.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://zgm.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yaj.ppjwa.cn

C#:   // 手写递归
来源：http://owh.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gvz.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jyt.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zos.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tdo.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cns.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kgg.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pdg.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pmk.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kcc.shanyushiyangkeji.top

================================================================================
来源：http://zay.smart0.xyz

O. 并发与异步
来源：http://avj.ctjpmb.com

================================================================================
来源：http://qhu.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://wlo.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://axt.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hwz.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://krt.guowangkeji.top

TS:   // 同 JS
来源：http://fhu.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://cjm.wangshuangyany.cn

Go:   go f()
来源：http://smt.ybcxt.top

Ruby: Thread.new { f }
来源：http://jfg.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://fqh.yfazqb.com

[O02] 使用线程池
来源：http://zwe.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rie.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qob.tian-w.cn

JS:   // worker_threads 线程池
来源：http://yau.guannengcc.top

TS:   // worker_threads 线程池
来源：http://rmm.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://uda.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://avy.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hpq.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dva.52xcode.cn

[O03] 加锁保护共享数据
来源：http://itz.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://ery.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://kxa.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://njc.haohaochexian.top

TS:   // 同 JS
来源：http://ogd.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://ake.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sij.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kiq.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://gjw.daria6918.cn

[O04] 定义异步函数并等待
来源：http://uco.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://enn.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eeu.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://fyk.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://icz.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ccb.ydjk.org.cn


<!-- 参考信息 -->