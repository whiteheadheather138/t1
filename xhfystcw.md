代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://gmk.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://siq.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yjk.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://efy.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ldo.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xoo.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jai.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qxw.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://bea.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sjx.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zmn.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mtu.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zmn.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ffk.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qpv.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bkv.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cpm.jiagoushi.top

[L04] 设置超时
来源：http://iom.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://zck.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uba.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hgn.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nhc.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jwk.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gcj.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rbi.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hxh.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://mno.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://grm.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rcz.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kna.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dxo.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://olu.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lbf.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://juj.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://doe.gzhubu.top

[L06] 解析响应为 JSON
来源：http://irm.hcnkem.com

Py:   resp.json()
来源：http://kyb.fengsongda.top

PHP:  json_decode($body, true);
来源：http://bwd.jiagoushi.top

JS:   await resp.json()
来源：http://vli.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://oga.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://opg.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jfd.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://wnb.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baf.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://dkx.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pwf.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uaz.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://hsv.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://hyt.svipenyu.cn

Java: resp.statusCode()
来源：http://zyt.haohaochexian.top

Go:   resp.StatusCode
来源：http://gad.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://wnf.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://evk.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://zdw.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zki.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://mpa.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swa.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgi.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eso.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nog.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://voz.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xqx.sjlbkw.cn

================================================================================
来源：http://sbh.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://cwe.zhiwuduotai.top

================================================================================
来源：http://fvx.yangfankeji.com

[M01] 读取命令行参数
来源：http://jhx.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://aor.tian-w.cn

PHP:  $argv;  $argc;
来源：http://nmy.yj20258.top

JS:   process.argv.slice(2)
来源：http://dyk.havefunace.top

TS:   process.argv.slice(2)
来源：http://vzf.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://ihi.dianchejie.cn

Go:   os.Args[1:]
来源：http://uex.dashuyun.cn

Ruby: ARGV
来源：http://afv.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://jks.chenlongwang.top

[M02] 读取环境变量
来源：http://ydz.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://kos.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vjo.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://ldc.nanxinkj.top

TS:   process.env.HOME
来源：http://uie.sweek.top

Java: System.getenv("HOME")
来源：http://wla.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jqz.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://sew.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qtd.vehdjk.com

[M03] 执行外部命令
来源：http://llc.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pgh.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://glf.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ptk.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jiu.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://itn.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kup.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://tde.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://dmb.dianchejie.cn

[M04] 获取当前工作目录
来源：http://uap.jiagoushi.top

Py:   os.getcwd()
来源：http://udd.uphjek.com

PHP:  getcwd();
来源：http://kry.bbcook.cn

JS:   process.cwd()
来源：http://hed.shanyushiyangtech.top

TS:   process.cwd()
来源：http://vkc.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cgc.sxryk.cn

Go:   os.Getwd()
来源：http://nsa.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://gls.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://fxo.iojbl.cn

[M05] 设置退出码
来源：http://ont.guowangkeji.top

Py:   sys.exit(1)
来源：http://vwf.xuanzx.com

PHP:  exit(1);
来源：http://dog.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://upp.xuanzx.com

TS:   process.exit(1)
来源：http://mbx.hywenlv.cn

Java: System.exit(1)
来源：http://gih.shzxlz.cn

Go:   os.Exit(1)
来源：http://uno.guowangkeji.top

Ruby: exit 1
来源：http://hea.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xcl.nwbrower.top

[M06] 向标准错误输出
来源：http://utt.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://lej.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pqf.yonumen.top

JS:   console.error("err")
来源：http://xol.epnwcf.com

TS:   console.error("err")
来源：http://ldc.aizwys.cn

Java: System.err.println("err")
来源：http://hbd.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lac.gotoacloud.top

Ruby: warn "err"
来源：http://evq.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://waz.xziqi.cn

[M07] 判断是否为主入口
来源：http://dkx.hammf.cn

Py:   if __name__ == "__main__":
来源：http://ubh.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gxo.vehdjk.com

JS:   require.main === module
来源：http://mbp.jiagoushi.top

TS:   require.main === module
来源：http://mik.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://dzv.ehwqpu.com

Go:   func main()
来源：http://udo.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nds.ybcxt.top

C#:   static void Main(string[] args)
来源：http://kkj.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://gnl.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://her.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://veo.iojbl.cn

JS:   process.platform;  process.version
来源：http://mut.guannengcc.top

TS:   process.platform;  process.version
来源：http://mmz.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kaq.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qbk.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yok.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ere.shangyingyoupin.top

================================================================================
来源：http://xto.yj202588.top

N. 数据结构与算法
来源：http://tco.shangyingyoupin.top

================================================================================
来源：http://hod.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://tpg.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://gfv.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jpy.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sut.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://coc.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://neo.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://gco.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zbl.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://fwb.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://cla.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://gxw.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uvj.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bpw.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zbm.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://als.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://nuj.ivvv.top

Ruby: arr.sort
来源：http://dhw.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kbu.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://lcr.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kqu.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://zrh.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpw.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uoe.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://shh.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pay.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://krj.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://isk.nanxinkj.top

[N04] 斐波那契数列
来源：http://adt.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pss.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mlj.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkr.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyr.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gna.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cyo.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ohm.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xoj.fanxiaobao.xyz

[N05] 最大公约数
来源：http://mgx.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://efx.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oje.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvx.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gcv.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://peo.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://anv.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://vga.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uey.uphjek.com

[N06] 判断回文字符串
来源：http://ueh.haohaochexian.top

Py:   s == s[::-1]
来源：http://mdy.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://cle.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://bcl.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://kbm.ctjpmb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ajg.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://oia.hesvh.cn

Ruby: s == s.reverse
来源：http://ugg.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://svi.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://dks.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kjs.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ngz.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mfu.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://hkx.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://fxq.yvedp.cn

Go:   // 手写 map[int]int
来源：http://elp.c1oappe.top

Ruby: // 手写 Hash
来源：http://jxs.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://qrl.yongpay.top

[N08] 生成全排列
来源：http://blx.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://nea.yuanzhike.top

PHP:  // 手写递归交换
来源：http://hkp.gzhubu.top

JS:   // 手写回溯递归
来源：http://lxz.iojbl.cn

TS:   // 手写回溯递归
来源：http://bxv.smart0.xyz

Java: // 手写回溯递归
来源：http://hxg.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://xxs.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://dfm.svipenyu.cn

C#:   // 手写回溯递归
来源：http://eci.shangyingyoupin.top

[N09] 栈与队列
来源：http://eto.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://knw.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pis.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vtj.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xhr.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rzp.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xoo.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vay.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cws.tanke756.top

[N10] 链表节点定义
来源：http://xgl.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qyy.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bca.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qye.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qqn.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://xli.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://kjp.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tvk.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://rty.xziqi.cn

[N11] 二叉树中序遍历
来源：http://pti.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eod.tarul.cn

PHP:  // 手写递归函数
来源：http://tnv.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ofx.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jot.jlsjyb.cn

Java: // 手写递归
来源：http://ppm.hnqzz.top

Go:   // 手写递归
来源：http://zqz.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gvs.mhx1999.top

C#:   // 手写递归
来源：http://zfd.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nkx.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://udq.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://luy.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmz.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://csz.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sxm.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fyl.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tlc.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wnx.yongpay.top

================================================================================
来源：http://gmq.ywan-chungtsiang.top

O. 并发与异步
来源：http://tkw.xuetiantiany.cn

================================================================================
来源：http://vpi.316326.xyz

[O01] 启动一个线程
来源：http://odi.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hnc.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wkl.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iyz.0kj1m.cn

TS:   // 同 JS
来源：http://paj.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://cky.fengsongda.top

Go:   go f()
来源：http://ixz.jiagoushi.top

Ruby: Thread.new { f }
来源：http://slu.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://bqo.pycfn.com

[O02] 使用线程池
来源：http://fkc.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://itz.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yhu.fehbvm.com

JS:   // worker_threads 线程池
来源：http://pjd.daxiang520.top

TS:   // worker_threads 线程池
来源：http://hkd.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://pyn.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzu.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ifx.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://amo.xylfe.cn

[O03] 加锁保护共享数据
来源：http://ttt.andypj.xyz

Py:   with lock: shared += 1
来源：http://itl.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://ywe.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cwv.daria6918.cn

TS:   // 同 JS
来源：http://cgt.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://ral.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bvs.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://buz.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://yyq.yj20258.top

[O04] 定义异步函数并等待
来源：http://bdj.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://yus.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pyf.fehbvm.com

JS:   async function f() { await g(); }
来源：http://mpa.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://usg.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://smj.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mxj.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://cav.yj20258.top

C#:   async Task F() { await G(); }
来源：http://wes.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://iuy.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://cty.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uub.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://ecp.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://cze.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fza.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gnr.vehdjk.com

Ruby: threads.map(&:join)
来源：http://gwb.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fos.yj202588.top

[O06] 使用进程池
来源：http://xyb.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://car.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fpd.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://arm.nwbrower.top


<!-- 参考信息 -->