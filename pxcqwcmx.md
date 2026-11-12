代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://irc.hysaishi.cn

[K07] 进制转换
来源：http://enf.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dui.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tev.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fkp.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lay.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ebz.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://juf.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xyc.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ank.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://foj.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://ypc.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ffk.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://bxx.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://ipd.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qxh.jinghuilouyu.cn

Go:   encoding/gob
来源：http://ddo.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://dnc.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lew.xuanzx.com

================================================================================
来源：http://lan.shzxlz.cn

L. 网络请求
来源：http://fxc.jianghu66.top

================================================================================
来源：http://bik.yfazqb.com

[L01] 发送 GET 请求
来源：http://zyy.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://reu.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wye.sxryk.cn

JS:   await fetch(url)
来源：http://mvk.zycfv.cn

TS:   await fetch(url)
来源：http://hpu.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://smv.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://yfz.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ohp.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://knl.andypj.xyz

[L02] 发送 POST JSON
来源：http://ggk.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vnl.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nic.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cix.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lki.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zfs.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wrq.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lqk.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uge.mhx1999.top

[L03] 设置自定义请求头
来源：http://qcf.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lyn.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qee.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wje.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ueb.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fix.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://clk.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://unc.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ucn.daxiang520.top

[L04] 设置超时
来源：http://ref.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://fdo.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tvw.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mho.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tyq.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ruo.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qjz.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fsc.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qgf.bbcook.cn

[L05] 上传文件（multipart）
来源：http://qhg.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cna.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pns.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pws.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uwj.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bui.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vaf.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://llb.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vtm.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://juj.fanxiaobao.xyz

Py:   resp.json()
来源：http://pmy.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://jjl.guowangkeji.top

JS:   await resp.json()
来源：http://gmb.shanyushiyangtech.top

TS:   await resp.json()
来源：http://nin.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oby.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xtu.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://tfv.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ihz.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://qsy.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tve.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://avr.uphjek.com

JS:   resp.ok;  resp.status
来源：http://dln.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://qyp.jqgfzy.top

Java: resp.statusCode()
来源：http://uvi.hnqzz.top

Go:   resp.StatusCode
来源：http://sgs.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://nqe.tanke756.top

C#:   (int)resp.StatusCode
来源：http://zez.hesvh.cn

[L08] 并发请求多个地址
来源：http://xpq.cdnleiting.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dkz.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://qju.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sfa.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tkp.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://suh.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lal.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oxy.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bnl.aibaodan.cn

================================================================================
来源：http://dni.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://cvi.xuanzx.com

================================================================================
来源：http://hut.hnxiangtu.top

[M01] 读取命令行参数
来源：http://bvk.yueranfly.top

Py:   sys.argv[1:]
来源：http://jzd.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://axy.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://njc.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://wws.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://zum.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://sgc.fehbvm.com

Ruby: ARGV
来源：http://cqm.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://wrx.yanxiufei.cn

[M02] 读取环境变量
来源：http://ohb.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://swi.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nyt.yanxiufei.cn

JS:   process.env.HOME
来源：http://jjz.jqgufenzy.top

TS:   process.env.HOME
来源：http://gbo.xziqi.cn

Java: System.getenv("HOME")
来源：http://bik.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://szg.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://tdx.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xpd.ydjk.org.cn

[M03] 执行外部命令
来源：http://kvw.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tit.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ypd.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ghk.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xqj.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nmp.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ufx.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://efs.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://ati.hcnkem.com

[M04] 获取当前工作目录
来源：http://xgp.hnqzz.top

Py:   os.getcwd()
来源：http://sdl.yuanzhike.top

PHP:  getcwd();
来源：http://rtp.jinghuilouyu.cn

JS:   process.cwd()
来源：http://yqg.c1oappe.top

TS:   process.cwd()
来源：http://smw.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://hma.316326.xyz

Go:   os.Getwd()
来源：http://twe.jinqigufen.top

Ruby: Dir.pwd
来源：http://ctz.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ruo.fktsv.cn

[M05] 设置退出码
来源：http://niz.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://rzs.nanxinkj.top

PHP:  exit(1);
来源：http://mef.316326.xyz

JS:   process.exit(1)
来源：http://xdy.yj20258.top

TS:   process.exit(1)
来源：http://eho.hnxiangtu.top

Java: System.exit(1)
来源：http://oeo.fzhhl.top

Go:   os.Exit(1)
来源：http://jta.yueranfly.top

Ruby: exit 1
来源：http://dve.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rxd.gogol.net.cn

[M06] 向标准错误输出
来源：http://xav.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://sjz.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gdh.fengsongda.top

JS:   console.error("err")
来源：http://lkd.nanxinkj.top

TS:   console.error("err")
来源：http://tfp.tian-w.cn

Java: System.err.println("err")
来源：http://mqz.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ccz.nanxuanxn.top

Ruby: warn "err"
来源：http://htt.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://pxt.vehdjk.com

[M07] 判断是否为主入口
来源：http://ffu.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://pgy.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mgs.redwolf501.top

JS:   require.main === module
来源：http://jhe.zdqjudy.top

TS:   require.main === module
来源：http://qnx.hcnkem.com

Java: public static void main(String[] args)
来源：http://ucu.sjlbkw.cn

Go:   func main()
来源：http://pki.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ezq.uphjek.com

C#:   static void Main(string[] args)
来源：http://sfo.cashguo.top

[M08] 获取系统与运行时信息
来源：http://lqg.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://mrk.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://bqc.fengsongda.top

JS:   process.platform;  process.version
来源：http://luc.aibaodan.cn

TS:   process.platform;  process.version
来源：http://zbb.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iya.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xnz.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dii.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://whi.jqgufenzy.top

================================================================================
来源：http://wha.ydzc1.top

N. 数据结构与算法
来源：http://ctm.yueranfly.top

================================================================================
来源：http://btt.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://pda.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://kqe.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yih.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jnt.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bbf.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://onl.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://eag.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xvk.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nhn.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://xpe.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://flo.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gye.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xvv.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ypm.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zto.tanke756.top

Go:   slices.Sort(arr)
来源：http://agc.yuxming.cn

Ruby: arr.sort
来源：http://leo.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://ara.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://kwe.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uiz.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://nks.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vgs.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgc.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eqw.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gqc.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xxq.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yid.guannengcc.top

[N04] 斐波那契数列
来源：http://wmu.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hlz.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sjf.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqw.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpl.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xlh.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zmj.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zkw.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jni.hesvh.cn

[N05] 最大公约数
来源：http://ttj.yj202588.top

Py:   math.gcd(a, b)
来源：http://uwg.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gki.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hvj.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://psy.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yxl.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://utm.shzxlz.cn

Ruby: a.gcd(b)
来源：http://jhn.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://luv.hammf.cn

[N06] 判断回文字符串
来源：http://zfr.yvedp.cn

Py:   s == s[::-1]
来源：http://ftv.xinyue.icu

PHP:  $s === strrev($s);
来源：http://gns.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://xxe.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://tze.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ode.yuxming.cn

Go:   // 双指针从两端比较
来源：http://cub.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://yfj.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dex.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://fwm.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://czp.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hih.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gkh.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://lra.yuxming.cn

Java: // 手写 HashMap
来源：http://mzs.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://ffa.chenlongwang.top

Ruby: // 手写 Hash
来源：http://elv.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://yvx.xziqi.cn

[N08] 生成全排列
来源：http://wsc.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://iyz.bbcook.cn

PHP:  // 手写递归交换
来源：http://lkg.yuxming.cn

JS:   // 手写回溯递归
来源：http://ikn.yj20258888.top

TS:   // 手写回溯递归
来源：http://yna.xylfe.cn

Java: // 手写回溯递归
来源：http://shd.tianlin.xyz

Go:   // 手写回溯递归
来源：http://mbv.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://ons.nwbrower.top

C#:   // 手写回溯递归
来源：http://iqt.shanyushiyangtech.top

[N09] 栈与队列
来源：http://dci.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eyl.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eib.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tfl.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ljg.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://paj.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fjs.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://crm.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vgh.yueranfly.top

[N10] 链表节点定义
来源：http://gvp.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uog.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xsq.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://arj.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ves.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://soe.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lnq.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ent.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://jhz.cucudq.cn

[N11] 二叉树中序遍历
来源：http://kqd.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zsh.aibaodan.cn

PHP:  // 手写递归函数
来源：http://iwh.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wpo.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqr.shanyushiyangtech.top

Java: // 手写递归
来源：http://ybf.ctjpmb.com

Go:   // 手写递归
来源：http://dwx.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fxg.redwolf501.top

C#:   // 手写递归
来源：http://itx.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xng.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ijv.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://due.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ycq.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vov.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pcu.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pfb.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xdx.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xyo.cdnleiting.top

================================================================================
来源：http://cid.redwolf501.top

O. 并发与异步
来源：http://mne.fktsv.cn

================================================================================
来源：http://cbv.cucudq.cn

[O01] 启动一个线程
来源：http://lyq.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nki.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vyl.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://opa.52xcode.cn

TS:   // 同 JS
来源：http://inf.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://hxf.xuanzx.com

Go:   go f()
来源：http://yfu.nanxinkj.top

Ruby: Thread.new { f }
来源：http://drz.ivvv.top

C#:   Task.Run(() => F());
来源：http://ksn.hongshengwenyu.top

[O02] 使用线程池
来源：http://xik.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://exq.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jjv.xinyue.icu

JS:   // worker_threads 线程池
来源：http://ujc.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://exo.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qvp.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wiz.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qkt.guannengcc.top


<!-- 参考信息 -->