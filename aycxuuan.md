代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jlj.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://akw.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jmg.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tdt.hysaishi.cn

[L03] 设置自定义请求头
来源：http://dcr.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rzs.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://esp.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mgk.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfy.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vnm.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fzs.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ygw.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oci.yangfankeji.com

[L04] 设置超时
来源：http://qvn.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://car.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lfo.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://exh.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmz.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://upo.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wgp.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hqb.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ety.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://fws.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uwq.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sab.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dnf.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bch.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qwg.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://grh.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://upx.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ttf.xinyue.icu

[L06] 解析响应为 JSON
来源：http://wtr.pengpengdd.cyou

Py:   resp.json()
来源：http://afm.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://ktq.nanxinkj.top

JS:   await resp.json()
来源：http://qlq.vqdsnc.cn

TS:   await resp.json()
来源：http://bef.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xhn.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jaw.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://jgr.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bwq.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://xle.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mfl.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbu.yj20258.top

JS:   resp.ok;  resp.status
来源：http://wml.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://jvb.jlsjyb.cn

Java: resp.statusCode()
来源：http://hoc.meibo888.top

Go:   resp.StatusCode
来源：http://sjc.zdbjq.cn

Ruby: resp.code.to_i
来源：http://zgt.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://vjy.yuxming.cn

[L08] 并发请求多个地址
来源：http://zfu.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vxv.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://kxw.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipl.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yop.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://apn.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wab.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bns.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dxo.bjfxy.top

================================================================================
来源：http://cqo.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://kqn.zhaomingkeji.xyz

================================================================================
来源：http://dzc.zhengqikj.top

[M01] 读取命令行参数
来源：http://tyf.haohaochexian.top

Py:   sys.argv[1:]
来源：http://vey.tarul.cn

PHP:  $argv;  $argc;
来源：http://bpv.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://bqq.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://jxz.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://qgq.gaohongyu789.top

Go:   os.Args[1:]
来源：http://wry.shanyushiyangtech.top

Ruby: ARGV
来源：http://vul.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://ebz.iojbl.cn

[M02] 读取环境变量
来源：http://dkd.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://isd.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kwo.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://tkg.shangyingyoupin.top

TS:   process.env.HOME
来源：http://mlk.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://tsl.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vpn.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://kqe.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://anq.cdnleiting.top

[M03] 执行外部命令
来源：http://hbs.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yfe.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ayi.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wjw.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hgn.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wtc.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xlh.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://tgx.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://ffx.nwbrower.top

[M04] 获取当前工作目录
来源：http://aba.fehbvm.com

Py:   os.getcwd()
来源：http://tyc.svipenyu.cn

PHP:  getcwd();
来源：http://iod.daxiang520.top

JS:   process.cwd()
来源：http://qsk.c1oappe.top

TS:   process.cwd()
来源：http://cdp.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://cep.jianghu66.top

Go:   os.Getwd()
来源：http://woa.zdqjudy.top

Ruby: Dir.pwd
来源：http://yux.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hfe.zhixingplan.top

[M05] 设置退出码
来源：http://ouz.jqgfzy.top

Py:   sys.exit(1)
来源：http://bop.yfazqb.com

PHP:  exit(1);
来源：http://mzd.ppjwa.cn

JS:   process.exit(1)
来源：http://hop.zhiwuduotai.top

TS:   process.exit(1)
来源：http://dre.chenjidiqi.icu

Java: System.exit(1)
来源：http://yii.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://awo.andypj.xyz

Ruby: exit 1
来源：http://fpu.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hft.316326.xyz

[M06] 向标准错误输出
来源：http://yah.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://okd.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vyf.shangyingyoupin.top

JS:   console.error("err")
来源：http://chh.gaohongyu789.top

TS:   console.error("err")
来源：http://fdl.gogol.net.cn

Java: System.err.println("err")
来源：http://ijv.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knl.sjlbkw.cn

Ruby: warn "err"
来源：http://ojk.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://kde.wangdashe.top

[M07] 判断是否为主入口
来源：http://awx.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://uew.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cdt.daxiang520.top

JS:   require.main === module
来源：http://aow.zhaomingkeji.xyz

TS:   require.main === module
来源：http://xcl.sysykeji.top

Java: public static void main(String[] args)
来源：http://ouy.shangyingyoupin.top

Go:   func main()
来源：http://jso.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hgt.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://wxf.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://mfc.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://ngm.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://cgq.gogol.net.cn

JS:   process.platform;  process.version
来源：http://ybl.gotoacloud.top

TS:   process.platform;  process.version
来源：http://tqz.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://unm.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://hth.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nug.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hut.hnqzz.top

================================================================================
来源：http://pqy.zycfv.cn

N. 数据结构与算法
来源：http://fjn.gzhubu.top

================================================================================
来源：http://qxr.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://ijh.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://tmy.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lne.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mtc.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zar.zdbjq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zfp.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://jni.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dst.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qpt.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://xbt.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://jxl.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tdv.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://htm.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yul.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mtv.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://hlo.daria6918.cn

Ruby: arr.sort
来源：http://zzw.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gbv.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://phm.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ewu.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://mea.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sll.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://upm.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dnb.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vzt.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gme.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://esf.vqdsnc.cn

[N04] 斐波那契数列
来源：http://gok.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dfr.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nar.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ete.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://imx.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trf.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dif.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://shx.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vta.aibaodan.cn

[N05] 最大公约数
来源：http://oam.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://zft.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nre.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sws.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lsq.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lie.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iuf.xziqi.cn

Ruby: a.gcd(b)
来源：http://enc.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tef.zhixingplan.top

[N06] 判断回文字符串
来源：http://vae.hnxiangtu.top

Py:   s == s[::-1]
来源：http://opp.meibo888.top

PHP:  $s === strrev($s);
来源：http://yam.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://qja.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://oxc.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bxc.wangdashe.top

Go:   // 双指针从两端比较
来源：http://koo.cqqwz.cn

Ruby: s == s.reverse
来源：http://ila.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wfh.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://pph.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://swd.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://waa.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://sru.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://ley.jianghu66.top

Java: // 手写 HashMap
来源：http://ynu.cheryme.top

Go:   // 手写 map[int]int
来源：http://lgz.yueranfly.top

Ruby: // 手写 Hash
来源：http://lix.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mcr.zdqjudy.top

[N08] 生成全排列
来源：http://oon.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://oej.ctjpmb.com

PHP:  // 手写递归交换
来源：http://qlg.uphjek.com

JS:   // 手写回溯递归
来源：http://vuj.tanke756.top

TS:   // 手写回溯递归
来源：http://mpd.sxryk.cn

Java: // 手写回溯递归
来源：http://qui.hywenlv.cn

Go:   // 手写回溯递归
来源：http://gij.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://psj.cheryme.top

C#:   // 手写回溯递归
来源：http://ksv.hnqzz.top

[N09] 栈与队列
来源：http://llw.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vtk.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cku.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jmo.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mrw.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eep.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yyy.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://imb.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://imk.hnqzz.top

[N10] 链表节点定义
来源：http://wfu.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vzu.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uma.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nbr.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zwm.yongpay.top

Java: class Node { int v; Node next; }
来源：http://cjv.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://rpk.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rve.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yju.c1oappe.top

[N11] 二叉树中序遍历
来源：http://dcm.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cbo.yongpay.top

PHP:  // 手写递归函数
来源：http://nax.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ker.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lmz.9152youxi.cn

Java: // 手写递归
来源：http://bcv.zhixingplan.top

Go:   // 手写递归
来源：http://nit.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wfq.zhijiandao.cn

C#:   // 手写递归
来源：http://xqq.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fpv.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbg.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wsm.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://brp.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://olf.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mhr.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sdp.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ztn.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ftg.xingfuxueyuan.xyz

================================================================================
来源：http://wft.hnqzz.top

O. 并发与异步
来源：http://ogw.zhaomingkeji.xyz

================================================================================
来源：http://xkf.xinyue.icu

[O01] 启动一个线程
来源：http://bat.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://koj.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ukz.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vql.yj20258888.top

TS:   // 同 JS
来源：http://tvu.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://qie.ehwqpu.com

Go:   go f()
来源：http://sga.yangfankeji.com

Ruby: Thread.new { f }
来源：http://cin.havefunace.top

C#:   Task.Run(() => F());
来源：http://avv.yuxming.cn

[O02] 使用线程池
来源：http://rja.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wly.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mby.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://jtz.xziqi.cn

TS:   // worker_threads 线程池
来源：http://zmc.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://xfl.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zlv.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://usy.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://crc.yvedp.cn

[O03] 加锁保护共享数据
来源：http://rpf.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://vxi.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://dnt.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ndt.tarul.cn

TS:   // 同 JS
来源：http://nwa.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://shl.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gte.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lkm.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://pdw.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://fth.cheryme.top

Py:   async def f():⏎    await g()
来源：http://syy.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ynf.tarul.cn

JS:   async function f() { await g(); }
来源：http://dej.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://mjf.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://plz.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pmi.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rgx.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://eob.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://xgj.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://lmi.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fwr.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://hcp.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://jaj.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qca.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://awx.hammf.cn

Ruby: threads.map(&:join)
来源：http://qpi.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://sbl.yfazqb.com

[O06] 使用进程池
来源：http://diu.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xku.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nrw.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://bpy.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://bwc.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jie.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mat.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://rff.zhijiandao.cn


<!-- 参考信息 -->