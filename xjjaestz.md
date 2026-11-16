代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ivm.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ntq.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://zpf.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://cot.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mkg.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://igw.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://lrb.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lqh.tanke756.top

Go:   encoding/gob
来源：http://pjq.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://gpw.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yry.9152youxi.cn

================================================================================
来源：http://fzc.zhixingplan.top

L. 网络请求
来源：http://vpk.zycfv.cn

================================================================================
来源：http://ojg.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://dcl.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lnk.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kss.cashguo.top

JS:   await fetch(url)
来源：http://aeh.quarkkingdee.top

TS:   await fetch(url)
来源：http://axs.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nnk.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://xbj.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fzj.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fwe.daxiang520.top

[L02] 发送 POST JSON
来源：http://tzc.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://nqx.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fsl.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://thy.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cki.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dqa.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xin.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lau.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qda.ppjwa.cn

[L03] 设置自定义请求头
来源：http://xuf.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nga.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zul.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eto.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqd.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wys.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nww.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://euw.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wss.aibaodan.cn

[L04] 设置超时
来源：http://zcn.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://zzy.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aks.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qln.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byx.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ouh.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://usy.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bfr.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lvh.epnwcf.com

[L05] 上传文件（multipart）
来源：http://bak.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rjl.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xdq.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fbx.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gac.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bkh.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jtk.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hpv.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cri.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://zvj.shuidangran.top

Py:   resp.json()
来源：http://ozd.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://dii.bbcook.cn

JS:   await resp.json()
来源：http://mdw.c1oappe.top

TS:   await resp.json()
来源：http://hun.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://foi.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kjs.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://cxj.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jdd.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://amr.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rhh.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fdi.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://eip.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://mus.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://eea.xuanzx.com

Go:   resp.StatusCode
来源：http://omk.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://zxl.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://tuu.0kj1m.cn

[L08] 并发请求多个地址
来源：http://pnm.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://snw.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://ksc.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mon.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uoy.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rmc.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gzo.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rri.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gmn.uphjek.com

================================================================================
来源：http://jnq.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://kfh.316326.xyz

================================================================================
来源：http://hyu.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://vgd.epnwcf.com

Py:   sys.argv[1:]
来源：http://iaq.jianghu66.top

PHP:  $argv;  $argc;
来源：http://tme.nwbrower.top

JS:   process.argv.slice(2)
来源：http://wge.guannengcc.top

TS:   process.argv.slice(2)
来源：http://slz.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://ekj.0kj1m.cn

Go:   os.Args[1:]
来源：http://hnp.zhaomingkeji.xyz

Ruby: ARGV
来源：http://thr.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://bxf.ehwqpu.com

[M02] 读取环境变量
来源：http://sbo.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://jwr.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sbc.zycfv.cn

JS:   process.env.HOME
来源：http://som.aibaodan.cn

TS:   process.env.HOME
来源：http://wsb.nwbrower.top

Java: System.getenv("HOME")
来源：http://xkb.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wtb.316326.xyz

Ruby: ENV["HOME"]
来源：http://vps.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://khx.snrcjt.cn

[M03] 执行外部命令
来源：http://lnd.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fas.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qhu.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nhv.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://arh.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lbf.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://glf.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://cwp.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://jww.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://inf.kuanghao11.cn

Py:   os.getcwd()
来源：http://zca.shanyushiyangtech.top

PHP:  getcwd();
来源：http://fxr.quarkkingdee.top

JS:   process.cwd()
来源：http://ktl.shangyingyoupin.top

TS:   process.cwd()
来源：http://rxp.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://fkz.hesvh.cn

Go:   os.Getwd()
来源：http://ayc.hesvh.cn

Ruby: Dir.pwd
来源：http://lqd.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://dzy.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://tfp.ydjk.org.cn

Py:   sys.exit(1)
来源：http://eon.hfpthk.cn

PHP:  exit(1);
来源：http://uab.hammf.cn

JS:   process.exit(1)
来源：http://vjy.dashuyun.cn

TS:   process.exit(1)
来源：http://bmc.shangyingyoupin.top

Java: System.exit(1)
来源：http://ydp.hywenlv.cn

Go:   os.Exit(1)
来源：http://kjv.chenjidiqi.icu

Ruby: exit 1
来源：http://fmw.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://apt.yongpay.top

[M06] 向标准错误输出
来源：http://yce.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://tmy.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mlp.yuanzhike.top

JS:   console.error("err")
来源：http://zbi.zhijiandao.cn

TS:   console.error("err")
来源：http://cdi.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://ngm.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ggu.quarkkingdee.top

Ruby: warn "err"
来源：http://luj.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://ock.yueranfly.top

[M07] 判断是否为主入口
来源：http://syj.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://xxn.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bav.yfazqb.com

JS:   require.main === module
来源：http://gem.zdqjudy.top

TS:   require.main === module
来源：http://rwv.yvedp.cn

Java: public static void main(String[] args)
来源：http://gqj.dianchejie.cn

Go:   func main()
来源：http://zky.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jte.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://zzv.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://kui.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://zkh.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://oag.0kj1m.cn

JS:   process.platform;  process.version
来源：http://wox.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://psv.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://onm.jianghu66.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rlx.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwn.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://omy.ehwqpu.com

================================================================================
来源：http://gjj.0kj1m.cn

N. 数据结构与算法
来源：http://fsj.guowangkeji.top

================================================================================
来源：http://nba.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://wnv.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://txh.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kmh.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qzl.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bet.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ytu.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://tbe.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ygt.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://ybi.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://dna.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://aeo.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ywq.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://php.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://czz.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fza.yfazqb.com

Go:   slices.Sort(arr)
来源：http://uui.zhoulong.xyz

Ruby: arr.sort
来源：http://gcp.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ylr.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://txi.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ect.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://wkk.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jli.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://geb.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sji.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zzw.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wav.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hpm.havefunace.top

[N04] 斐波那契数列
来源：http://rni.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uql.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pcj.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ejq.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tyw.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ozk.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bcu.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jcf.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wdp.gogol.net.cn

[N05] 最大公约数
来源：http://fkq.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://zik.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nfn.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tof.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://grn.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nrd.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ltx.hysaishi.cn

Ruby: a.gcd(b)
来源：http://zxl.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kku.nanxinkj.top

[N06] 判断回文字符串
来源：http://jpm.zdqjudy.top

Py:   s == s[::-1]
来源：http://ncm.bjfxy.top

PHP:  $s === strrev($s);
来源：http://qcg.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://eyp.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://ptg.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ogy.iojbl.cn

Go:   // 双指针从两端比较
来源：http://mtf.chenlongwang.top

Ruby: s == s.reverse
来源：http://gnt.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cki.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://dbo.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rzt.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ztl.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zey.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://fxn.ydjk.org.cn

Java: // 手写 HashMap
来源：http://ydy.yj20258.top

Go:   // 手写 map[int]int
来源：http://wso.yj20258.top

Ruby: // 手写 Hash
来源：http://epb.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://srz.xylfe.cn

[N08] 生成全排列
来源：http://sxn.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://wbg.yj20258.top

PHP:  // 手写递归交换
来源：http://qqd.birdmap.top

JS:   // 手写回溯递归
来源：http://can.zdbjq.cn

TS:   // 手写回溯递归
来源：http://xpx.sweek.top

Java: // 手写回溯递归
来源：http://tzo.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://jmu.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://amf.cashguo.top

C#:   // 手写回溯递归
来源：http://ifp.hammf.cn

[N09] 栈与队列
来源：http://gap.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rkd.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iuw.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hsi.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lbf.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://log.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oeo.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hxq.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gfc.dashuyun.cn

[N10] 链表节点定义
来源：http://gim.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yab.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ujk.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vdw.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://upr.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://fln.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tkz.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tsf.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ili.uphjek.com

[N11] 二叉树中序遍历
来源：http://gbl.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://upt.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://gqe.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lth.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ick.yj20258.top

Java: // 手写递归
来源：http://gcu.fanxiaobao.xyz

Go:   // 手写递归
来源：http://ebx.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://trr.jqgufenzy.top

C#:   // 手写递归
来源：http://fwk.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fex.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://avn.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vfn.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcq.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://euj.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://opf.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mnz.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://izh.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://agc.hysaishi.cn

================================================================================
来源：http://nre.0kj1m.cn

O. 并发与异步
来源：http://tez.yonumen.top

================================================================================
来源：http://bsx.sxryk.cn

[O01] 启动一个线程
来源：http://rxc.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://omt.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cdy.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kcv.fehbvm.com

TS:   // 同 JS
来源：http://rxf.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://hzi.sjlbkw.cn

Go:   go f()
来源：http://ojc.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://cmi.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://pav.meibo888.top

[O02] 使用线程池
来源：http://dtn.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xrb.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ehr.yj202588.top

JS:   // worker_threads 线程池
来源：http://guh.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://itx.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ijd.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gqn.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ctb.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yzr.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://wif.tianlin.xyz

Py:   with lock: shared += 1
来源：http://dau.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://xam.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yjc.dianchejie.cn

TS:   // 同 JS
来源：http://poe.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://njn.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fnn.jianghu66.top


<!-- 参考信息 -->