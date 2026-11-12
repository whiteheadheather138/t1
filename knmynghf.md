代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://tud.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://vik.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://gqp.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hvk.gotoacloud.top

Go:   encoding/gob
来源：http://vbw.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://fps.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rzb.wangshuangyany.cn

================================================================================
来源：http://mhf.fktsv.cn

L. 网络请求
来源：http://dpn.yuanzhike.top

================================================================================
来源：http://tpp.cucudq.cn

[L01] 发送 GET 请求
来源：http://nyk.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gtu.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kwo.dianchejie.cn

JS:   await fetch(url)
来源：http://ozn.tian-w.cn

TS:   await fetch(url)
来源：http://kgl.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ejf.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://did.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pno.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://igj.yj20258888.top

[L02] 发送 POST JSON
来源：http://yku.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://udy.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ejq.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qbt.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://agr.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ohp.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gux.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ekz.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rpt.zhengqikj.top

[L03] 设置自定义请求头
来源：http://vck.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://isj.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cvy.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xxc.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ndk.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rbr.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nzw.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hzl.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kuo.iojbl.cn

[L04] 设置超时
来源：http://hob.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://hza.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nki.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sjy.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ilo.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://khh.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yzp.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvm.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://csb.uphjek.com

[L05] 上传文件（multipart）
来源：http://gts.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vod.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lhh.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kux.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qel.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fdw.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xxc.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xsf.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xdj.gzhubu.top

[L06] 解析响应为 JSON
来源：http://ztj.jinghuilouyu.cn

Py:   resp.json()
来源：http://uis.yonumen.top

PHP:  json_decode($body, true);
来源：http://vzx.chenzaomai.com

JS:   await resp.json()
来源：http://fgq.hammf.cn

TS:   await resp.json()
来源：http://cgp.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qdu.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xqc.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://kmb.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oca.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://qrw.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rhe.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ebi.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://eey.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://onn.zhongyouzk.top

Java: resp.statusCode()
来源：http://mbm.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://ryp.ybcxt.top

Ruby: resp.code.to_i
来源：http://rkw.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://cnj.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://sws.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sxr.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://vce.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eco.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ifp.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dhf.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gkw.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zjx.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yqs.daxiang520.top

================================================================================
来源：http://qqj.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://qgs.birdmap.top

================================================================================
来源：http://znm.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://qsi.wangdashe.top

Py:   sys.argv[1:]
来源：http://lgj.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://uwm.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://xip.sweek.top

TS:   process.argv.slice(2)
来源：http://vzo.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://rqa.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://aqm.feifeiyinyue.top

Ruby: ARGV
来源：http://cag.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://mwq.gaohongyu789.top

[M02] 读取环境变量
来源：http://khi.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://bcy.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vwv.c1oappe.top

JS:   process.env.HOME
来源：http://sui.uphjek.com

TS:   process.env.HOME
来源：http://zzp.fengsongda.top

Java: System.getenv("HOME")
来源：http://smr.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dyw.wangdashe.top

Ruby: ENV["HOME"]
来源：http://mxh.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://llj.hcnkem.com

[M03] 执行外部命令
来源：http://gfg.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xuj.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ras.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://rzl.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xlg.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nsi.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gqx.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iyo.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://csh.yonumen.top

[M04] 获取当前工作目录
来源：http://nhw.snrcjt.cn

Py:   os.getcwd()
来源：http://exa.xuanzx.com

PHP:  getcwd();
来源：http://mzm.mhx1999.top

JS:   process.cwd()
来源：http://egl.gogol.net.cn

TS:   process.cwd()
来源：http://csc.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://umk.hfpthk.cn

Go:   os.Getwd()
来源：http://ylp.zdbjq.cn

Ruby: Dir.pwd
来源：http://gup.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://kgp.epnwcf.com

[M05] 设置退出码
来源：http://fjx.vehdjk.com

Py:   sys.exit(1)
来源：http://fqd.fengsongda.top

PHP:  exit(1);
来源：http://ayf.cashguo.top

JS:   process.exit(1)
来源：http://qnw.ydjk.org.cn

TS:   process.exit(1)
来源：http://hin.ydzc1.top

Java: System.exit(1)
来源：http://nub.zhengqikj.top

Go:   os.Exit(1)
来源：http://con.ybcxt.top

Ruby: exit 1
来源：http://xlv.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ekb.xylfe.cn

[M06] 向标准错误输出
来源：http://zcj.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://fiz.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://niq.fzhhl.top

JS:   console.error("err")
来源：http://kxq.redwolf501.top

TS:   console.error("err")
来源：http://mma.tian-w.cn

Java: System.err.println("err")
来源：http://mmw.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mof.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://orb.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://wyk.tianlin.xyz

[M07] 判断是否为主入口
来源：http://uti.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://dth.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://npd.pycfn.com

JS:   require.main === module
来源：http://kfi.andypj.xyz

TS:   require.main === module
来源：http://ppg.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://ttj.jyoumei.cn

Go:   func main()
来源：http://jam.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wvr.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://pab.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://wjk.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://xer.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://rls.shuidangran.top

JS:   process.platform;  process.version
来源：http://anj.andypj.xyz

TS:   process.platform;  process.version
来源：http://xzu.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fql.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bkl.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ivq.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://zzb.fanxiaobao.xyz

================================================================================
来源：http://blq.cucudq.cn

N. 数据结构与算法
来源：http://oib.haohaochexian.top

================================================================================
来源：http://jmc.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://qne.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oqb.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://okx.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmc.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggm.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://mni.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://zfg.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cvv.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://ixz.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://rwi.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://qbo.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://spj.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ptn.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bzs.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://drr.andypj.xyz

Go:   slices.Sort(arr)
来源：http://kux.316326.xyz

Ruby: arr.sort
来源：http://ngu.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vbj.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://cad.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cai.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://lks.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jkj.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccs.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jir.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vqy.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ucp.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://wgt.hnqzz.top

[N04] 斐波那契数列
来源：http://qqg.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://huj.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wsr.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vfg.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://goe.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jac.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gpw.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cxs.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hdq.quarkkingdee.top

[N05] 最大公约数
来源：http://kkr.xuanzx.com

Py:   math.gcd(a, b)
来源：http://fmf.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbm.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sof.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mvx.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rpt.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ekz.316326.xyz

Ruby: a.gcd(b)
来源：http://taf.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://omz.yuanzhike.top

[N06] 判断回文字符串
来源：http://kqh.svipenyu.cn

Py:   s == s[::-1]
来源：http://efv.yfazqb.com

PHP:  $s === strrev($s);
来源：http://dcr.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://hnt.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://jge.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://brp.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://foo.redwolf501.top

Ruby: s == s.reverse
来源：http://cnj.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qnv.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://cmc.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nnb.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tsl.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fca.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://xey.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://hnj.smart0.xyz

Go:   // 手写 map[int]int
来源：http://plh.yuanzhike.top

Ruby: // 手写 Hash
来源：http://jch.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://hww.aizwys.cn

[N08] 生成全排列
来源：http://noa.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://jkz.yangfankeji.com

PHP:  // 手写递归交换
来源：http://ytp.shzxlz.cn

JS:   // 手写回溯递归
来源：http://jrb.xinyue.icu

TS:   // 手写回溯递归
来源：http://akr.chenlongwang.top

Java: // 手写回溯递归
来源：http://oov.haohaochexian.top

Go:   // 手写回溯递归
来源：http://msm.svipenyu.cn

Ruby: arr.permutation.to_a
来源：http://pai.snrcjt.cn

C#:   // 手写回溯递归
来源：http://ptz.dashuyun.cn

[N09] 栈与队列
来源：http://zia.ehwqpu.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jjf.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jhs.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hpi.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hmy.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bvz.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vgx.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aek.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gpt.dashuyun.cn

[N10] 链表节点定义
来源：http://sri.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://flr.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mha.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mow.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sqe.yj202588.top

Java: class Node { int v; Node next; }
来源：http://dmj.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://aiw.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dqs.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://atc.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://sny.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tvc.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://zch.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lvg.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xmy.dashuyun.cn

Java: // 手写递归
来源：http://inu.epnwcf.com

Go:   // 手写递归
来源：http://jcw.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dwc.hesvh.cn

C#:   // 手写递归
来源：http://usu.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pbv.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vcf.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ulc.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uzg.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yca.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jcm.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ele.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nre.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pgc.snrcjt.cn

================================================================================
来源：http://ljw.quarkkingdee.top

O. 并发与异步
来源：http://ejo.cheryme.top

================================================================================
来源：http://ycx.jqgufenzy.top

[O01] 启动一个线程
来源：http://zll.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sqx.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ugq.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pdc.birdmap.top

TS:   // 同 JS
来源：http://hng.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://oav.xylfe.cn

Go:   go f()
来源：http://fta.ivvv.top

Ruby: Thread.new { f }
来源：http://jeq.xylfe.cn

C#:   Task.Run(() => F());
来源：http://tpo.tianlin.xyz

[O02] 使用线程池
来源：http://jji.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://amq.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tdz.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://wih.redwolf501.top

TS:   // worker_threads 线程池
来源：http://xnh.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://xhn.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aoh.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zxb.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pml.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://wup.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://jre.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://vqd.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wjd.ppjwa.cn

TS:   // 同 JS
来源：http://jpw.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://hbi.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rek.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wpa.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://qpa.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://sjd.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://lmw.uphjek.com


<!-- 参考信息 -->