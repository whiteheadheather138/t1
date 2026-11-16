代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://txx.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dvr.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yin.vehdjk.com

[L02] 发送 POST JSON
来源：http://cqt.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xyg.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qik.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mro.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cny.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yfj.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dks.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bsv.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lgz.andypj.xyz

[L03] 设置自定义请求头
来源：http://cjq.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ytl.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jsv.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ady.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vhf.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://inz.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lxf.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jqd.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bxs.redwolf501.top

[L04] 设置超时
来源：http://ewp.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://cas.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ffo.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjs.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://agl.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://koy.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ouw.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ygq.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mtk.ivvv.top

[L05] 上传文件（multipart）
来源：http://rkx.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ije.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ynx.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nbk.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://klp.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sgz.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sax.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yzx.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pew.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://ths.zhengqikj.top

Py:   resp.json()
来源：http://lfa.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://qwo.jiagoushi.top

JS:   await resp.json()
来源：http://wyd.tanke756.top

TS:   await resp.json()
来源：http://jpg.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://smw.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fmf.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://wsb.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bkp.zycfv.cn

[L07] 处理 HTTP 状态码
来源：http://mwq.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://roy.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ovm.cheryme.top

JS:   resp.ok;  resp.status
来源：http://jbl.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://brg.ctjpmb.com

Java: resp.statusCode()
来源：http://trr.c1oappe.top

Go:   resp.StatusCode
来源：http://ufz.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://rwb.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://ahx.yueranfly.top

[L08] 并发请求多个地址
来源：http://xrw.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lgg.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://yjx.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dbr.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnf.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uph.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nuf.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ruo.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kfy.ywan-chungtsiang.top

================================================================================
来源：http://qna.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://gvw.aibaodan.cn

================================================================================
来源：http://zvp.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://viu.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://jdm.c1oappe.top

PHP:  $argv;  $argc;
来源：http://mgv.vehdjk.com

JS:   process.argv.slice(2)
来源：http://tdg.birdmap.top

TS:   process.argv.slice(2)
来源：http://hyx.yj20258.top

Java: args 数组（main 方法参数）
来源：http://yhm.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://fse.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://kxq.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://hnf.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://gnq.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://pzt.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wex.ehwqpu.com

JS:   process.env.HOME
来源：http://rkq.jianghu66.top

TS:   process.env.HOME
来源：http://prf.ydzc1.top

Java: System.getenv("HOME")
来源：http://ljr.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dsh.nwbrower.top

Ruby: ENV["HOME"]
来源：http://wkc.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmq.hnqzz.top

[M03] 执行外部命令
来源：http://fsr.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ldu.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kvf.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vrg.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jgi.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nwp.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fzp.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hbd.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://ewr.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://imm.zhongyouzk.top

Py:   os.getcwd()
来源：http://eyh.yvedp.cn

PHP:  getcwd();
来源：http://rbs.wangdashe.top

JS:   process.cwd()
来源：http://hai.cdnleiting.top

TS:   process.cwd()
来源：http://cch.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://pvi.zhoulong.xyz

Go:   os.Getwd()
来源：http://qal.cdnleiting.top

Ruby: Dir.pwd
来源：http://lel.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kng.aibaodan.cn

[M05] 设置退出码
来源：http://yui.zycfv.cn

Py:   sys.exit(1)
来源：http://hbk.pengpengdd.cyou

PHP:  exit(1);
来源：http://zfp.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://ehc.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://mpp.c1oappe.top

Java: System.exit(1)
来源：http://qrx.fzhhl.top

Go:   os.Exit(1)
来源：http://see.hcnkem.com

Ruby: exit 1
来源：http://okv.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lqz.dianchejie.cn

[M06] 向标准错误输出
来源：http://gea.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://lln.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ucl.ydzc1.top

JS:   console.error("err")
来源：http://yon.sysykeji.top

TS:   console.error("err")
来源：http://qex.birdmap.top

Java: System.err.println("err")
来源：http://xlc.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://emc.snrcjt.cn

Ruby: warn "err"
来源：http://dux.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://zae.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://hwp.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://gfj.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dvp.jianghu66.top

JS:   require.main === module
来源：http://zqf.zhixingplan.top

TS:   require.main === module
来源：http://wrv.tanke756.top

Java: public static void main(String[] args)
来源：http://nkr.gzhubu.top

Go:   func main()
来源：http://tff.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zik.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://jwq.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://otl.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://qno.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://zxd.epnwcf.com

JS:   process.platform;  process.version
来源：http://igv.hywenlv.cn

TS:   process.platform;  process.version
来源：http://rqq.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uny.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tdh.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fgi.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lyg.nanxuanxn.top

================================================================================
来源：http://llz.gzhubu.top

N. 数据结构与算法
来源：http://ylh.jinqigufen.top

================================================================================
来源：http://unl.yonumen.top

[N01] 二分查找（有序数组）
来源：http://ext.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://urk.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gka.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ydx.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uur.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://swd.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://tta.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kyd.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://adv.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://phy.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://eud.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sez.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://osb.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tmt.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wcm.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://klo.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://ale.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lga.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://vqy.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rvr.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://jdk.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjr.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vti.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mwo.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jjh.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gvg.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://tgi.yvedp.cn

[N04] 斐波那契数列
来源：http://lrw.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcj.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xyu.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxr.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vrr.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ras.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xrq.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jdh.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uve.dianchejie.cn

[N05] 最大公约数
来源：http://qdb.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://lru.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://orn.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcj.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qeu.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ekk.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zbh.guannengcc.top

Ruby: a.gcd(b)
来源：http://zyy.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mmf.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://vep.zhoulong.xyz

Py:   s == s[::-1]
来源：http://nne.xuanzx.com

PHP:  $s === strrev($s);
来源：http://tgs.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://uef.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://ysb.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ylm.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://mvh.zdbjq.cn

Ruby: s == s.reverse
来源：http://qua.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://acy.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://pol.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mkr.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gqs.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hfn.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://vjb.nanxuanxn.top

Java: // 手写 HashMap
来源：http://tlu.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://jvj.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://rvo.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://ywx.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://qxz.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://tha.smart0.xyz

PHP:  // 手写递归交换
来源：http://hvb.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://sqh.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://jiz.jlsjyb.cn

Java: // 手写回溯递归
来源：http://frq.hammf.cn

Go:   // 手写回溯递归
来源：http://xtf.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://dgg.yvedp.cn

C#:   // 手写回溯递归
来源：http://fki.aibaodan.cn

[N09] 栈与队列
来源：http://xwi.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qyd.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yqq.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hrz.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uzw.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gta.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qsp.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bjl.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hol.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://ywd.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xhp.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wnl.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ojo.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://krc.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://pmj.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://qof.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hmv.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://xqs.52xcode.cn

[N11] 二叉树中序遍历
来源：http://ybk.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vdj.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://jfv.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://new.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ywj.sweek.top

Java: // 手写递归
来源：http://gwu.hesvh.cn

Go:   // 手写递归
来源：http://zll.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://axg.xziqi.cn

C#:   // 手写递归
来源：http://pfl.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yrw.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mfo.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://scg.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dkg.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdk.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eyu.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yfi.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tle.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pfu.ywan-chungtsiang.top

================================================================================
来源：http://lsi.chenlongwang.top

O. 并发与异步
来源：http://kqh.vehdjk.com

================================================================================
来源：http://ruk.nanxuanxn.top

[O01] 启动一个线程
来源：http://gqo.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zpl.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rcy.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://syg.jqgfzy.top

TS:   // 同 JS
来源：http://xnk.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://ryb.fehbvm.com

Go:   go f()
来源：http://uav.ppjwa.cn

Ruby: Thread.new { f }
来源：http://nvg.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://uld.bbcook.cn

[O02] 使用线程池
来源：http://cac.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oqb.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://opa.yfazqb.com

JS:   // worker_threads 线程池
来源：http://zoe.bjfxy.top

TS:   // worker_threads 线程池
来源：http://eqy.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://ldh.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hly.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vgd.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cfs.yj20258888.top

[O03] 加锁保护共享数据
来源：http://fep.guowangkeji.top

Py:   with lock: shared += 1
来源：http://hse.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://qsz.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yht.fktsv.cn

TS:   // 同 JS
来源：http://foa.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://ema.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mto.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zlz.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://fxr.birdmap.top

[O04] 定义异步函数并等待
来源：http://ejw.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://kze.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vyx.yongpay.top

JS:   async function f() { await g(); }
来源：http://pum.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://emw.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://unk.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ljg.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://azk.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://brk.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://cqr.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://wql.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qij.yonumen.top

JS:   await Promise.all(tasks)
来源：http://lfv.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://ukw.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pae.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ibj.gzhubu.top

Ruby: threads.map(&:join)
来源：http://mzo.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pnv.guannengcc.top


<!-- 参考信息 -->