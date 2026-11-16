代发 wailian999

L. 网络请求
来源：http://alh.shanyushiyangkeji.top

================================================================================
来源：http://sgs.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://pnz.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://myk.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://prq.nanxinkj.top

JS:   await fetch(url)
来源：http://gxd.fktsv.cn

TS:   await fetch(url)
来源：http://wcv.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://imb.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://dit.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ouu.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://miq.cqqwz.cn

[L02] 发送 POST JSON
来源：http://wkd.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://krs.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bhe.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://abj.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xrb.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vrz.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mqe.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ivn.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mxi.wangdashe.top

[L03] 设置自定义请求头
来源：http://xuc.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://thp.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bqm.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xup.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uuh.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hkr.yueranfly.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wzy.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rtd.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jkl.birdmap.top

[L04] 设置超时
来源：http://noy.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://fzs.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jxj.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://umg.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxs.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pyb.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nuj.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yen.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://etn.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://hfi.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bjy.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qnt.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ezs.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nmd.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mtu.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bjc.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://otg.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ibn.xziqi.cn

[L06] 解析响应为 JSON
来源：http://tbq.xylfe.cn

Py:   resp.json()
来源：http://yxk.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://ysh.bbcook.cn

JS:   await resp.json()
来源：http://lpc.andypj.xyz

TS:   await resp.json()
来源：http://vhq.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gfa.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://irh.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://vjt.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lco.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://ase.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hol.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uvh.uphjek.com

JS:   resp.ok;  resp.status
来源：http://gvu.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://cfe.dianchejie.cn

Java: resp.statusCode()
来源：http://kez.zhoulong.xyz

Go:   resp.StatusCode
来源：http://ncy.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://wlh.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://dyj.nanxinkj.top

[L08] 并发请求多个地址
来源：http://gej.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dmi.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://uis.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oea.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byn.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kww.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ccc.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://leg.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hbg.gotoacloud.top

================================================================================
来源：http://kki.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://hib.9152youxi.cn

================================================================================
来源：http://bju.nanxinkj.top

[M01] 读取命令行参数
来源：http://bge.tanke756.top

Py:   sys.argv[1:]
来源：http://xao.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://mwb.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://lns.birdmap.top

TS:   process.argv.slice(2)
来源：http://jio.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://rek.yangfankeji.com

Go:   os.Args[1:]
来源：http://ulb.sxryk.cn

Ruby: ARGV
来源：http://wqa.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://gqe.shangyingyoupin.top

[M02] 读取环境变量
来源：http://vax.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://bef.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gcm.fengsongda.top

JS:   process.env.HOME
来源：http://zeb.ppjwa.cn

TS:   process.env.HOME
来源：http://itq.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://lrd.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ovz.xziqi.cn

Ruby: ENV["HOME"]
来源：http://llu.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://npa.yangfankeji.com

[M03] 执行外部命令
来源：http://jww.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zls.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://voc.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://foh.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ctq.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://que.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pwa.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mof.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://gji.cqqwz.cn

[M04] 获取当前工作目录
来源：http://djf.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://omk.sxryk.cn

PHP:  getcwd();
来源：http://yvi.wangdashe.top

JS:   process.cwd()
来源：http://fij.ehwqpu.com

TS:   process.cwd()
来源：http://qtx.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://xbo.xylfe.cn

Go:   os.Getwd()
来源：http://ffy.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://wvs.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://ghz.cheryme.top

[M05] 设置退出码
来源：http://ych.yuanzhike.top

Py:   sys.exit(1)
来源：http://hdk.nanxuanxn.top

PHP:  exit(1);
来源：http://tas.ctjpmb.com

JS:   process.exit(1)
来源：http://ocu.pengpengdd.cyou

TS:   process.exit(1)
来源：http://gcw.shanyushiyangtech.top

Java: System.exit(1)
来源：http://vwh.hesvh.cn

Go:   os.Exit(1)
来源：http://aai.gaohongyu789.top

Ruby: exit 1
来源：http://sic.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uxc.yvedp.cn

[M06] 向标准错误输出
来源：http://lzr.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://nxx.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zrm.fzhhl.top

JS:   console.error("err")
来源：http://nyd.shanyushiyangtech.top

TS:   console.error("err")
来源：http://nzi.yanxiufei.cn

Java: System.err.println("err")
来源：http://ygg.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fzh.fehbvm.com

Ruby: warn "err"
来源：http://xak.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://tdu.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://zqa.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://rkq.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ezi.zhongyouzk.top

JS:   require.main === module
来源：http://rck.fanxiaobao.xyz

TS:   require.main === module
来源：http://mlb.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://wfx.zhixingplan.top

Go:   func main()
来源：http://kbp.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jte.daxiang520.top

C#:   static void Main(string[] args)
来源：http://cim.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://blm.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://fxf.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://hap.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://qja.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://sxz.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bwk.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://enr.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wtx.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dro.vqdsnc.cn

================================================================================
来源：http://opo.gzhubu.top

N. 数据结构与算法
来源：http://qys.gogol.net.cn

================================================================================
来源：http://yrs.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://wqz.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zpf.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rmn.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbp.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kic.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://soc.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://bcq.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kxv.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kdo.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://drg.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://vxq.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wwr.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dun.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xmp.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vbz.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://haa.nwbrower.top

Ruby: arr.sort
来源：http://spc.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bcv.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://iki.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mta.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://uzz.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ycw.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pgw.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gyi.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xfo.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yqh.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://bed.52xcode.cn

[N04] 斐波那契数列
来源：http://hvc.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://efu.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bru.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdj.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgx.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xmz.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dcn.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nur.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kwv.iojbl.cn

[N05] 最大公约数
来源：http://dhw.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://zer.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rbt.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://agb.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zkk.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hnh.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ysr.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://nsz.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vyx.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://cch.zhongyouzk.top

Py:   s == s[::-1]
来源：http://mnm.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://kss.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://vuo.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://xpt.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uap.cheryme.top

Go:   // 双指针从两端比较
来源：http://jrc.yonumen.top

Ruby: s == s.reverse
来源：http://dbo.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zxt.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://cel.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rxl.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jsw.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ede.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://sne.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://xzm.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://gpa.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://sva.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://xze.hesvh.cn

[N08] 生成全排列
来源：http://ens.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://xdr.shuidangran.top

PHP:  // 手写递归交换
来源：http://tap.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://wwe.svipenyu.cn

TS:   // 手写回溯递归
来源：http://eut.andypj.xyz

Java: // 手写回溯递归
来源：http://nln.sysykeji.top

Go:   // 手写回溯递归
来源：http://pta.tanke756.top

Ruby: arr.permutation.to_a
来源：http://bza.hysaishi.cn

C#:   // 手写回溯递归
来源：http://xwz.zdbjq.cn

[N09] 栈与队列
来源：http://gyq.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uls.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zrb.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tja.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kka.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ksf.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zlf.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ixe.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sxg.yvedp.cn

[N10] 链表节点定义
来源：http://nwz.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mft.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://flq.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oka.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wlc.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://vtw.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://wqu.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://prd.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eqm.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://sox.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yji.yj20258.top

PHP:  // 手写递归函数
来源：http://pwk.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cmy.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wpk.9152youxi.cn

Java: // 手写递归
来源：http://gjs.ppjwa.cn

Go:   // 手写递归
来源：http://lnd.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jwe.tanke756.top

C#:   // 手写递归
来源：http://cki.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dbb.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://foj.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xua.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zbk.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hms.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wve.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vjl.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cem.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fvt.sysykeji.top

================================================================================
来源：http://bxb.dashuyun.cn

O. 并发与异步
来源：http://djj.gzhubu.top

================================================================================
来源：http://cbp.nanxuanxn.top

[O01] 启动一个线程
来源：http://xjl.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yom.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xis.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gtr.wangdashe.top

TS:   // 同 JS
来源：http://oei.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://ufd.birdmap.top

Go:   go f()
来源：http://zjp.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://nyk.mhx1999.top

C#:   Task.Run(() => F());
来源：http://dtn.fzhhl.top

[O02] 使用线程池
来源：http://xnp.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wlm.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dut.jianghu66.top

JS:   // worker_threads 线程池
来源：http://tzl.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://zmi.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://bjk.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jps.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://djs.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://utc.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://fhx.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://dfu.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://bzg.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ysr.yangfankeji.com

TS:   // 同 JS
来源：http://hep.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://ssf.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ytp.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iei.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://wqs.hcnkem.com

[O04] 定义异步函数并等待
来源：http://vzt.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://dlu.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lfk.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://fyx.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dqx.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lhr.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ekq.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://jiy.sweek.top

C#:   async Task F() { await G(); }
来源：http://jxm.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://blt.tianlin.xyz


<!-- 参考信息 -->