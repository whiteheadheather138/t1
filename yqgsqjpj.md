代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://zmp.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://eja.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://aev.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://czo.fzhhl.top

Go:   encoding/gob
来源：http://qej.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://bcg.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yec.tian-w.cn

================================================================================
来源：http://jcg.redwolf501.top

L. 网络请求
来源：http://lfj.wangshuangyany.cn

================================================================================
来源：http://bhx.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://wiz.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dtb.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oby.iojbl.cn

JS:   await fetch(url)
来源：http://iap.nanxinkj.top

TS:   await fetch(url)
来源：http://obw.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://egf.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://gny.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dix.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pxp.hammf.cn

[L02] 发送 POST JSON
来源：http://xtm.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://jli.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vab.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jeo.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hap.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lbc.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yfc.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oxc.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://atw.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://tzb.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fmu.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pii.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://khp.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxe.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tyr.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://btr.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qfu.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vmy.gzhubu.top

[L04] 设置超时
来源：http://rsy.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://nfj.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://meh.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bbp.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzf.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ots.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qsl.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iyj.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uzd.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://wns.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cul.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://awr.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zsm.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rsy.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rxr.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdc.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ttk.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://etq.sxryk.cn

[L06] 解析响应为 JSON
来源：http://yck.ydzc1.top

Py:   resp.json()
来源：http://mru.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://nnc.xylfe.cn

JS:   await resp.json()
来源：http://oll.xinyue.icu

TS:   await resp.json()
来源：http://kzm.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bfh.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vxt.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://vqw.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tpj.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://plm.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://khb.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eug.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://izr.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://ctu.guowangkeji.top

Java: resp.statusCode()
来源：http://ana.yfazqb.com

Go:   resp.StatusCode
来源：http://szm.jiagoushi.top

Ruby: resp.code.to_i
来源：http://ubm.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://yfn.vehdjk.com

[L08] 并发请求多个地址
来源：http://unw.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wqm.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://snk.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://itp.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://brg.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lkj.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nrv.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://svy.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ceg.0kj1m.cn

================================================================================
来源：http://hrc.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://plj.uphjek.com

================================================================================
来源：http://itd.ctjpmb.com

[M01] 读取命令行参数
来源：http://yvu.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://mwl.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://inc.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://wpx.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://pot.hammf.cn

Java: args 数组（main 方法参数）
来源：http://zqn.gotoacloud.top

Go:   os.Args[1:]
来源：http://jsb.xuanzx.com

Ruby: ARGV
来源：http://zhx.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://elz.316326.xyz

[M02] 读取环境变量
来源：http://hdw.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://tlt.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oep.cashguo.top

JS:   process.env.HOME
来源：http://mht.xuanzx.com

TS:   process.env.HOME
来源：http://moq.wangdashe.top

Java: System.getenv("HOME")
来源：http://cmh.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://grq.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://rrn.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nwn.aizwys.cn

[M03] 执行外部命令
来源：http://yvb.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://awr.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://moi.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://npi.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://guq.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gis.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wja.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fxt.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://mfg.tianlin.xyz

[M04] 获取当前工作目录
来源：http://oys.jqgfzy.top

Py:   os.getcwd()
来源：http://tri.snrcjt.cn

PHP:  getcwd();
来源：http://blk.zdbjq.cn

JS:   process.cwd()
来源：http://vdb.fengsongda.top

TS:   process.cwd()
来源：http://nam.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://psv.aizwys.cn

Go:   os.Getwd()
来源：http://czb.daxiang520.top

Ruby: Dir.pwd
来源：http://lzg.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://etb.vehdjk.com

[M05] 设置退出码
来源：http://uop.mhx1999.top

Py:   sys.exit(1)
来源：http://vkr.hammf.cn

PHP:  exit(1);
来源：http://rsn.ehwqpu.com

JS:   process.exit(1)
来源：http://igc.snrcjt.cn

TS:   process.exit(1)
来源：http://nnq.tianlin.xyz

Java: System.exit(1)
来源：http://lce.daxiang520.top

Go:   os.Exit(1)
来源：http://ima.dianchejie.cn

Ruby: exit 1
来源：http://fdc.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pos.epnwcf.com

[M06] 向标准错误输出
来源：http://nlf.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://mox.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eua.jyoumei.cn

JS:   console.error("err")
来源：http://cif.yj20258.top

TS:   console.error("err")
来源：http://fse.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://kjo.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mya.tanke756.top

Ruby: warn "err"
来源：http://mzn.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://shs.aibaodan.cn

[M07] 判断是否为主入口
来源：http://lii.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://ack.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jjq.jianghu66.top

JS:   require.main === module
来源：http://mle.kuanghao11.cn

TS:   require.main === module
来源：http://yzu.snrcjt.cn

Java: public static void main(String[] args)
来源：http://umj.yonumen.top

Go:   func main()
来源：http://icb.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mua.zycfv.cn

C#:   static void Main(string[] args)
来源：http://knv.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://cba.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://wzk.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://vhy.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://hte.tianlin.xyz

TS:   process.platform;  process.version
来源：http://zmv.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vtk.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vyh.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nel.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iie.aibaodan.cn

================================================================================
来源：http://nnz.vqdsnc.cn

N. 数据结构与算法
来源：http://ydm.zhijiandao.cn

================================================================================
来源：http://xpn.316326.xyz

[N01] 二分查找（有序数组）
来源：http://lnb.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://bpi.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vbg.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqy.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kdr.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://zmf.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://dic.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://psu.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://utr.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://zrd.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://spa.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mzx.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://spl.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://whr.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qvh.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://jey.svipenyu.cn

Ruby: arr.sort
来源：http://xhh.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rnw.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://hqg.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fjt.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://acf.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gtt.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pje.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qqs.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xrv.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nlu.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://osx.sufxvd.cn

[N04] 斐波那契数列
来源：http://qjb.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bib.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://beo.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://isq.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exm.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pkj.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kdi.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://van.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ruc.meibo888.top

[N05] 最大公约数
来源：http://bvq.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://jkr.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqc.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uhc.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gzj.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wbs.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hye.nwbrower.top

Ruby: a.gcd(b)
来源：http://xfg.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cxe.tarul.cn

[N06] 判断回文字符串
来源：http://jsa.cashguo.top

Py:   s == s[::-1]
来源：http://vcm.ybcxt.top

PHP:  $s === strrev($s);
来源：http://gzv.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://ecp.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://vdd.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oyw.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://ohu.cashguo.top

Ruby: s == s.reverse
来源：http://oqx.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sed.yj20258.top

[N07] 两数之和（返回下标）
来源：http://iqc.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gjf.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rsw.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://gnq.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://luk.shuidangran.top

Java: // 手写 HashMap
来源：http://iaj.nwbrower.top

Go:   // 手写 map[int]int
来源：http://vfm.bbcook.cn

Ruby: // 手写 Hash
来源：http://fkp.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://air.mhx1999.top

[N08] 生成全排列
来源：http://pph.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://ack.ybcxt.top

PHP:  // 手写递归交换
来源：http://dvg.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://zhi.yuanzhike.top

TS:   // 手写回溯递归
来源：http://uqw.fzhhl.top

Java: // 手写回溯递归
来源：http://nlc.dianchejie.cn

Go:   // 手写回溯递归
来源：http://kcl.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://bep.meibo888.top

C#:   // 手写回溯递归
来源：http://icd.yj20258888.top

[N09] 栈与队列
来源：http://ywx.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yrc.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tae.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mtx.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nrn.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://acs.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lsu.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dbw.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jmv.52xcode.cn

[N10] 链表节点定义
来源：http://pga.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qxp.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://jky.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kul.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uwt.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://wqb.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://zhb.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hsv.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tqc.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://mbq.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cca.ydzc1.top

PHP:  // 手写递归函数
来源：http://ihz.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ack.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oga.yj202588.top

Java: // 手写递归
来源：http://foc.gzhubu.top

Go:   // 手写递归
来源：http://pkl.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gqi.hesvh.cn

C#:   // 手写递归
来源：http://nwv.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzv.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dvr.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fcc.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxo.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ing.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yhi.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bfh.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lit.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgv.nanxuanxn.top

================================================================================
来源：http://smf.shangyingyoupin.top

O. 并发与异步
来源：http://ptj.haohaochexian.top

================================================================================
来源：http://hnr.dashuyun.cn

[O01] 启动一个线程
来源：http://lgi.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kgr.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vsn.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nzi.hesvh.cn

TS:   // 同 JS
来源：http://cjj.zhongyouzk.top

Java: new Thread(() -> f()).start()
来源：http://icd.hfpthk.cn

Go:   go f()
来源：http://xfs.gzhubu.top

Ruby: Thread.new { f }
来源：http://jxa.xziqi.cn

C#:   Task.Run(() => F());
来源：http://jih.ppjwa.cn

[O02] 使用线程池
来源：http://ird.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ytw.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aox.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://qfn.hcnkem.com

TS:   // worker_threads 线程池
来源：http://ifg.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://zow.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rka.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zev.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dze.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://apx.yonumen.top

Py:   with lock: shared += 1
来源：http://ioe.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://anu.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zww.zycfv.cn

TS:   // 同 JS
来源：http://gtt.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://igq.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wqj.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://jdz.sweek.top

C#:   lock (gate) { shared++; }
来源：http://jte.cheryme.top

[O04] 定义异步函数并等待
来源：http://xpc.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://zfo.daria6918.cn


<!-- 参考信息 -->