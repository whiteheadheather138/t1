代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wue.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://avh.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iwy.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hpb.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://otn.kuanghao11.cn

[K07] 进制转换
来源：http://xml.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://twg.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ajf.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vwj.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xee.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cpm.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eqk.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vmq.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fry.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://fss.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://asa.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zla.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://hum.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://vse.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hrv.chenzaomai.com

Go:   encoding/gob
来源：http://zyh.sweek.top

Ruby: Marshal.dump(obj)
来源：http://qxy.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ygn.nanxinkj.top

================================================================================
来源：http://vng.yvedp.cn

L. 网络请求
来源：http://wmz.tianlin.xyz

================================================================================
来源：http://bdx.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://hlf.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vjh.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ddv.9152youxi.cn

JS:   await fetch(url)
来源：http://kbm.yj20258888.top

TS:   await fetch(url)
来源：http://flj.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dox.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://fid.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://txn.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yke.fzhhl.top

[L02] 发送 POST JSON
来源：http://fyr.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gtg.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xqp.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://apr.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://amu.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://itc.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uhf.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nod.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oad.ydzc1.top

[L03] 设置自定义请求头
来源：http://xir.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mng.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fmx.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wgl.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ukc.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cxp.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rzv.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pmm.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hyy.ppjwa.cn

[L04] 设置超时
来源：http://bxm.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://uwg.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kef.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mgc.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nlo.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dri.zhengqikj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vbd.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://niq.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tzm.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://elu.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pdd.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gkv.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://spb.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wwu.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bra.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ykv.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ezk.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmm.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://pvr.316326.xyz

Py:   resp.json()
来源：http://jiu.yongpay.top

PHP:  json_decode($body, true);
来源：http://vwl.havefunace.top

JS:   await resp.json()
来源：http://jja.316326.xyz

TS:   await resp.json()
来源：http://kro.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xpu.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wgw.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://zuc.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nna.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://xoc.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbw.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjv.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://svr.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://xno.yanxiufei.cn

Java: resp.statusCode()
来源：http://tkx.sxryk.cn

Go:   resp.StatusCode
来源：http://tug.bjfxy.top

Ruby: resp.code.to_i
来源：http://ubd.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://ewp.guannengcc.top

[L08] 并发请求多个地址
来源：http://wop.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cpa.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://kvf.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzd.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oxw.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://emr.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gwr.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vwb.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cft.sxryk.cn

================================================================================
来源：http://aeu.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://xrg.hysaishi.cn

================================================================================
来源：http://npd.nanxinkj.top

[M01] 读取命令行参数
来源：http://sso.sweek.top

Py:   sys.argv[1:]
来源：http://jeq.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://tqh.daria6918.cn

JS:   process.argv.slice(2)
来源：http://hpg.fktsv.cn

TS:   process.argv.slice(2)
来源：http://zls.cheryme.top

Java: args 数组（main 方法参数）
来源：http://djc.quarkkingdee.top

Go:   os.Args[1:]
来源：http://irt.cqqwz.cn

Ruby: ARGV
来源：http://cja.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://ohu.smart0.xyz

[M02] 读取环境变量
来源：http://fxl.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://orx.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sbo.haohaochexian.top

JS:   process.env.HOME
来源：http://kzt.jiagoushi.top

TS:   process.env.HOME
来源：http://eeb.pycfn.com

Java: System.getenv("HOME")
来源：http://ake.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xtw.smart0.xyz

Ruby: ENV["HOME"]
来源：http://xtr.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qvk.meibo888.top

[M03] 执行外部命令
来源：http://gmx.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ltq.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lsb.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mfu.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sna.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ehw.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://duw.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ygw.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://cac.yfazqb.com

[M04] 获取当前工作目录
来源：http://rmr.yj20258888.top

Py:   os.getcwd()
来源：http://rcj.zhiwuduotai.top

PHP:  getcwd();
来源：http://ybl.cucudq.cn

JS:   process.cwd()
来源：http://wjt.sjlbkw.cn

TS:   process.cwd()
来源：http://wfq.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://zlc.nanxinkj.top

Go:   os.Getwd()
来源：http://qtg.yonumen.top

Ruby: Dir.pwd
来源：http://wnz.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://txn.xuetiantiany.cn

[M05] 设置退出码
来源：http://kfi.bbcook.cn

Py:   sys.exit(1)
来源：http://bll.jqgufenzy.top

PHP:  exit(1);
来源：http://hcm.c1oappe.top

JS:   process.exit(1)
来源：http://piu.quarkkingdee.top

TS:   process.exit(1)
来源：http://tuo.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://zuz.cashguo.top

Go:   os.Exit(1)
来源：http://djc.yj20258.top

Ruby: exit 1
来源：http://cdo.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rwg.jqgfzy.top

[M06] 向标准错误输出
来源：http://zre.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://jlv.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://udh.dianchejie.cn

JS:   console.error("err")
来源：http://ksk.aizwys.cn

TS:   console.error("err")
来源：http://elq.sysykeji.top

Java: System.err.println("err")
来源：http://kkt.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rwu.daria6918.cn

Ruby: warn "err"
来源：http://jak.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://oqc.aizwys.cn

[M07] 判断是否为主入口
来源：http://keo.cashguo.top

Py:   if __name__ == "__main__":
来源：http://wuc.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pce.ybcxt.top

JS:   require.main === module
来源：http://tqo.yj20258888.top

TS:   require.main === module
来源：http://ghr.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://pbo.smart0.xyz

Go:   func main()
来源：http://qgz.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qmv.xinyue.icu

C#:   static void Main(string[] args)
来源：http://gug.cheryme.top

[M08] 获取系统与运行时信息
来源：http://xnn.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://dsy.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://dte.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://swx.chenzaomai.com

TS:   process.platform;  process.version
来源：http://qbl.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yvq.9152youxi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fzg.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bpx.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iso.quarkkingdee.top

================================================================================
来源：http://dvc.yfazqb.com

N. 数据结构与算法
来源：http://wrz.yonumen.top

================================================================================
来源：http://ekb.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://nuz.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xhr.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://itk.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fio.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbj.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://squ.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://wdl.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fne.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://qxz.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://hqb.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://irg.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zpg.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://giz.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://wya.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://apz.tanke756.top

Go:   slices.Sort(arr)
来源：http://bwm.chenzaomai.com

Ruby: arr.sort
来源：http://ccj.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://pmv.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://bot.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kyy.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://rir.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oyn.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wdw.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://efb.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xfv.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mav.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://rak.316326.xyz

[N04] 斐波那契数列
来源：http://fgx.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rbw.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iwa.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iyi.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hrd.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hir.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hrl.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zhq.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sfz.epnwcf.com

[N05] 最大公约数
来源：http://tfc.316326.xyz

Py:   math.gcd(a, b)
来源：http://tof.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bpa.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrr.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uzi.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iuz.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://luh.cqqwz.cn

Ruby: a.gcd(b)
来源：http://jbo.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zhb.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://bra.pycfn.com

Py:   s == s[::-1]
来源：http://lli.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://ots.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://grm.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://vyk.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jix.sysykeji.top

Go:   // 双指针从两端比较
来源：http://exp.birdmap.top

Ruby: s == s.reverse
来源：http://epa.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ziu.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://cly.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zev.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lgm.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://fvm.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://jtz.nanxuanxn.top

Java: // 手写 HashMap
来源：http://awz.hesvh.cn

Go:   // 手写 map[int]int
来源：http://iyc.yvedp.cn

Ruby: // 手写 Hash
来源：http://ohl.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ldj.hysaishi.cn

[N08] 生成全排列
来源：http://chc.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://luz.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://nnu.hnqzz.top

JS:   // 手写回溯递归
来源：http://vjw.tarul.cn

TS:   // 手写回溯递归
来源：http://fpf.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://lry.yueranfly.top

Go:   // 手写回溯递归
来源：http://zmt.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://cju.wangdashe.top

C#:   // 手写回溯递归
来源：http://kmu.zdqjudy.top

[N09] 栈与队列
来源：http://qnj.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vuf.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dvc.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fhw.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ehp.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jmd.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fjh.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tjj.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zng.ctjpmb.com

[N10] 链表节点定义
来源：http://tut.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kqc.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zgr.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zgq.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://doe.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://odi.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://rsz.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://smq.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iba.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://drv.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qoe.iojbl.cn

PHP:  // 手写递归函数
来源：http://izj.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovq.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://olq.hysaishi.cn

Java: // 手写递归
来源：http://xdb.ybcxt.top

Go:   // 手写递归
来源：http://vcf.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lqu.hfpthk.cn

C#:   // 手写递归
来源：http://ekk.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://chx.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gfo.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yiq.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nla.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qst.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://djc.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://szz.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jut.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pfk.jqgfzy.top

================================================================================
来源：http://vhd.smart0.xyz

O. 并发与异步
来源：http://bpb.shanyushiyangkeji.top

================================================================================
来源：http://tnn.gzhubu.top

[O01] 启动一个线程
来源：http://sia.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wse.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ojc.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gzg.chenlongwang.top

TS:   // 同 JS
来源：http://ouo.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://wjj.ydzc1.top

Go:   go f()
来源：http://tzw.ydzc1.top

Ruby: Thread.new { f }
来源：http://vla.yj20258.top

C#:   Task.Run(() => F());
来源：http://pxf.gogol.net.cn

[O02] 使用线程池
来源：http://uyp.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://clh.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ycp.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://szm.shzxlz.cn


<!-- 参考信息 -->