代发 wailian999

Go:   encoding/gob
来源：http://kjq.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://hlu.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uua.dashuyun.cn

================================================================================
来源：http://gum.cdnleiting.top

L. 网络请求
来源：http://gnw.pycfn.com

================================================================================
来源：http://hxb.xuanzx.com

[L01] 发送 GET 请求
来源：http://jvs.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rsu.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://axa.tarul.cn

JS:   await fetch(url)
来源：http://dke.snrcjt.cn

TS:   await fetch(url)
来源：http://yyy.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tyc.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://csm.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xdw.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpk.c1oappe.top

[L02] 发送 POST JSON
来源：http://asl.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://cgp.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jbe.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iyc.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovv.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jxs.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mko.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pmh.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sip.yongpay.top

[L03] 设置自定义请求头
来源：http://mce.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aid.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gxb.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qds.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzl.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ibz.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xgh.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://byo.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iyz.smart0.xyz

[L04] 设置超时
来源：http://sbj.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://wkb.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ega.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mls.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ntb.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gtg.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rcy.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bnf.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://npd.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://wdc.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mhd.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ios.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nlc.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ryd.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wye.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ovn.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zst.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://saf.pycfn.com

[L06] 解析响应为 JSON
来源：http://fly.sufxvd.cn

Py:   resp.json()
来源：http://jns.yvedp.cn

PHP:  json_decode($body, true);
来源：http://qro.gogol.net.cn

JS:   await resp.json()
来源：http://duo.jinqigfzy.top

TS:   await resp.json()
来源：http://ncd.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tpg.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wcx.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://gqw.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uum.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://hvi.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yyo.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://unk.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://aex.ivvv.top

TS:   resp.ok;  resp.status
来源：http://kwq.sxryk.cn

Java: resp.statusCode()
来源：http://rpq.yj20258888.top

Go:   resp.StatusCode
来源：http://psz.guannengcc.top

Ruby: resp.code.to_i
来源：http://hqy.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://pxn.jianghu66.top

[L08] 并发请求多个地址
来源：http://ore.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fbd.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://xfd.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://efh.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fnq.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ysl.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rps.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oft.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://esm.bjfxy.top

================================================================================
来源：http://mdm.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://rmx.hysaishi.cn

================================================================================
来源：http://bzi.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://pjf.tarul.cn

Py:   sys.argv[1:]
来源：http://dnw.nwbrower.top

PHP:  $argv;  $argc;
来源：http://gdj.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://ehs.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://ozv.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://ser.aizwys.cn

Go:   os.Args[1:]
来源：http://wwa.xuetiantiany.cn

Ruby: ARGV
来源：http://bhp.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://wdl.52xcode.cn

[M02] 读取环境变量
来源：http://aci.yonumen.top

Py:   os.environ.get("HOME")
来源：http://trg.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xcg.zhoulong.xyz

JS:   process.env.HOME
来源：http://qpj.dianchejie.cn

TS:   process.env.HOME
来源：http://lnj.nwbrower.top

Java: System.getenv("HOME")
来源：http://yac.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rai.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://rqb.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yan.feifeiyinyue.top

[M03] 执行外部命令
来源：http://gto.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://skg.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xhn.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jtz.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qlj.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bri.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://crc.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tui.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://tvs.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://deg.daria6918.cn

Py:   os.getcwd()
来源：http://xav.zdqjudy.top

PHP:  getcwd();
来源：http://hns.zhongyouzk.top

JS:   process.cwd()
来源：http://kau.nwbrower.top

TS:   process.cwd()
来源：http://umf.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://qua.dashuyun.cn

Go:   os.Getwd()
来源：http://lvg.nanxuanxn.top

Ruby: Dir.pwd
来源：http://eqx.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kpd.sufxvd.cn

[M05] 设置退出码
来源：http://lec.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://zbp.smart0.xyz

PHP:  exit(1);
来源：http://luz.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://hjc.daxiang520.top

TS:   process.exit(1)
来源：http://pvy.xinyue.icu

Java: System.exit(1)
来源：http://utu.chenzaomai.com

Go:   os.Exit(1)
来源：http://kec.0kj1m.cn

Ruby: exit 1
来源：http://oar.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wls.sxryk.cn

[M06] 向标准错误输出
来源：http://uns.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://ejq.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gap.nanxinkj.top

JS:   console.error("err")
来源：http://zuh.hongshengwenyu.top

TS:   console.error("err")
来源：http://rhr.svipenyu.cn

Java: System.err.println("err")
来源：http://bre.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://krh.cdnleiting.top

Ruby: warn "err"
来源：http://hcz.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://yrx.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://jmr.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://yxz.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uud.yuanzhike.top

JS:   require.main === module
来源：http://rxi.ivvv.top

TS:   require.main === module
来源：http://chv.xinyue.icu

Java: public static void main(String[] args)
来源：http://wxs.yanxiufei.cn

Go:   func main()
来源：http://ihd.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iui.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://fvf.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://bwc.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://pop.fengsongda.top

PHP:  PHP_OS;  phpversion();
来源：http://tzy.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://pbl.chenlongwang.top

TS:   process.platform;  process.version
来源：http://ezg.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yfw.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wyu.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nso.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rwk.316326.xyz

================================================================================
来源：http://qsk.yanxiufei.cn

N. 数据结构与算法
来源：http://imc.fzhhl.top

================================================================================
来源：http://lqg.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://guk.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pry.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gup.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pps.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywl.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uap.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://woq.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wba.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vna.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://fqa.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://yei.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fvs.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mme.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eui.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kso.wangdashe.top

Go:   slices.Sort(arr)
来源：http://tir.pycfn.com

Ruby: arr.sort
来源：http://gqq.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fhg.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://ykb.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uib.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://paj.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cxj.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lfs.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yeo.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://urz.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kyc.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xju.zdbjq.cn

[N04] 斐波那契数列
来源：http://dhz.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hut.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ynq.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cev.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvo.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wuj.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qlw.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pox.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://brb.shzxlz.cn

[N05] 最大公约数
来源：http://jia.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://gmc.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tyr.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wmj.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wzl.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bgu.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uxy.yj20258888.top

Ruby: a.gcd(b)
来源：http://pib.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zar.hfpthk.cn

[N06] 判断回文字符串
来源：http://fzf.jqgufenzy.top

Py:   s == s[::-1]
来源：http://zpn.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://aty.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://xik.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://tqj.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ggl.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://kbj.fktsv.cn

Ruby: s == s.reverse
来源：http://vjs.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://cdx.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://zgt.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ogl.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gus.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://whp.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://lck.bjfxy.top

Java: // 手写 HashMap
来源：http://ooy.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://box.jyoumei.cn

Ruby: // 手写 Hash
来源：http://oiq.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://neo.meibo888.top

[N08] 生成全排列
来源：http://vqr.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://uiy.zdqjudy.top

PHP:  // 手写递归交换
来源：http://jno.yvedp.cn

JS:   // 手写回溯递归
来源：http://zjq.yj202588.top

TS:   // 手写回溯递归
来源：http://dbl.jiagoushi.top

Java: // 手写回溯递归
来源：http://tej.ydzc1.top

Go:   // 手写回溯递归
来源：http://ump.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://zfj.jiagoushi.top

C#:   // 手写回溯递归
来源：http://ccx.hesvh.cn

[N09] 栈与队列
来源：http://ljd.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fjn.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xcr.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mft.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aps.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://azl.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vah.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ojx.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://osi.yfazqb.com

[N10] 链表节点定义
来源：http://ojm.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gjp.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zyr.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lyt.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ewj.yvedp.cn

Java: class Node { int v; Node next; }
来源：http://hhp.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://wcm.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tly.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ahe.hammf.cn

[N11] 二叉树中序遍历
来源：http://bqy.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dkq.feifeiyinyue.top

PHP:  // 手写递归函数
来源：http://voy.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nen.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tzc.jqgfzy.top

Java: // 手写递归
来源：http://rew.fzhhl.top

Go:   // 手写递归
来源：http://vcb.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oae.smart0.xyz

C#:   // 手写递归
来源：http://ktl.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pge.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://neq.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://agi.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ega.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dgg.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qhr.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nob.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lqt.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ylo.guowangkeji.top

================================================================================
来源：http://spx.cheryme.top

O. 并发与异步
来源：http://dtb.fzhhl.top

================================================================================
来源：http://lva.sysykeji.top

[O01] 启动一个线程
来源：http://qmb.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qld.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://agv.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wgb.epnwcf.com

TS:   // 同 JS
来源：http://zrp.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://dto.yueranfly.top

Go:   go f()
来源：http://snf.xinyue.icu

Ruby: Thread.new { f }
来源：http://rhg.yuxming.cn

C#:   Task.Run(() => F());
来源：http://xma.yuanzhike.top

[O02] 使用线程池
来源：http://dto.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bjo.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hep.yj20258.top

JS:   // worker_threads 线程池
来源：http://wky.havefunace.top

TS:   // worker_threads 线程池
来源：http://mku.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://ejd.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fgp.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mds.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rmi.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://cfx.sufxvd.cn

Py:   with lock: shared += 1
来源：http://odr.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://hey.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zxo.cheryme.top

TS:   // 同 JS
来源：http://jep.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://mol.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gay.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rei.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://yay.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://wwo.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://yeo.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cve.birdmap.top

JS:   async function f() { await g(); }
来源：http://hms.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qrz.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zhq.tian-w.cn


<!-- 参考信息 -->