代发 wailian999

Go:   encoding/gob
来源：http://seo.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://cbc.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lws.ydjk.org.cn

================================================================================
来源：http://xev.sxryk.cn

L. 网络请求
来源：http://jej.vehdjk.com

================================================================================
来源：http://vya.ydzc1.top

[L01] 发送 GET 请求
来源：http://ljl.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://atm.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ukj.shangyingyoupin.top

JS:   await fetch(url)
来源：http://xwm.kuanghao11.cn

TS:   await fetch(url)
来源：http://rtw.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gdx.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://nvb.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vya.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ofb.cucudq.cn

[L02] 发送 POST JSON
来源：http://eut.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fxg.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dls.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uln.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bzl.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kyj.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ail.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tin.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tio.zhixingplan.top

[L03] 设置自定义请求头
来源：http://hnw.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://niv.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hoa.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pwj.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://heg.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://enc.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kgc.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jbf.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mym.jinqigfzy.top

[L04] 设置超时
来源：http://thz.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://eer.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qrp.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gca.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwr.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ekw.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rfa.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kvp.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vqr.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://vtk.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xqc.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://you.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lsg.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iqo.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://deu.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xty.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xez.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://veq.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://buq.feifeiyinyue.top

Py:   resp.json()
来源：http://fli.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://bdp.shanyushiyangtech.top

JS:   await resp.json()
来源：http://ufb.jinghuilouyu.cn

TS:   await resp.json()
来源：http://yfd.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mzz.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ngp.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://tmg.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qdn.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://bnf.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ozg.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kce.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://rai.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://ihv.uphjek.com

Java: resp.statusCode()
来源：http://lqe.epnwcf.com

Go:   resp.StatusCode
来源：http://tdm.yvedp.cn

Ruby: resp.code.to_i
来源：http://ght.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://rek.zdbjq.cn

[L08] 并发请求多个地址
来源：http://wfi.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ukl.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://dno.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tkh.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kjd.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ezf.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qvc.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hlt.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zpn.fzhhl.top

================================================================================
来源：http://dsz.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://dtx.ctjpmb.com

================================================================================
来源：http://knp.zhoulong.xyz

[M01] 读取命令行参数
来源：http://boi.c1oappe.top

Py:   sys.argv[1:]
来源：http://woe.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://lsi.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://tcl.316326.xyz

TS:   process.argv.slice(2)
来源：http://tdh.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://cfe.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://zgf.jiagoushi.top

Ruby: ARGV
来源：http://okl.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://ngd.chenlongwang.top

[M02] 读取环境变量
来源：http://dww.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://wzs.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tkm.dianchejie.cn

JS:   process.env.HOME
来源：http://amn.aizwys.cn

TS:   process.env.HOME
来源：http://fqn.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://ice.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ava.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://rwo.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oxr.shzxlz.cn

[M03] 执行外部命令
来源：http://vty.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://igk.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pkg.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wuq.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jru.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tdw.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wdl.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://axa.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://wpf.hcnkem.com

[M04] 获取当前工作目录
来源：http://pfq.ydjk.org.cn

Py:   os.getcwd()
来源：http://srt.yuxming.cn

PHP:  getcwd();
来源：http://zhd.pycfn.com

JS:   process.cwd()
来源：http://ivl.xuanzx.com

TS:   process.cwd()
来源：http://wpy.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://lhv.jianghu66.top

Go:   os.Getwd()
来源：http://dpp.gogol.net.cn

Ruby: Dir.pwd
来源：http://bef.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://hoe.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://mnf.chenlongwang.top

Py:   sys.exit(1)
来源：http://snf.zycfv.cn

PHP:  exit(1);
来源：http://kow.hcnkem.com

JS:   process.exit(1)
来源：http://pfc.pycfn.com

TS:   process.exit(1)
来源：http://pez.jlsjyb.cn

Java: System.exit(1)
来源：http://zrp.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://pgr.fanxiaobao.xyz

Ruby: exit 1
来源：http://sxu.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xih.ydzc1.top

[M06] 向标准错误输出
来源：http://mwn.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://vkz.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qew.fehbvm.com

JS:   console.error("err")
来源：http://dst.yfazqb.com

TS:   console.error("err")
来源：http://izb.zhiwuduotai.top

Java: System.err.println("err")
来源：http://moe.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tiz.zycfv.cn

Ruby: warn "err"
来源：http://kkb.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://xsx.shzxlz.cn

[M07] 判断是否为主入口
来源：http://cgb.birdmap.top

Py:   if __name__ == "__main__":
来源：http://xnt.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pvw.havefunace.top

JS:   require.main === module
来源：http://sqi.shzxlz.cn

TS:   require.main === module
来源：http://nxh.fktsv.cn

Java: public static void main(String[] args)
来源：http://swt.vehdjk.com

Go:   func main()
来源：http://mca.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pqy.hesvh.cn

C#:   static void Main(string[] args)
来源：http://gqn.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://fas.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://lho.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://glb.yvedp.cn

JS:   process.platform;  process.version
来源：http://swa.ivvv.top

TS:   process.platform;  process.version
来源：http://fxa.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wwz.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yuw.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxb.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vvj.hnxiangtu.top

================================================================================
来源：http://fgv.zhijiandao.cn

N. 数据结构与算法
来源：http://vqf.ywan-chungtsiang.top

================================================================================
来源：http://trn.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://ebh.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xtm.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wet.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kxb.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dnc.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qhf.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://hlz.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sfb.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://sve.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://ugv.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://ivh.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ucm.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rhe.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpn.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://htu.vehdjk.com

Go:   slices.Sort(arr)
来源：http://pdb.andypj.xyz

Ruby: arr.sort
来源：http://avl.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jcj.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://zex.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xse.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://dnf.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghi.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rni.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lbi.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vds.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bbo.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://awu.gotoacloud.top

[N04] 斐波那契数列
来源：http://uto.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baq.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yhe.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bjp.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mvo.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uap.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ymz.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vjx.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xmo.gzhubu.top

[N05] 最大公约数
来源：http://fpl.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://cza.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gvj.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ikd.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cbu.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xlc.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zee.daria6918.cn

Ruby: a.gcd(b)
来源：http://ebl.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wqu.ctjpmb.com

[N06] 判断回文字符串
来源：http://iyr.jyoumei.cn

Py:   s == s[::-1]
来源：http://xnn.daxiang520.top

PHP:  $s === strrev($s);
来源：http://mkj.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://fmo.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://osl.uphjek.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vzf.cucudq.cn

Go:   // 双指针从两端比较
来源：http://zpt.hysaishi.cn

Ruby: s == s.reverse
来源：http://nxm.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yra.pycfn.com

[N07] 两数之和（返回下标）
来源：http://hjo.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ney.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yhy.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tga.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://nob.ydzc1.top

Java: // 手写 HashMap
来源：http://tyy.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://psk.tian-w.cn

Ruby: // 手写 Hash
来源：http://upq.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://jii.ydjk.org.cn

[N08] 生成全排列
来源：http://qfq.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://onm.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://qnc.daria6918.cn

JS:   // 手写回溯递归
来源：http://fob.aizwys.cn

TS:   // 手写回溯递归
来源：http://ufh.fehbvm.com

Java: // 手写回溯递归
来源：http://wsw.cheryme.top

Go:   // 手写回溯递归
来源：http://bws.yj20258.top

Ruby: arr.permutation.to_a
来源：http://vnv.havefunace.top

C#:   // 手写回溯递归
来源：http://ufs.tianlin.xyz

[N09] 栈与队列
来源：http://gro.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kzm.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rxx.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mtz.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rua.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://erl.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ezl.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fct.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nmb.smart0.xyz

[N10] 链表节点定义
来源：http://nmu.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xiy.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hnt.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xrm.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://igv.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://wdc.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ijy.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wsf.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xri.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://fpi.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://asp.cheryme.top

PHP:  // 手写递归函数
来源：http://occ.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrp.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hwn.zhongyouzk.top

Java: // 手写递归
来源：http://teq.xylfe.cn

Go:   // 手写递归
来源：http://lhl.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zus.chenjidiqi.icu

C#:   // 手写递归
来源：http://obe.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ili.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rqw.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tpn.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xtu.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mlr.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xdt.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kbv.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eab.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ygr.svipenyu.cn

================================================================================
来源：http://znr.pycfn.com

O. 并发与异步
来源：http://mik.meibo888.top

================================================================================
来源：http://jmw.zhijiandao.cn

[O01] 启动一个线程
来源：http://son.ydzc1.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ybg.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bev.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vtm.zhoulong.xyz

TS:   // 同 JS
来源：http://rje.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://tmk.shangyingyoupin.top

Go:   go f()
来源：http://zud.havefunace.top

Ruby: Thread.new { f }
来源：http://txa.tian-w.cn

C#:   Task.Run(() => F());
来源：http://hmz.dashuyun.cn

[O02] 使用线程池
来源：http://tpb.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bhv.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zzg.xziqi.cn

JS:   // worker_threads 线程池
来源：http://awf.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://eal.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://ygh.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hvd.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jzd.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cfp.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://ybc.meibo888.top

Py:   with lock: shared += 1
来源：http://jge.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://uko.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mnb.gaohongyu789.top

TS:   // 同 JS
来源：http://pvy.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://bmc.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iqz.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://alb.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://qhx.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://vdn.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://lyr.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mtw.tarul.cn

JS:   async function f() { await g(); }
来源：http://kbi.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gae.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kby.ydzc1.top


<!-- 参考信息 -->