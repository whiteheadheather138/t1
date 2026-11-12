代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zwi.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bme.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://xrc.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://yuy.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gxa.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://kbq.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://hqs.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rmu.birdmap.top

Go:   encoding/gob
来源：http://uqg.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://ouk.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ddi.sysykeji.top

================================================================================
来源：http://vml.ctjpmb.com

L. 网络请求
来源：http://czl.havefunace.top

================================================================================
来源：http://kbj.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://lxf.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mcw.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://udu.ydzc1.top

JS:   await fetch(url)
来源：http://aae.aizwys.cn

TS:   await fetch(url)
来源：http://txc.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yry.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://fnx.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://qkp.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rjl.fzhhl.top

[L02] 发送 POST JSON
来源：http://kdb.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://txa.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dtw.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwp.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmj.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mbo.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eer.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ycz.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eem.epnwcf.com

[L03] 设置自定义请求头
来源：http://uhz.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ytf.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fqj.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mos.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbi.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gzy.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oyc.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fwf.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fak.cucudq.cn

[L04] 设置超时
来源：http://jza.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://lqb.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bkz.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rdy.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bax.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lff.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gkv.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qql.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vya.fktsv.cn

[L05] 上传文件（multipart）
来源：http://xve.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fuq.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kry.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jsp.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vgd.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://juw.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bdh.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://roe.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mnu.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://zbx.316326.xyz

Py:   resp.json()
来源：http://cmz.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://nbc.epnwcf.com

JS:   await resp.json()
来源：http://ltw.tarul.cn

TS:   await resp.json()
来源：http://bkq.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://toz.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eqc.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://ugr.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bhe.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://vxj.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sai.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lan.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://zcr.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://kun.yj20258888.top

Java: resp.statusCode()
来源：http://xoy.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://pac.ivvv.top

Ruby: resp.code.to_i
来源：http://nrh.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://yoo.tanke756.top

[L08] 并发请求多个地址
来源：http://ebu.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jah.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://xop.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cwu.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izn.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pbn.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aph.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zhq.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ebf.svipenyu.cn

================================================================================
来源：http://yeu.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://mnk.ywan-chungtsiang.top

================================================================================
来源：http://gtm.chenzaomai.com

[M01] 读取命令行参数
来源：http://myz.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://jir.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://ell.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://kdk.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://yiu.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://qyu.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://eom.hesvh.cn

Ruby: ARGV
来源：http://egw.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://uhq.zdbjq.cn

[M02] 读取环境变量
来源：http://qtu.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://vfq.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xdf.hywenlv.cn

JS:   process.env.HOME
来源：http://tus.pengpengdd.cyou

TS:   process.env.HOME
来源：http://gmj.ydzc1.top

Java: System.getenv("HOME")
来源：http://bso.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://syf.uphjek.com

Ruby: ENV["HOME"]
来源：http://zpc.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hsq.zhiwuduotai.top

[M03] 执行外部命令
来源：http://dmu.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tse.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vye.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fna.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pqt.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blj.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://xhf.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://czl.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://ylo.ehwqpu.com

[M04] 获取当前工作目录
来源：http://ayp.bbcook.cn

Py:   os.getcwd()
来源：http://bry.chenlongwang.top

PHP:  getcwd();
来源：http://gnp.9152youxi.cn

JS:   process.cwd()
来源：http://ygw.cheryme.top

TS:   process.cwd()
来源：http://rbc.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://cvx.ybcxt.top

Go:   os.Getwd()
来源：http://haa.haohaochexian.top

Ruby: Dir.pwd
来源：http://hkx.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://aut.tianlin.xyz

[M05] 设置退出码
来源：http://doy.hcnkem.com

Py:   sys.exit(1)
来源：http://ubs.hnxiangtu.top

PHP:  exit(1);
来源：http://njf.hesvh.cn

JS:   process.exit(1)
来源：http://soj.nwbrower.top

TS:   process.exit(1)
来源：http://icn.cashguo.top

Java: System.exit(1)
来源：http://cwl.hywenlv.cn

Go:   os.Exit(1)
来源：http://rud.fktsv.cn

Ruby: exit 1
来源：http://hzd.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hte.yueranfly.top

[M06] 向标准错误输出
来源：http://yln.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://znb.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mgx.hywenlv.cn

JS:   console.error("err")
来源：http://kto.gaohongyu789.top

TS:   console.error("err")
来源：http://zgx.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://bsx.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mgo.cashguo.top

Ruby: warn "err"
来源：http://dqd.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://qnl.ydzc1.top

[M07] 判断是否为主入口
来源：http://kgj.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://dnh.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fei.havefunace.top

JS:   require.main === module
来源：http://udq.c1oappe.top

TS:   require.main === module
来源：http://eag.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://mmx.xziqi.cn

Go:   func main()
来源：http://koz.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fuq.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://cwp.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://jig.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://jlz.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://rzz.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://cmu.cdnleiting.top

TS:   process.platform;  process.version
来源：http://ghy.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wbf.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cee.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zpx.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wyl.jinghuilouyu.cn

================================================================================
来源：http://jzu.tarul.cn

N. 数据结构与算法
来源：http://vci.ywan-chungtsiang.top

================================================================================
来源：http://qpe.pycfn.com

[N01] 二分查找（有序数组）
来源：http://lyh.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cgu.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rwa.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ylx.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wop.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://ngw.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://ppk.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://asx.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://rku.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://ols.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://ogt.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vmi.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rtx.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zfe.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://are.hesvh.cn

Go:   slices.Sort(arr)
来源：http://mwe.jyoumei.cn

Ruby: arr.sort
来源：http://axx.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iea.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://gue.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bix.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://jvf.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zge.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ysk.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ucv.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tnv.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fuu.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://arg.aizwys.cn

[N04] 斐波那契数列
来源：http://btq.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vaa.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ubf.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nsm.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nxg.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hqm.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fry.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bwy.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eua.yvedp.cn

[N05] 最大公约数
来源：http://tju.fehbvm.com

Py:   math.gcd(a, b)
来源：http://pio.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://omm.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wua.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wgb.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cbc.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ial.316326.xyz

Ruby: a.gcd(b)
来源：http://len.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ipn.52xcode.cn

[N06] 判断回文字符串
来源：http://dzv.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://abs.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://ddo.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://psp.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://tqd.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ffe.tarul.cn

Go:   // 双指针从两端比较
来源：http://zax.fzhhl.top

Ruby: s == s.reverse
来源：http://nsf.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://hyn.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://iqj.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kyj.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dxr.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://agk.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://ypv.yfazqb.com

Java: // 手写 HashMap
来源：http://llg.yfazqb.com

Go:   // 手写 map[int]int
来源：http://hag.yj202588.top

Ruby: // 手写 Hash
来源：http://gnb.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://obz.quarkkingdee.top

[N08] 生成全排列
来源：http://qpy.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://hxq.daxiang520.top

PHP:  // 手写递归交换
来源：http://tsr.vehdjk.com

JS:   // 手写回溯递归
来源：http://amy.yuxming.cn

TS:   // 手写回溯递归
来源：http://xva.yfazqb.com

Java: // 手写回溯递归
来源：http://rtd.iojbl.cn

Go:   // 手写回溯递归
来源：http://igi.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://ozc.meibo888.top

C#:   // 手写回溯递归
来源：http://fgx.fehbvm.com

[N09] 栈与队列
来源：http://fwa.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://owc.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ijb.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vdx.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://voo.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bdy.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wvu.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://joe.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://idb.hywenlv.cn

[N10] 链表节点定义
来源：http://okv.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zuo.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aro.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ogi.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nzq.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://wjo.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://gfw.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xuq.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mof.hcnkem.com

[N11] 二叉树中序遍历
来源：http://wtk.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mci.bbcook.cn

PHP:  // 手写递归函数
来源：http://nvx.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rwd.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipf.ctjpmb.com

Java: // 手写递归
来源：http://qsd.yonumen.top

Go:   // 手写递归
来源：http://kls.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jxu.sufxvd.cn

C#:   // 手写递归
来源：http://smr.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mvr.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xbt.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pbo.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tnu.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovw.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rqt.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rmh.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tdr.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://msx.zhongyouzk.top

================================================================================
来源：http://njz.jqgfzy.top

O. 并发与异步
来源：http://noh.ivvv.top

================================================================================
来源：http://yxo.9152youxi.cn

[O01] 启动一个线程
来源：http://xbf.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xsz.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://typ.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wdc.tanke756.top

TS:   // 同 JS
来源：http://tta.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://ngz.chenlongwang.top

Go:   go f()
来源：http://mgv.yongpay.top

Ruby: Thread.new { f }
来源：http://joy.c1oappe.top

C#:   Task.Run(() => F());
来源：http://egn.9152youxi.cn

[O02] 使用线程池
来源：http://owu.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gry.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ngh.ivvv.top

JS:   // worker_threads 线程池
来源：http://suf.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://pud.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://qjr.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dvd.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://agx.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rso.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://llp.daria6918.cn

Py:   with lock: shared += 1
来源：http://eyw.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://hvf.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gbk.pengpengdd.cyou

TS:   // 同 JS
来源：http://stk.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://rza.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jsh.guannengcc.top


<!-- 参考信息 -->