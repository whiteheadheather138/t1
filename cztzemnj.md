代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rel.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vmj.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vch.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izl.yuxming.cn

[L03] 设置自定义请求头
来源：http://ybm.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gwe.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xne.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fnh.tian-w.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gdf.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zsy.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wft.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xfg.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iur.yfazqb.com

[L04] 设置超时
来源：http://riu.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://ocz.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ubr.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvh.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://efa.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tlb.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dvm.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://smx.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mzn.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://quq.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cza.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://awc.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gro.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cgc.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bnt.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xlq.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mbk.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsq.xylfe.cn

[L06] 解析响应为 JSON
来源：http://weg.wangshuangyany.cn

Py:   resp.json()
来源：http://mme.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://lvf.xinyue.icu

JS:   await resp.json()
来源：http://sba.9152youxi.cn

TS:   await resp.json()
来源：http://wcb.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ksp.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fmn.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://jxp.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbu.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://eev.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jpa.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xvi.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://yzi.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://zzf.yuanzhike.top

Java: resp.statusCode()
来源：http://mli.kuanghao11.cn

Go:   resp.StatusCode
来源：http://cds.bbcook.cn

Ruby: resp.code.to_i
来源：http://lba.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://rcq.svipenyu.cn

[L08] 并发请求多个地址
来源：http://cgd.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qmp.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://yek.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://but.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jmm.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eth.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovl.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://feo.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hwm.svipenyu.cn

================================================================================
来源：http://rlh.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://lcl.guannengcc.top

================================================================================
来源：http://ama.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://kzr.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://ebg.yfazqb.com

PHP:  $argv;  $argc;
来源：http://jnl.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://pqq.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://ikl.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://pur.wangdashe.top

Go:   os.Args[1:]
来源：http://ckj.hammf.cn

Ruby: ARGV
来源：http://yse.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://shm.hnqzz.top

[M02] 读取环境变量
来源：http://fmz.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://alj.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zfp.chenjidiqi.icu

JS:   process.env.HOME
来源：http://apn.iojbl.cn

TS:   process.env.HOME
来源：http://giw.andypj.xyz

Java: System.getenv("HOME")
来源：http://boy.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zqo.nwbrower.top

Ruby: ENV["HOME"]
来源：http://kyq.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zlf.zhengqikj.top

[M03] 执行外部命令
来源：http://xbj.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bla.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zed.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bex.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hgk.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ixo.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xzq.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://utj.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://pmb.svipenyu.cn

[M04] 获取当前工作目录
来源：http://qcv.sysykeji.top

Py:   os.getcwd()
来源：http://ted.daxiang520.top

PHP:  getcwd();
来源：http://abc.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://nrz.vehdjk.com

TS:   process.cwd()
来源：http://ydh.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://gdd.ydjk.org.cn

Go:   os.Getwd()
来源：http://nqa.ppjwa.cn

Ruby: Dir.pwd
来源：http://lig.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://enk.redwolf501.top

[M05] 设置退出码
来源：http://tow.haohaochexian.top

Py:   sys.exit(1)
来源：http://vqh.jinqigfzy.top

PHP:  exit(1);
来源：http://nlp.tarul.cn

JS:   process.exit(1)
来源：http://fyl.hnxiangtu.top

TS:   process.exit(1)
来源：http://gyo.zycfv.cn

Java: System.exit(1)
来源：http://run.ydjk.org.cn

Go:   os.Exit(1)
来源：http://xvw.uphjek.com

Ruby: exit 1
来源：http://usk.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cmp.yueranfly.top

[M06] 向标准错误输出
来源：http://wme.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://ukv.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gll.gzhubu.top

JS:   console.error("err")
来源：http://sbw.yanxiufei.cn

TS:   console.error("err")
来源：http://bbl.meibo888.top

Java: System.err.println("err")
来源：http://mzs.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://htj.yonumen.top

Ruby: warn "err"
来源：http://ndo.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://fmh.gotoacloud.top

[M07] 判断是否为主入口
来源：http://cod.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://esk.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oou.zhaomingkeji.xyz

JS:   require.main === module
来源：http://wtr.dianchejie.cn

TS:   require.main === module
来源：http://ird.0kj1m.cn

Java: public static void main(String[] args)
来源：http://vfm.hcnkem.com

Go:   func main()
来源：http://prw.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xmt.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://vht.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://une.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://sqf.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://sep.dashuyun.cn

JS:   process.platform;  process.version
来源：http://toc.nanxinkj.top

TS:   process.platform;  process.version
来源：http://hdq.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rya.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://atk.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pqe.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://enz.jiagoushi.top

================================================================================
来源：http://trj.pengpengdd.cyou

N. 数据结构与算法
来源：http://jyo.yuanzhike.top

================================================================================
来源：http://exa.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://flz.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://fcz.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xnt.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://omo.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://emo.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://jvv.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://wdt.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nxv.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://det.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://lvb.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://qkd.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qir.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ebm.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sko.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qwz.ybcxt.top

Go:   slices.Sort(arr)
来源：http://tji.hysaishi.cn

Ruby: arr.sort
来源：http://yab.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://gsu.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://uta.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qqn.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://jvj.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxn.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hhn.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://soz.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rjp.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gew.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://hob.sysykeji.top

[N04] 斐波那契数列
来源：http://dgb.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qem.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qvt.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fjp.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pvx.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kuv.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oys.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://plk.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vir.hywenlv.cn

[N05] 最大公约数
来源：http://vhp.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://yfa.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://njs.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://poq.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sjn.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kiz.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tad.tanke756.top

Ruby: a.gcd(b)
来源：http://wae.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://htj.cucudq.cn

[N06] 判断回文字符串
来源：http://tzw.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://iwm.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://jju.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://myr.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://sww.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xcz.hcnkem.com

Go:   // 双指针从两端比较
来源：http://cvv.sufxvd.cn

Ruby: s == s.reverse
来源：http://qae.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cce.birdmap.top

[N07] 两数之和（返回下标）
来源：http://its.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ovu.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yad.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://knt.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://rtw.ydzc1.top

Java: // 手写 HashMap
来源：http://qoz.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://myo.cucudq.cn

Ruby: // 手写 Hash
来源：http://ryq.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://czb.jinqigfzy.top

[N08] 生成全排列
来源：http://muq.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://oeb.guannengcc.top

PHP:  // 手写递归交换
来源：http://oqz.fengsongda.top

JS:   // 手写回溯递归
来源：http://xtm.birdmap.top

TS:   // 手写回溯递归
来源：http://zgd.vqdsnc.cn

Java: // 手写回溯递归
来源：http://dvv.yuanzhike.top

Go:   // 手写回溯递归
来源：http://nnz.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://meo.iojbl.cn

C#:   // 手写回溯递归
来源：http://trl.hcnkem.com

[N09] 栈与队列
来源：http://ezc.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iqr.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fhx.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cug.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bkq.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pzf.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ish.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rye.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sel.daria6918.cn

[N10] 链表节点定义
来源：http://ylm.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://muq.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mqu.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://klr.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lfn.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://uni.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://hdm.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lel.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://int.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://uww.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://knu.yj202588.top

PHP:  // 手写递归函数
来源：http://gud.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fym.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ldx.zhixingplan.top

Java: // 手写递归
来源：http://bkt.yongpay.top

Go:   // 手写递归
来源：http://jlc.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://znb.jiagoushi.top

C#:   // 手写递归
来源：http://aex.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://umq.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nmp.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ujd.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lji.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dkv.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xoo.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pbb.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://neb.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eeb.haohaochexian.top

================================================================================
来源：http://unk.aibaodan.cn

O. 并发与异步
来源：http://ugj.bjfxy.top

================================================================================
来源：http://vtp.chenjidiqi.icu

[O01] 启动一个线程
来源：http://tnu.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zex.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uke.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bso.hesvh.cn

TS:   // 同 JS
来源：http://iek.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://jrk.pycfn.com

Go:   go f()
来源：http://eht.ppjwa.cn

Ruby: Thread.new { f }
来源：http://vxr.fengsongda.top

C#:   Task.Run(() => F());
来源：http://urt.jlsjyb.cn

[O02] 使用线程池
来源：http://ywl.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ggr.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lae.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://ryk.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://dby.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rzb.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hon.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://glw.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://usz.tanke756.top

[O03] 加锁保护共享数据
来源：http://vbs.yfazqb.com

Py:   with lock: shared += 1
来源：http://zkj.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://rza.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sqn.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://vdh.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://lwf.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nfz.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://gth.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://puw.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://enu.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://pre.pycfn.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cgi.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://oqm.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tuy.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gbh.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nun.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://qqe.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://nfx.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://pnw.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://ygf.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qbj.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://xan.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://few.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://msq.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zsk.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://vwp.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vio.zhoulong.xyz

[O06] 使用进程池
来源：http://qeo.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qlg.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kbu.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://jiw.uphjek.com

TS:   // child_process / cluster 模块
来源：http://byl.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://min.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://czb.daria6918.cn

Ruby: // fork 块
来源：http://igf.yj202588.top


<!-- 参考信息 -->