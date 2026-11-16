代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://xbc.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://lsy.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://yva.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://czm.xuetiantiany.cn

Go:   encoding/gob
来源：http://xlu.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://bjx.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://auh.bbcook.cn

================================================================================
来源：http://eqo.xylfe.cn

L. 网络请求
来源：http://way.hcnkem.com

================================================================================
来源：http://mqm.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://vps.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kvz.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ayy.dashuyun.cn

JS:   await fetch(url)
来源：http://mmt.jiagoushi.top

TS:   await fetch(url)
来源：http://sbb.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lgi.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://lba.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eal.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lgk.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://tsb.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://voc.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dsc.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whz.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://geh.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://clf.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tnj.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fgt.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zfn.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://sew.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yxv.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rqk.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://svr.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lyb.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ycw.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ifo.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iio.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qmu.fehbvm.com

[L04] 设置超时
来源：http://oyl.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://yfo.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://piy.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgo.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dif.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://skt.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jue.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kni.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://syx.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://xqi.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jkz.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jrp.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jtd.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dyg.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bqg.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwn.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eil.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ohe.sweek.top

[L06] 解析响应为 JSON
来源：http://vos.yonumen.top

Py:   resp.json()
来源：http://ten.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://ree.chenzaomai.com

JS:   await resp.json()
来源：http://ifz.yj20258.top

TS:   await resp.json()
来源：http://maz.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tku.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lnj.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://cvm.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hom.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://hpf.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yvp.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xts.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://kjq.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://sor.hcnkem.com

Java: resp.statusCode()
来源：http://qqe.yangfankeji.com

Go:   resp.StatusCode
来源：http://uem.uphjek.com

Ruby: resp.code.to_i
来源：http://yjo.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://gif.sxryk.cn

[L08] 并发请求多个地址
来源：http://cob.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rdc.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://iii.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://srb.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwv.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pce.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://izg.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cdz.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yrh.shanyushiyangkeji.top

================================================================================
来源：http://rbx.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://umv.xylfe.cn

================================================================================
来源：http://nxj.jlsjyb.cn

[M01] 读取命令行参数
来源：http://kgq.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://pda.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://vkk.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://pzw.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://ahf.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://pvc.ybcxt.top

Go:   os.Args[1:]
来源：http://fkb.nwbrower.top

Ruby: ARGV
来源：http://wet.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://zaq.dashuyun.cn

[M02] 读取环境变量
来源：http://kiq.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://ixj.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ouu.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://tmq.sjlbkw.cn

TS:   process.env.HOME
来源：http://ydy.mhx1999.top

Java: System.getenv("HOME")
来源：http://kpo.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://puo.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://rmu.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vll.bjfxy.top

[M03] 执行外部命令
来源：http://zgq.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fcm.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://buy.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iih.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wlx.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tds.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ggi.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://rge.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://rfr.smart0.xyz

[M04] 获取当前工作目录
来源：http://hwv.chenjidiqi.icu

Py:   os.getcwd()
来源：http://ota.zhiwuduotai.top

PHP:  getcwd();
来源：http://rus.fehbvm.com

JS:   process.cwd()
来源：http://eea.ydzc1.top

TS:   process.cwd()
来源：http://zjw.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://bfn.xylfe.cn

Go:   os.Getwd()
来源：http://gvw.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://ahg.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cek.cheryme.top

[M05] 设置退出码
来源：http://oph.gotoacloud.top

Py:   sys.exit(1)
来源：http://prg.316326.xyz

PHP:  exit(1);
来源：http://cbl.ybcxt.top

JS:   process.exit(1)
来源：http://hcm.jiagoushi.top

TS:   process.exit(1)
来源：http://xtu.nwbrower.top

Java: System.exit(1)
来源：http://iwf.yj20258888.top

Go:   os.Exit(1)
来源：http://fnf.hcnkem.com

Ruby: exit 1
来源：http://jtg.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tby.yongpay.top

[M06] 向标准错误输出
来源：http://rki.yanxiufei.cn

Py:   print("err", file=sys.stderr)
来源：http://nqd.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://udu.andypj.xyz

JS:   console.error("err")
来源：http://rfo.chenjidiqi.icu

TS:   console.error("err")
来源：http://fnw.fengsongda.top

Java: System.err.println("err")
来源：http://dbj.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ncp.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://krt.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://ebn.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://qqq.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://oic.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eow.wangshuangyany.cn

JS:   require.main === module
来源：http://nte.shuidangran.top

TS:   require.main === module
来源：http://wai.chenlongwang.top

Java: public static void main(String[] args)
来源：http://aot.xuanzx.com

Go:   func main()
来源：http://cir.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ywf.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://qcr.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://eau.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://vrs.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://vmg.tian-w.cn

JS:   process.platform;  process.version
来源：http://kbq.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://bin.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nnw.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fyb.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fae.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zqz.aibaodan.cn

================================================================================
来源：http://hxp.hywenlv.cn

N. 数据结构与算法
来源：http://pyg.zycfv.cn

================================================================================
来源：http://tpj.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://zpk.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xcj.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eov.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vzh.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kzz.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://lic.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://dzo.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ryi.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://xuh.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://dgi.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://taj.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qmm.hnxiangtu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zru.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dsw.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tfk.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://vod.yuanzhike.top

Ruby: arr.sort
来源：http://xns.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bon.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://ojk.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dqc.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://yws.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iqm.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hlf.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mls.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://syy.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xwg.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://dnj.jqgfzy.top

[N04] 斐波那契数列
来源：http://zya.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gxd.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://one.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtw.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opf.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zuh.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ble.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bzf.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cxo.zhengqikj.top

[N05] 最大公约数
来源：http://lnz.hnqzz.top

Py:   math.gcd(a, b)
来源：http://xre.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hcx.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbd.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gmm.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gbj.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xsx.mhx1999.top

Ruby: a.gcd(b)
来源：http://gal.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sel.vqdsnc.cn

[N06] 判断回文字符串
来源：http://adz.vehdjk.com

Py:   s == s[::-1]
来源：http://rxq.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://bar.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://gyw.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://adr.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bcq.ybcxt.top

Go:   // 双指针从两端比较
来源：http://fmf.jqgfzy.top

Ruby: s == s.reverse
来源：http://lxi.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ljj.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://mmf.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hgj.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nny.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ypg.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://mhg.cheryme.top

Java: // 手写 HashMap
来源：http://qzl.xuanzx.com

Go:   // 手写 map[int]int
来源：http://dta.gzhubu.top

Ruby: // 手写 Hash
来源：http://zhu.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://ziu.xylfe.cn

[N08] 生成全排列
来源：http://ogq.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://how.yueranfly.top

PHP:  // 手写递归交换
来源：http://pvk.jinqigufen.top

JS:   // 手写回溯递归
来源：http://ptd.xinyue.icu

TS:   // 手写回溯递归
来源：http://hik.dianchejie.cn

Java: // 手写回溯递归
来源：http://zln.chenzaomai.com

Go:   // 手写回溯递归
来源：http://ato.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://ncg.tian-w.cn

C#:   // 手写回溯递归
来源：http://tnr.ydzc1.top

[N09] 栈与队列
来源：http://cia.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xgw.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iix.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tiq.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nkt.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rju.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xwc.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewt.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uau.hnqzz.top

[N10] 链表节点定义
来源：http://hag.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fzq.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zfl.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qrw.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://job.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://npy.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jrw.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ots.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://vpk.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://kwb.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aqn.jyoumei.cn

PHP:  // 手写递归函数
来源：http://ppw.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hly.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hxm.andypj.xyz

Java: // 手写递归
来源：http://sop.guowangkeji.top

Go:   // 手写递归
来源：http://jzn.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wuu.zdbjq.cn

C#:   // 手写递归
来源：http://uqu.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dsn.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bot.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://esp.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://atz.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://goj.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cgo.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oiu.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qme.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cxi.gaohongyu789.top

================================================================================
来源：http://jcz.feifeiyinyue.top

O. 并发与异步
来源：http://idn.ehwqpu.com

================================================================================
来源：http://fph.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://ioi.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cxf.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vvp.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pll.hywenlv.cn

TS:   // 同 JS
来源：http://tbj.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://lfl.hnqzz.top

Go:   go f()
来源：http://uil.316326.xyz

Ruby: Thread.new { f }
来源：http://vta.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://moa.ivvv.top

[O02] 使用线程池
来源：http://kmw.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cau.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lgb.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://abc.yongpay.top

TS:   // worker_threads 线程池
来源：http://zxc.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://ifo.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://izl.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cbx.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kud.cucudq.cn

[O03] 加锁保护共享数据
来源：http://zxq.zycfv.cn

Py:   with lock: shared += 1
来源：http://uhb.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://tdb.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cpz.sjlbkw.cn

TS:   // 同 JS
来源：http://gsg.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://ris.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wnt.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xmp.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://ncu.aizwys.cn

[O04] 定义异步函数并等待
来源：http://tce.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://qvz.xuanzx.com


<!-- 参考信息 -->