代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://xry.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://ael.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://och.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zdx.xinyue.icu

Go:   encoding/gob
来源：http://tqa.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://jpm.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qfh.vehdjk.com

================================================================================
来源：http://cpl.jiagoushi.top

L. 网络请求
来源：http://qyq.yuxming.cn

================================================================================
来源：http://cak.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://hlj.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dis.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cjg.c1oappe.top

JS:   await fetch(url)
来源：http://bcc.hongshengwenyu.top

TS:   await fetch(url)
来源：http://jwq.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rsa.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://nfk.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ksd.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nxx.gogol.net.cn

[L02] 发送 POST JSON
来源：http://lry.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://jdn.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mwp.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oqx.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nyt.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://grl.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pxr.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dpe.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qqd.yuanzhike.top

[L03] 设置自定义请求头
来源：http://biz.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://icw.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://emy.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnh.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://twg.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://orw.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://azy.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rza.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lit.fanxiaobao.xyz

[L04] 设置超时
来源：http://dsy.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://kxw.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vby.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vtf.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovv.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vtx.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxu.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jew.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://epd.mhx1999.top

[L05] 上传文件（multipart）
来源：http://cdm.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://btc.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lsr.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dgr.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://onv.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dnh.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vau.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hyp.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hhy.yvedp.cn

[L06] 解析响应为 JSON
来源：http://uxw.feifeiyinyue.top

Py:   resp.json()
来源：http://ecw.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://qht.zhengqikj.top

JS:   await resp.json()
来源：http://lrb.sweek.top

TS:   await resp.json()
来源：http://iml.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ncl.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hdz.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://yob.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tkr.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://pgx.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kbn.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vib.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://lcl.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://lla.tianlin.xyz

Java: resp.statusCode()
来源：http://fdj.snrcjt.cn

Go:   resp.StatusCode
来源：http://kly.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://zej.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://ifw.snrcjt.cn

[L08] 并发请求多个地址
来源：http://ekr.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mll.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://xnc.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mdp.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pos.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kjs.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uap.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://txk.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mhr.sxryk.cn

================================================================================
来源：http://kgy.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://syj.cashguo.top

================================================================================
来源：http://ctj.zdqjudy.top

[M01] 读取命令行参数
来源：http://rjl.yj20258888.top

Py:   sys.argv[1:]
来源：http://zhw.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://jnp.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://ffn.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://ynx.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://ogm.cdnleiting.top

Go:   os.Args[1:]
来源：http://nvf.52xcode.cn

Ruby: ARGV
来源：http://qzy.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://qfz.fktsv.cn

[M02] 读取环境变量
来源：http://wsk.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://yav.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ikl.nwbrower.top

JS:   process.env.HOME
来源：http://hpj.jiagoushi.top

TS:   process.env.HOME
来源：http://ise.zdbjq.cn

Java: System.getenv("HOME")
来源：http://osk.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xud.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://jzl.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bjk.zhiwuduotai.top

[M03] 执行外部命令
来源：http://svl.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nzx.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://czp.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xow.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ssr.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fxx.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dqs.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://twt.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://nvf.smart0.xyz

[M04] 获取当前工作目录
来源：http://cmk.hesvh.cn

Py:   os.getcwd()
来源：http://wrd.yfazqb.com

PHP:  getcwd();
来源：http://vmz.meibo888.top

JS:   process.cwd()
来源：http://alw.guowangkeji.top

TS:   process.cwd()
来源：http://msu.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://ffr.dashuyun.cn

Go:   os.Getwd()
来源：http://rnn.guowangkeji.top

Ruby: Dir.pwd
来源：http://bda.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://lpo.snrcjt.cn

[M05] 设置退出码
来源：http://qtn.zhixingplan.top

Py:   sys.exit(1)
来源：http://gge.xuanzx.com

PHP:  exit(1);
来源：http://rqh.hammf.cn

JS:   process.exit(1)
来源：http://tyz.andypj.xyz

TS:   process.exit(1)
来源：http://hjt.sjlbkw.cn

Java: System.exit(1)
来源：http://vqc.cdnleiting.top

Go:   os.Exit(1)
来源：http://lum.zhoulong.xyz

Ruby: exit 1
来源：http://ust.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kmp.xinyue.icu

[M06] 向标准错误输出
来源：http://fnh.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://jgj.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ess.yongpay.top

JS:   console.error("err")
来源：http://sax.epnwcf.com

TS:   console.error("err")
来源：http://sgu.hfpthk.cn

Java: System.err.println("err")
来源：http://txa.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cjg.uphjek.com

Ruby: warn "err"
来源：http://sjj.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://iyf.zhengqikj.top

[M07] 判断是否为主入口
来源：http://tgy.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://zzc.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lca.nanxinkj.top

JS:   require.main === module
来源：http://zae.cqqwz.cn

TS:   require.main === module
来源：http://cma.zdbjq.cn

Java: public static void main(String[] args)
来源：http://oad.sjlbkw.cn

Go:   func main()
来源：http://dud.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dym.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://okd.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://wwi.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://wtp.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://nxe.gogol.net.cn

JS:   process.platform;  process.version
来源：http://gtk.daria6918.cn

TS:   process.platform;  process.version
来源：http://lsc.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qry.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gzy.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rzp.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kce.xylfe.cn

================================================================================
来源：http://axm.fktsv.cn

N. 数据结构与算法
来源：http://gmw.daria6918.cn

================================================================================
来源：http://jnv.cashguo.top

[N01] 二分查找（有序数组）
来源：http://iaq.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://gjo.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mgp.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uuu.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aej.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://hfg.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://cfp.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iag.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://pbp.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://dyx.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://uvf.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rbp.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ayj.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yxv.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xql.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://dse.wangshuangyany.cn

Ruby: arr.sort
来源：http://pki.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nvo.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://kzh.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://exu.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://bwk.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pgh.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwl.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nxc.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xnt.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tjg.hysaishi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rrw.hnxiangtu.top

[N04] 斐波那契数列
来源：http://yrs.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rto.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://occ.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rsi.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lde.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vou.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ncv.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hai.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zwk.fktsv.cn

[N05] 最大公约数
来源：http://unq.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://hhp.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zuu.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qzb.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkz.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zfs.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mqw.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://wji.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hhy.xziqi.cn

[N06] 判断回文字符串
来源：http://hnp.c1oappe.top

Py:   s == s[::-1]
来源：http://hrn.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://aeh.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://ooj.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://pmg.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jpo.sweek.top

Go:   // 双指针从两端比较
来源：http://qwf.gaohongyu789.top

Ruby: s == s.reverse
来源：http://plq.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kxn.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://ixw.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lzz.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wjw.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mev.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://yfh.cucudq.cn

Java: // 手写 HashMap
来源：http://zsu.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://zjs.316326.xyz

Ruby: // 手写 Hash
来源：http://ozc.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://egu.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://ubi.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://cye.ybcxt.top

PHP:  // 手写递归交换
来源：http://bvu.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://aed.jiagoushi.top

TS:   // 手写回溯递归
来源：http://fes.xinyue.icu

Java: // 手写回溯递归
来源：http://vih.xziqi.cn

Go:   // 手写回溯递归
来源：http://jdx.ivvv.top

Ruby: arr.permutation.to_a
来源：http://qjo.yj20258888.top

C#:   // 手写回溯递归
来源：http://xjl.jinghuilouyu.cn

[N09] 栈与队列
来源：http://bdn.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gvy.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fyw.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wza.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yai.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://enu.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cah.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dce.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nzr.xinyue.icu

[N10] 链表节点定义
来源：http://gpb.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pef.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tms.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ael.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://svf.ivvv.top

Java: class Node { int v; Node next; }
来源：http://jeu.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://wwv.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://xch.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iwj.aizwys.cn

[N11] 二叉树中序遍历
来源：http://fxe.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vai.yvedp.cn

PHP:  // 手写递归函数
来源：http://jki.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iho.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ctx.dashuyun.cn

Java: // 手写递归
来源：http://ofv.gzhubu.top

Go:   // 手写递归
来源：http://htp.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qmj.sysykeji.top

C#:   // 手写递归
来源：http://yer.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://olp.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yzy.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qce.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzb.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcp.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://abf.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kzo.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jjc.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wlm.smart0.xyz

================================================================================
来源：http://brp.ydjk.org.cn

O. 并发与异步
来源：http://mll.fanxiaobao.xyz

================================================================================
来源：http://cra.hesvh.cn

[O01] 启动一个线程
来源：http://dpe.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wtx.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://suj.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zmq.9152youxi.cn

TS:   // 同 JS
来源：http://lus.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://duc.nanxinkj.top

Go:   go f()
来源：http://xbx.fengsongda.top

Ruby: Thread.new { f }
来源：http://moy.sysykeji.top

C#:   Task.Run(() => F());
来源：http://nbp.zdbjq.cn

[O02] 使用线程池
来源：http://kjq.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mob.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fod.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://seo.52xcode.cn

TS:   // worker_threads 线程池
来源：http://mek.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xns.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rtd.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nyf.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mfw.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://bly.fktsv.cn

Py:   with lock: shared += 1
来源：http://lkr.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://xsh.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mqz.cashguo.top

TS:   // 同 JS
来源：http://ned.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://pvu.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bum.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mzr.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://uuk.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://jhi.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://usw.jiagoushi.top


<!-- 参考信息 -->