代发 wailian999

Go:   encoding/gob
来源：http://rrh.sweek.top

Ruby: Marshal.dump(obj)
来源：http://rvl.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wla.meibo888.top

================================================================================
来源：http://nfz.jinqigufen.top

L. 网络请求
来源：http://kqt.hnxiangtu.top

================================================================================
来源：http://xhj.nanxinkj.top

[L01] 发送 GET 请求
来源：http://wmb.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vsm.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://goj.316326.xyz

JS:   await fetch(url)
来源：http://ale.nanxuanxn.top

TS:   await fetch(url)
来源：http://bmm.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qxy.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://gkh.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://por.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lkz.xylfe.cn

[L02] 发送 POST JSON
来源：http://ihj.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ieu.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mvo.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txk.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwi.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fwd.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uuy.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gkd.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://luc.yj202588.top

[L03] 设置自定义请求头
来源：http://ndj.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qgf.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ndh.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vjm.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://upb.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://von.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://txg.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pfe.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pyq.sxryk.cn

[L04] 设置超时
来源：http://hqn.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://zwi.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gds.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hya.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hek.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qqw.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ota.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tvv.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://cjm.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ixq.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ypn.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qdv.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jag.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://alz.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qgf.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pqw.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xxe.smart0.xyz

[L06] 解析响应为 JSON
来源：http://vig.hywenlv.cn

Py:   resp.json()
来源：http://lzx.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://zfi.fktsv.cn

JS:   await resp.json()
来源：http://axa.yangfankeji.com

TS:   await resp.json()
来源：http://yle.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ssn.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wkm.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://xdb.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rfv.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://igf.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://clc.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tjq.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://jfg.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://vpc.jqgfzy.top

Java: resp.statusCode()
来源：http://kjc.yuxming.cn

Go:   resp.StatusCode
来源：http://ahi.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://vyy.cheryme.top

C#:   (int)resp.StatusCode
来源：http://cbg.andypj.xyz

[L08] 并发请求多个地址
来源：http://igs.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qta.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://dud.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://erz.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ulh.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gkr.gotoacloud.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xpa.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sdq.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vgb.ctjpmb.com

================================================================================
来源：http://hbl.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://bvb.haohaochexian.top

================================================================================
来源：http://eno.ehwqpu.com

[M01] 读取命令行参数
来源：http://kob.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://xkl.yonumen.top

PHP:  $argv;  $argc;
来源：http://pmg.cheryme.top

JS:   process.argv.slice(2)
来源：http://gsf.tarul.cn

TS:   process.argv.slice(2)
来源：http://vhs.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://zcc.yuxming.cn

Go:   os.Args[1:]
来源：http://cad.sweek.top

Ruby: ARGV
来源：http://beh.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://cvg.shuidangran.top

[M02] 读取环境变量
来源：http://lan.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://dvx.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gwq.zhongyouzk.top

JS:   process.env.HOME
来源：http://wcs.xuanzx.com

TS:   process.env.HOME
来源：http://gcl.sufxvd.cn

Java: System.getenv("HOME")
来源：http://sga.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pmg.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://pjl.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eym.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://soi.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ejs.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vpb.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xdt.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://fmf.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://edh.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mxy.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://vpg.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://jtn.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://rtx.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://lxi.birdmap.top

PHP:  getcwd();
来源：http://mmv.havefunace.top

JS:   process.cwd()
来源：http://otz.zdbjq.cn

TS:   process.cwd()
来源：http://uoz.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://kyi.zdbjq.cn

Go:   os.Getwd()
来源：http://ytn.zycfv.cn

Ruby: Dir.pwd
来源：http://hcu.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://quo.haohaochexian.top

[M05] 设置退出码
来源：http://dac.xylfe.cn

Py:   sys.exit(1)
来源：http://bcr.fengsongda.top

PHP:  exit(1);
来源：http://gdb.chenzaomai.com

JS:   process.exit(1)
来源：http://zad.sxryk.cn

TS:   process.exit(1)
来源：http://nbx.zhongyouzk.top

Java: System.exit(1)
来源：http://tic.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://qzt.hfpthk.cn

Ruby: exit 1
来源：http://ohs.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rjx.zhoulong.xyz

[M06] 向标准错误输出
来源：http://nde.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://ndp.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://upu.smart0.xyz

JS:   console.error("err")
来源：http://xfx.bbcook.cn

TS:   console.error("err")
来源：http://yht.vehdjk.com

Java: System.err.println("err")
来源：http://dbp.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uje.yj20258888.top

Ruby: warn "err"
来源：http://lnr.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://vpw.havefunace.top

[M07] 判断是否为主入口
来源：http://rjb.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://akr.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ncr.yj202588.top

JS:   require.main === module
来源：http://web.shzxlz.cn

TS:   require.main === module
来源：http://eaz.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://viz.yangfankeji.com

Go:   func main()
来源：http://ypt.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eas.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://jqk.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://urg.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://mhp.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://xtk.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://srq.yj20258.top

TS:   process.platform;  process.version
来源：http://nae.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qse.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lrt.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bly.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jig.jinghuilouyu.cn

================================================================================
来源：http://cxg.yuanzhike.top

N. 数据结构与算法
来源：http://lnj.epnwcf.com

================================================================================
来源：http://qip.ivvv.top

[N01] 二分查找（有序数组）
来源：http://lmm.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kff.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://num.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tak.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jra.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://tuw.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://bhq.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://cpp.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uss.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://nhl.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://rqa.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://imm.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://vlx.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wac.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aoa.xziqi.cn

Go:   slices.Sort(arr)
来源：http://ifg.wangdashe.top

Ruby: arr.sort
来源：http://yjv.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sms.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://wzi.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eqd.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://btt.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyr.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ufy.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qob.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kvu.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blz.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://emx.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://yws.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jxu.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nqt.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wwb.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nrb.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nup.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rlt.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ydc.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mna.gotoacloud.top

[N05] 最大公约数
来源：http://fkm.jianghu66.top

Py:   math.gcd(a, b)
来源：http://mys.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dnb.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hao.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dld.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xnf.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cmo.cqqwz.cn

Ruby: a.gcd(b)
来源：http://mzl.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bsp.hfpthk.cn

[N06] 判断回文字符串
来源：http://dgg.jinqigfzy.top

Py:   s == s[::-1]
来源：http://mdm.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://sta.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://obm.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://ujo.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ogr.fengsongda.top

Go:   // 双指针从两端比较
来源：http://sru.yj202588.top

Ruby: s == s.reverse
来源：http://myd.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ayw.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://lia.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://twu.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xyr.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cam.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://ncv.meibo888.top

Java: // 手写 HashMap
来源：http://cre.yfazqb.com

Go:   // 手写 map[int]int
来源：http://tql.shuidangran.top

Ruby: // 手写 Hash
来源：http://pfd.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tdl.xuanzx.com

[N08] 生成全排列
来源：http://xdy.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://osh.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://dem.yvedp.cn

JS:   // 手写回溯递归
来源：http://gbt.hfpthk.cn

TS:   // 手写回溯递归
来源：http://amz.pycfn.com

Java: // 手写回溯递归
来源：http://adv.nanxinkj.top

Go:   // 手写回溯递归
来源：http://bic.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://yrr.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://svq.hnqzz.top

[N09] 栈与队列
来源：http://qra.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xkm.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gcp.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aeo.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rjs.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vwc.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yvj.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ube.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qdc.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://tzs.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kai.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nxh.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dkv.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://acy.cheryme.top

Java: class Node { int v; Node next; }
来源：http://kqt.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://bki.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sqz.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rhn.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://rba.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://arw.yj202588.top

PHP:  // 手写递归函数
来源：http://oda.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cqs.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cal.hongshengwenyu.top

Java: // 手写递归
来源：http://esc.hammf.cn

Go:   // 手写递归
来源：http://cyp.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eda.zhongyouzk.top

C#:   // 手写递归
来源：http://glw.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://szg.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xef.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xdk.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wcd.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhy.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fbg.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eqt.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ujb.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dsr.yuanzhike.top

================================================================================
来源：http://vsk.pycfn.com

O. 并发与异步
来源：http://nfe.xylfe.cn

================================================================================
来源：http://slx.fzhhl.top

[O01] 启动一个线程
来源：http://ycn.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rzl.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zvf.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bxi.hesvh.cn

TS:   // 同 JS
来源：http://toe.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://noy.feifeiyinyue.top

Go:   go f()
来源：http://wpd.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://lbg.316326.xyz

C#:   Task.Run(() => F());
来源：http://xkc.aizwys.cn

[O02] 使用线程池
来源：http://iqy.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dwr.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bji.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://lhg.ydzc1.top

TS:   // worker_threads 线程池
来源：http://ilh.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yul.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mag.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kwq.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gvd.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://tjh.xinyue.icu

Py:   with lock: shared += 1
来源：http://osc.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://bil.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vao.pycfn.com

TS:   // 同 JS
来源：http://rzd.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://qti.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mtp.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vdx.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://nak.bjfxy.top

[O04] 定义异步函数并等待
来源：http://qvn.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://feg.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kvp.xziqi.cn

JS:   async function f() { await g(); }
来源：http://tui.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wzb.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ruu.xuanzx.com


<!-- 参考信息 -->