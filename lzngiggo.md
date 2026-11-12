代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://tbk.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cyl.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aug.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ksf.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://myj.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ekc.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zam.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://goh.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://ipe.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tuc.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://avx.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzp.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xon.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://esz.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nel.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://whi.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wpu.zdqjudy.top

[L04] 设置超时
来源：http://ydy.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://rsf.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ylh.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdw.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tco.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cbo.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gpo.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://trg.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://exm.uphjek.com

[L05] 上传文件（multipart）
来源：http://upn.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uzj.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pgk.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nys.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://csw.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lfw.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cuh.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ovn.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wkl.xziqi.cn

[L06] 解析响应为 JSON
来源：http://wnb.zdqjudy.top

Py:   resp.json()
来源：http://jvv.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://jlp.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://cgr.xuetiantiany.cn

TS:   await resp.json()
来源：http://zyb.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fsb.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uss.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://xin.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lpw.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://yoy.shangyingyoupin.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ceg.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://var.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://wng.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://nfl.shangyingyoupin.top

Java: resp.statusCode()
来源：http://wkf.haohaochexian.top

Go:   resp.StatusCode
来源：http://cyy.ybcxt.top

Ruby: resp.code.to_i
来源：http://sdt.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://vhf.hywenlv.cn

[L08] 并发请求多个地址
来源：http://qvi.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yme.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://xju.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxq.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ahc.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njb.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://txk.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prv.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dth.yfazqb.com

================================================================================
来源：http://hvh.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://zvv.xylfe.cn

================================================================================
来源：http://src.jianghu66.top

[M01] 读取命令行参数
来源：http://kfc.shzxlz.cn

Py:   sys.argv[1:]
来源：http://zfp.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://jab.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://etx.shuidangran.top

TS:   process.argv.slice(2)
来源：http://pjb.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://wix.bjfxy.top

Go:   os.Args[1:]
来源：http://alz.gaohongyu789.top

Ruby: ARGV
来源：http://mod.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://fob.tanke756.top

[M02] 读取环境变量
来源：http://wnb.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://mvj.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xse.xinyue.icu

JS:   process.env.HOME
来源：http://wvn.nanxinkj.top

TS:   process.env.HOME
来源：http://oxf.cucudq.cn

Java: System.getenv("HOME")
来源：http://dad.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddr.wangdashe.top

Ruby: ENV["HOME"]
来源：http://csb.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://htt.nwbrower.top

[M03] 执行外部命令
来源：http://ycm.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fwo.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aat.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ufk.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eul.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hpy.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dbl.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://kew.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://noz.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://wqi.ctjpmb.com

Py:   os.getcwd()
来源：http://rso.wangshuangyany.cn

PHP:  getcwd();
来源：http://jlo.zhixingplan.top

JS:   process.cwd()
来源：http://ygg.ehwqpu.com

TS:   process.cwd()
来源：http://kwv.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://omo.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://gtk.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://byh.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wfw.bbcook.cn

[M05] 设置退出码
来源：http://xfc.tanke756.top

Py:   sys.exit(1)
来源：http://zjr.yuxming.cn

PHP:  exit(1);
来源：http://qal.gogol.net.cn

JS:   process.exit(1)
来源：http://dgu.zhijiandao.cn

TS:   process.exit(1)
来源：http://atg.nanxuanxn.top

Java: System.exit(1)
来源：http://zom.aibaodan.cn

Go:   os.Exit(1)
来源：http://dtq.cdnleiting.top

Ruby: exit 1
来源：http://zim.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vvs.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://wbd.hesvh.cn

Py:   print("err", file=sys.stderr)
来源：http://wax.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ihg.fktsv.cn

JS:   console.error("err")
来源：http://ouk.fanxiaobao.xyz

TS:   console.error("err")
来源：http://qwj.kuanghao11.cn

Java: System.err.println("err")
来源：http://rai.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gmv.0kj1m.cn

Ruby: warn "err"
来源：http://edt.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://muh.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://qcc.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://rfv.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mzq.xziqi.cn

JS:   require.main === module
来源：http://sae.havefunace.top

TS:   require.main === module
来源：http://tdy.yongpay.top

Java: public static void main(String[] args)
来源：http://ila.quarkkingdee.top

Go:   func main()
来源：http://qfg.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://esw.yj20258.top

C#:   static void Main(string[] args)
来源：http://cmn.ivvv.top

[M08] 获取系统与运行时信息
来源：http://uca.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://awx.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://vrr.ppjwa.cn

JS:   process.platform;  process.version
来源：http://xnd.sxryk.cn

TS:   process.platform;  process.version
来源：http://mab.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qdr.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://adq.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fql.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iys.kuanghao11.cn

================================================================================
来源：http://uty.chenjidiqi.icu

N. 数据结构与算法
来源：http://ktm.fanxiaobao.xyz

================================================================================
来源：http://elf.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://wmp.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://ieb.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jof.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vxd.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cdj.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://orb.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://jsg.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lpr.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://iyr.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://hcv.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://cou.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rhb.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mxe.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oba.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://smw.316326.xyz

Go:   slices.Sort(arr)
来源：http://blt.gzhubu.top

Ruby: arr.sort
来源：http://hpv.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iur.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://zet.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dyy.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://hod.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmh.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ycl.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nmu.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pxx.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://egg.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yju.yfazqb.com

[N04] 斐波那契数列
来源：http://nde.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vnd.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rni.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pvr.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvd.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rby.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rtb.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://upr.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://roc.cucudq.cn

[N05] 最大公约数
来源：http://hbv.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://ern.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qzy.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aaw.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aal.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tfq.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cbd.hammf.cn

Ruby: a.gcd(b)
来源：http://gyo.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ajl.yuanzhike.top

[N06] 判断回文字符串
来源：http://ely.ydzc1.top

Py:   s == s[::-1]
来源：http://vln.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://iyn.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://huo.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://ovn.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cuf.wangdashe.top

Go:   // 双指针从两端比较
来源：http://avn.zhoulong.xyz

Ruby: s == s.reverse
来源：http://fjb.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jlu.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://mtl.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xhi.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vlo.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qgv.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://uqs.9152youxi.cn

Java: // 手写 HashMap
来源：http://puh.zhoulong.xyz

Go:   // 手写 map[int]int
来源：http://tgp.jinqigufen.top

Ruby: // 手写 Hash
来源：http://geb.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://kje.hnxiangtu.top

[N08] 生成全排列
来源：http://awy.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://osn.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://aes.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://zhl.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://fvv.hcnkem.com

Java: // 手写回溯递归
来源：http://gbo.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://kup.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://rmd.pycfn.com

C#:   // 手写回溯递归
来源：http://yqe.hnqzz.top

[N09] 栈与队列
来源：http://kuu.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cdl.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://avz.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ecw.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jgl.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://chb.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lib.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lqa.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lqn.hesvh.cn

[N10] 链表节点定义
来源：http://nrr.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dsw.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fsx.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qws.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://foh.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://ygg.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uyb.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ioj.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bmo.fengsongda.top

[N11] 二叉树中序遍历
来源：http://hvc.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mkc.svipenyu.cn

PHP:  // 手写递归函数
来源：http://hjd.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czh.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://umh.yfazqb.com

Java: // 手写递归
来源：http://sfj.zhixingplan.top

Go:   // 手写递归
来源：http://ene.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yao.sysykeji.top

C#:   // 手写递归
来源：http://fak.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ojh.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eut.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pym.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aye.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lpn.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jnn.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://art.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zhs.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wpi.c1oappe.top

================================================================================
来源：http://ecu.fengsongda.top

O. 并发与异步
来源：http://yxa.jinyuanbaomall.cn

================================================================================
来源：http://ank.fktsv.cn

[O01] 启动一个线程
来源：http://rfv.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zaf.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uez.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oxt.nwbrower.top

TS:   // 同 JS
来源：http://ubf.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://zac.zycfv.cn

Go:   go f()
来源：http://ehw.uphjek.com

Ruby: Thread.new { f }
来源：http://nom.cucudq.cn

C#:   Task.Run(() => F());
来源：http://ayv.sufxvd.cn

[O02] 使用线程池
来源：http://bov.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qrk.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://neb.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://ijx.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://cvw.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://qqq.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://noi.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ihy.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mtd.yuxming.cn

[O03] 加锁保护共享数据
来源：http://jdi.chenlongwang.top

Py:   with lock: shared += 1
来源：http://nth.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://ujy.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ecg.shzxlz.cn

TS:   // 同 JS
来源：http://nzp.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://efw.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wnl.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vtv.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://snc.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://vvd.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://gmo.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://irn.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://lte.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nlv.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rxf.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rjr.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cte.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://msr.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://tqd.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://zkf.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kin.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://ruo.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://xvl.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hln.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fsb.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://xtn.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://esr.c1oappe.top

[O06] 使用进程池
来源：http://yfn.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ykx.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jub.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://ybd.0kj1m.cn


<!-- 参考信息 -->