代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pde.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pdr.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://nus.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://ibi.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://uch.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://hja.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://vrx.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kge.smart0.xyz

Go:   encoding/gob
来源：http://gvw.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://jsh.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xzp.yuxming.cn

================================================================================
来源：http://mlx.gogol.net.cn

L. 网络请求
来源：http://spl.fanxiaobao.xyz

================================================================================
来源：http://fzi.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://fuu.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ibe.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dhh.xziqi.cn

JS:   await fetch(url)
来源：http://ehw.birdmap.top

TS:   await fetch(url)
来源：http://cxb.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://urk.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://hss.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fph.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://avj.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://jup.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iqi.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ezw.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwd.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjb.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://adi.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wmd.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wdc.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bxq.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://xov.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kzi.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eqk.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aiq.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpv.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tpi.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nmm.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://edl.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://luf.pycfn.com

[L04] 设置超时
来源：http://kxd.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://rxo.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lxv.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rgm.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tbk.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bvu.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zyi.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://imp.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lhw.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://kwf.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xqb.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pov.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xkh.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyc.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kke.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://err.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ara.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eax.xinyue.icu

[L06] 解析响应为 JSON
来源：http://kux.zdbjq.cn

Py:   resp.json()
来源：http://mcl.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://dbh.daria6918.cn

JS:   await resp.json()
来源：http://neu.svipenyu.cn

TS:   await resp.json()
来源：http://okm.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gxq.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wha.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://hrf.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lcg.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://lsh.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://szu.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mox.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://wrj.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://ulp.daxiang520.top

Java: resp.statusCode()
来源：http://hpp.fehbvm.com

Go:   resp.StatusCode
来源：http://hnh.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://rpe.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://qdv.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://ilr.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ubt.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://hqh.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbh.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://coj.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cxc.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ygl.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://obs.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gkg.hongshengwenyu.top

================================================================================
来源：http://zhx.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://nfg.hywenlv.cn

================================================================================
来源：http://odx.ydzc1.top

[M01] 读取命令行参数
来源：http://tqs.sysykeji.top

Py:   sys.argv[1:]
来源：http://hdc.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://ujf.fehbvm.com

JS:   process.argv.slice(2)
来源：http://hto.iojbl.cn

TS:   process.argv.slice(2)
来源：http://hry.havefunace.top

Java: args 数组（main 方法参数）
来源：http://sej.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://bcy.wangdashe.top

Ruby: ARGV
来源：http://ckz.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://mna.sufxvd.cn

[M02] 读取环境变量
来源：http://hqr.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://xvn.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ykx.zycfv.cn

JS:   process.env.HOME
来源：http://mxl.xziqi.cn

TS:   process.env.HOME
来源：http://dnh.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://jay.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xxt.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://khl.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hty.nanxuanxn.top

[M03] 执行外部命令
来源：http://ahq.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uem.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zmw.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sei.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mwo.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xlw.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://udk.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://lbj.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://ipm.cucudq.cn

[M04] 获取当前工作目录
来源：http://iam.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://xfy.pengpengdd.cyou

PHP:  getcwd();
来源：http://rss.gotoacloud.top

JS:   process.cwd()
来源：http://oqm.hysaishi.cn

TS:   process.cwd()
来源：http://fnz.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://oze.ydjk.org.cn

Go:   os.Getwd()
来源：http://ria.chenzaomai.com

Ruby: Dir.pwd
来源：http://ibp.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uho.jyoumei.cn

[M05] 设置退出码
来源：http://krw.gaohongyu789.top

Py:   sys.exit(1)
来源：http://ewj.316326.xyz

PHP:  exit(1);
来源：http://rrw.0kj1m.cn

JS:   process.exit(1)
来源：http://emw.sweek.top

TS:   process.exit(1)
来源：http://rjb.epnwcf.com

Java: System.exit(1)
来源：http://lxo.ybcxt.top

Go:   os.Exit(1)
来源：http://fee.birdmap.top

Ruby: exit 1
来源：http://gpw.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://thx.yongpay.top

[M06] 向标准错误输出
来源：http://wfg.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://dlf.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fyo.shanyushiyangtech.top

JS:   console.error("err")
来源：http://jhs.ivvv.top

TS:   console.error("err")
来源：http://hpi.fzhhl.top

Java: System.err.println("err")
来源：http://pwi.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tog.aibaodan.cn

Ruby: warn "err"
来源：http://dwj.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://tmi.xylfe.cn

[M07] 判断是否为主入口
来源：http://com.uphjek.com

Py:   if __name__ == "__main__":
来源：http://hlw.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cya.yongpay.top

JS:   require.main === module
来源：http://lrm.shanyushiyangkeji.top

TS:   require.main === module
来源：http://qui.pycfn.com

Java: public static void main(String[] args)
来源：http://eyk.yj20258.top

Go:   func main()
来源：http://okt.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qyz.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://aka.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://mji.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://yuc.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://gpx.yfazqb.com

JS:   process.platform;  process.version
来源：http://mof.vehdjk.com

TS:   process.platform;  process.version
来源：http://byg.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uyd.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vxq.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://okt.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://bmo.birdmap.top

================================================================================
来源：http://rae.ppjwa.cn

N. 数据结构与算法
来源：http://glm.yj202588.top

================================================================================
来源：http://wcg.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://khm.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://srv.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xxk.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ble.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ifg.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://gyr.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ara.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ntz.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://ofj.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://mpy.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://fpw.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gze.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qav.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tju.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ahd.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://heo.gaohongyu789.top

Ruby: arr.sort
来源：http://wql.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pzx.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://epb.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://toc.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://vmn.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://htr.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://flb.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dah.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gum.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cef.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ysk.guowangkeji.top

[N04] 斐波那契数列
来源：http://gmv.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rng.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gfp.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ccz.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ekb.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ayq.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://avs.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ioe.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gdz.daria6918.cn

[N05] 最大公约数
来源：http://umb.xylfe.cn

Py:   math.gcd(a, b)
来源：http://lxz.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://noi.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tgk.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hem.zhixingplan.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eou.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wfd.meibo888.top

Ruby: a.gcd(b)
来源：http://zhf.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jbk.ydjk.org.cn

[N06] 判断回文字符串
来源：http://dan.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://vzw.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://ujw.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://tft.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://gzo.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://faj.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://xma.aizwys.cn

Ruby: s == s.reverse
来源：http://tec.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mrp.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://nmy.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cfl.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wnf.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bly.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://yel.jianghu66.top

Java: // 手写 HashMap
来源：http://kmp.fehbvm.com

Go:   // 手写 map[int]int
来源：http://lfj.snrcjt.cn

Ruby: // 手写 Hash
来源：http://hvb.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://tki.shuidangran.top

[N08] 生成全排列
来源：http://aag.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://wcr.hammf.cn

PHP:  // 手写递归交换
来源：http://ibv.daxiang520.top

JS:   // 手写回溯递归
来源：http://mdp.gotoacloud.top

TS:   // 手写回溯递归
来源：http://egj.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://pfl.zhixingplan.top

Go:   // 手写回溯递归
来源：http://xqc.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://pyf.tian-w.cn

C#:   // 手写回溯递归
来源：http://kgu.yuanzhike.top

[N09] 栈与队列
来源：http://acy.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tlt.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iqc.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kqn.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lhe.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hkb.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xek.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sfr.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xod.ybcxt.top

[N10] 链表节点定义
来源：http://jdj.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://frb.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hkd.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ssy.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tzl.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://bmt.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xua.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yjp.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ruh.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://rsn.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fko.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://pjz.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qis.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fue.zdqjudy.top

Java: // 手写递归
来源：http://tzo.sufxvd.cn

Go:   // 手写递归
来源：http://buy.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ade.yj20258.top

C#:   // 手写递归
来源：http://cfj.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://err.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xvk.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://alh.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hhi.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cdx.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://voc.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nyg.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xgj.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://idq.havefunace.top

================================================================================
来源：http://pop.vehdjk.com

O. 并发与异步
来源：http://kqh.jyoumei.cn

================================================================================
来源：http://img.sjlbkw.cn

[O01] 启动一个线程
来源：http://bfa.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://seb.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xec.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vab.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://nln.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://ubs.zhengqikj.top

Go:   go f()
来源：http://ouu.gzhubu.top

Ruby: Thread.new { f }
来源：http://dhx.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://blm.cqqwz.cn

[O02] 使用线程池
来源：http://aqy.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://peg.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rua.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://pfy.cashguo.top

TS:   // worker_threads 线程池
来源：http://izs.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yqw.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aot.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xkf.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qsr.uphjek.com

[O03] 加锁保护共享数据
来源：http://dvz.cdnleiting.top

Py:   with lock: shared += 1
来源：http://gdz.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://gjx.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yzs.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://vgt.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://lgc.ydzc1.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nym.chenjidiqi.icu


<!-- 参考信息 -->