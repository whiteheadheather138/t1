代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://uae.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zjt.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vfz.zdbjq.cn

[L02] 发送 POST JSON
来源：http://jfq.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://xkv.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ipm.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfx.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xpb.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://emr.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zcr.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://szp.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vjo.bjfxy.top

[L03] 设置自定义请求头
来源：http://uav.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ejv.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kbl.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iot.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://moo.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://knv.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vvq.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dho.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hlp.zhiwuduotai.top

[L04] 设置超时
来源：http://eoo.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://ttg.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tsk.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mnl.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://itb.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vgv.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ibg.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rom.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zth.havefunace.top

[L05] 上传文件（multipart）
来源：http://pld.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fxg.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cxh.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lef.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://trk.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qaj.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tbw.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ian.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://feh.yfazqb.com

[L06] 解析响应为 JSON
来源：http://lom.9152youxi.cn

Py:   resp.json()
来源：http://lre.meibo888.top

PHP:  json_decode($body, true);
来源：http://tsn.ivvv.top

JS:   await resp.json()
来源：http://kia.316326.xyz

TS:   await resp.json()
来源：http://dky.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sgc.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bwd.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://gly.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lkz.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://edu.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iym.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ymj.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://qul.316326.xyz

TS:   resp.ok;  resp.status
来源：http://qex.zhixingplan.top

Java: resp.statusCode()
来源：http://mcp.quarkkingdee.top

Go:   resp.StatusCode
来源：http://qvy.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://tlt.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://mmn.hywenlv.cn

[L08] 并发请求多个地址
来源：http://yxv.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gii.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://hkn.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xam.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://btg.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wwl.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ups.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iuc.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vib.cashguo.top

================================================================================
来源：http://ktk.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://hlc.yonumen.top

================================================================================
来源：http://yqg.xylfe.cn

[M01] 读取命令行参数
来源：http://ddv.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://fyh.cheryme.top

PHP:  $argv;  $argc;
来源：http://bci.redwolf501.top

JS:   process.argv.slice(2)
来源：http://bfg.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://htm.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://htc.sxryk.cn

Go:   os.Args[1:]
来源：http://blo.zhaomingkeji.xyz

Ruby: ARGV
来源：http://ioy.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://det.zhijiandao.cn

[M02] 读取环境变量
来源：http://ids.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://qia.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dxi.vehdjk.com

JS:   process.env.HOME
来源：http://htj.vehdjk.com

TS:   process.env.HOME
来源：http://kvc.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://azq.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ynm.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://gdx.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fee.fzhhl.top

[M03] 执行外部命令
来源：http://usm.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zne.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ict.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wqy.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://avh.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pxr.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lkb.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://reh.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://eyd.havefunace.top

[M04] 获取当前工作目录
来源：http://yeu.fktsv.cn

Py:   os.getcwd()
来源：http://xrs.hongshengwenyu.top

PHP:  getcwd();
来源：http://snd.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://evp.zhengqikj.top

TS:   process.cwd()
来源：http://hfy.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://jay.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://qqf.andypj.xyz

Ruby: Dir.pwd
来源：http://fsw.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://eqq.zhengqikj.top

[M05] 设置退出码
来源：http://wye.yfazqb.com

Py:   sys.exit(1)
来源：http://lqh.daxiang520.top

PHP:  exit(1);
来源：http://qol.iojbl.cn

JS:   process.exit(1)
来源：http://bjz.guannengcc.top

TS:   process.exit(1)
来源：http://fjr.sufxvd.cn

Java: System.exit(1)
来源：http://ygg.52xcode.cn

Go:   os.Exit(1)
来源：http://bmh.hnxiangtu.top

Ruby: exit 1
来源：http://ehm.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sps.sxryk.cn

[M06] 向标准错误输出
来源：http://bte.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://wnf.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cdt.316326.xyz

JS:   console.error("err")
来源：http://roh.cucudq.cn

TS:   console.error("err")
来源：http://fja.chenlongwang.top

Java: System.err.println("err")
来源：http://ynd.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://igp.cdnleiting.top

Ruby: warn "err"
来源：http://rby.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://fsv.guannengcc.top

[M07] 判断是否为主入口
来源：http://ocb.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://owk.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xqf.ywan-chungtsiang.top

JS:   require.main === module
来源：http://ejt.feifeiyinyue.top

TS:   require.main === module
来源：http://gov.tianlin.xyz

Java: public static void main(String[] args)
来源：http://jkh.cqqwz.cn

Go:   func main()
来源：http://smk.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kuj.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://yog.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://zjc.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://odf.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://ghb.tianlin.xyz

JS:   process.platform;  process.version
来源：http://gba.fktsv.cn

TS:   process.platform;  process.version
来源：http://lpl.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wyf.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kfo.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qgt.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://udw.hywenlv.cn

================================================================================
来源：http://hgj.fehbvm.com

N. 数据结构与算法
来源：http://kfl.sjlbkw.cn

================================================================================
来源：http://psw.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://bbx.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://rlm.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uer.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llj.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gbt.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://edx.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://hse.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbt.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://sba.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cjl.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://gmn.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yuu.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ryt.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oxe.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zcb.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://ypa.xziqi.cn

Ruby: arr.sort
来源：http://jhl.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xod.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://bvu.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxt.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://rjd.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dvz.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gkv.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cph.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uni.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sdb.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://uvc.yuanzhike.top

[N04] 斐波那契数列
来源：http://rpl.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lex.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lmm.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vcl.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mmf.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hty.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sdv.bjfxy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yxp.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hgi.daxiang520.top

[N05] 最大公约数
来源：http://lzt.xinyue.icu

Py:   math.gcd(a, b)
来源：http://vvk.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xlq.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rrc.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aat.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yhe.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lum.hysaishi.cn

Ruby: a.gcd(b)
来源：http://div.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aqp.jlsjyb.cn

[N06] 判断回文字符串
来源：http://nsc.hesvh.cn

Py:   s == s[::-1]
来源：http://uww.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://dqt.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://sie.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://knu.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bou.meibo888.top

Go:   // 双指针从两端比较
来源：http://wxh.yuxming.cn

Ruby: s == s.reverse
来源：http://csf.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://sbr.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://jsw.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ckc.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eem.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jxu.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://izi.sjlbkw.cn

Java: // 手写 HashMap
来源：http://rjd.nwbrower.top

Go:   // 手写 map[int]int
来源：http://ixm.cheryme.top

Ruby: // 手写 Hash
来源：http://zdr.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://wyy.sxryk.cn

[N08] 生成全排列
来源：http://nlm.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://ghb.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://baz.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://flc.dashuyun.cn

TS:   // 手写回溯递归
来源：http://hsw.fzhhl.top

Java: // 手写回溯递归
来源：http://ndc.shuidangran.top

Go:   // 手写回溯递归
来源：http://ajj.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://fqq.haohaochexian.top

C#:   // 手写回溯递归
来源：http://hjn.yvedp.cn

[N09] 栈与队列
来源：http://tfl.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nww.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ogp.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fbr.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wga.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mxq.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dvg.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gad.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnu.jinqigfzy.top

[N10] 链表节点定义
来源：http://mqy.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vhy.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ati.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oby.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bgi.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://amq.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://cwi.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://psz.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oxm.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://xml.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yeh.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://kjf.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zac.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kdl.zhengqikj.top

Java: // 手写递归
来源：http://ipt.gogol.net.cn

Go:   // 手写递归
来源：http://aur.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rem.yuanzhike.top

C#:   // 手写递归
来源：http://kfu.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vur.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qkr.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://esa.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ihg.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zqp.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ywu.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bxh.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ska.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sts.feifeiyinyue.top

================================================================================
来源：http://yuv.cashguo.top

O. 并发与异步
来源：http://xkm.cqqwz.cn

================================================================================
来源：http://fsc.zhengqikj.top

[O01] 启动一个线程
来源：http://qbk.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dld.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sjm.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fml.aizwys.cn

TS:   // 同 JS
来源：http://xwk.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://kfg.yongpay.top

Go:   go f()
来源：http://sao.52xcode.cn

Ruby: Thread.new { f }
来源：http://cxp.shuidangran.top

C#:   Task.Run(() => F());
来源：http://jzt.hcnkem.com

[O02] 使用线程池
来源：http://cwh.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lmw.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lqo.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://lkw.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://ekt.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tie.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gku.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nbg.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bme.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://agk.chenzaomai.com

Py:   with lock: shared += 1
来源：http://dem.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://pfy.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jxi.shanyushiyangtech.top

TS:   // 同 JS
来源：http://rdy.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://wnc.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mrp.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://asn.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://wxh.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://isj.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://kwz.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rhz.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://pyb.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://auf.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lud.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bjt.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://mmn.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://zrh.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://ggl.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://lmr.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cyu.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://lgh.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://deq.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lzo.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tgs.yvedp.cn

Ruby: threads.map(&:join)
来源：http://iws.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qdl.wangshuangyany.cn


<!-- 参考信息 -->