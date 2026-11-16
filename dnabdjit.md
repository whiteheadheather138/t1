代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmh.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hwv.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://srq.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyd.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://swf.jinqigfzy.top

[K07] 进制转换
来源：http://bmk.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yij.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jir.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xyi.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cvi.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rdg.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ake.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dzk.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lrh.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://xzu.yongpay.top

Py:   pickle.dumps(obj)
来源：http://gzr.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lrr.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://yke.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://pgp.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fai.xuetiantiany.cn

Go:   encoding/gob
来源：http://gtc.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://mbc.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rqk.xylfe.cn

================================================================================
来源：http://dpj.zhixingplan.top

L. 网络请求
来源：http://nvo.ydzc1.top

================================================================================
来源：http://hji.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://brn.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oqn.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tyx.fengsongda.top

JS:   await fetch(url)
来源：http://gzb.jlsjyb.cn

TS:   await fetch(url)
来源：http://hvv.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tjm.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://zcp.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://veh.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pmm.svipenyu.cn

[L02] 发送 POST JSON
来源：http://tuo.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kbb.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wgz.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bjj.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hnc.meibo888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cbm.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eze.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://etr.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://swm.bjfxy.top

[L03] 设置自定义请求头
来源：http://nyk.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gxz.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lsb.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uop.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxx.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://spz.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://won.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://khy.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oqy.hcnkem.com

[L04] 设置超时
来源：http://djz.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://wdd.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hor.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azc.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://csd.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oji.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gcx.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvf.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://exz.xinyue.icu

[L05] 上传文件（multipart）
来源：http://mma.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ipz.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rvr.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ari.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyr.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kjj.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zbq.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mfg.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iwi.shuidangran.top

[L06] 解析响应为 JSON
来源：http://byq.52xcode.cn

Py:   resp.json()
来源：http://hhm.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://gbo.jiagoushi.top

JS:   await resp.json()
来源：http://xgo.sysykeji.top

TS:   await resp.json()
来源：http://pzj.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ssc.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jyc.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://gxf.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://atu.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://akd.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hrd.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ssj.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://mub.yongpay.top

TS:   resp.ok;  resp.status
来源：http://rnf.yueranfly.top

Java: resp.statusCode()
来源：http://grm.hysaishi.cn

Go:   resp.StatusCode
来源：http://ciy.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://cna.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://xpf.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://exl.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://shl.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://ogm.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://abc.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aig.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ahc.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yef.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lpm.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bzj.zycfv.cn

================================================================================
来源：http://sbt.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://zxn.jqgfzy.top

================================================================================
来源：http://tvc.dashuyun.cn

[M01] 读取命令行参数
来源：http://qtw.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://eei.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://hxr.pycfn.com

JS:   process.argv.slice(2)
来源：http://qlb.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://tmk.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://agb.xylfe.cn

Go:   os.Args[1:]
来源：http://vhm.sxryk.cn

Ruby: ARGV
来源：http://rls.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://zfy.chenzaomai.com

[M02] 读取环境变量
来源：http://roa.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://gky.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://moq.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://rla.cdnleiting.top

TS:   process.env.HOME
来源：http://tvg.hcnkem.com

Java: System.getenv("HOME")
来源：http://avz.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://naf.andypj.xyz

Ruby: ENV["HOME"]
来源：http://slc.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mhp.kuanghao11.cn

[M03] 执行外部命令
来源：http://bqg.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rki.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vqi.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://dgy.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uzs.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cvk.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qly.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://bsb.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://rup.ydzc1.top

[M04] 获取当前工作目录
来源：http://vjt.yj20258.top

Py:   os.getcwd()
来源：http://uaq.jiagoushi.top

PHP:  getcwd();
来源：http://ptu.pengpengdd.cyou

JS:   process.cwd()
来源：http://zmz.hnxiangtu.top

TS:   process.cwd()
来源：http://rcm.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://kqv.shuidangran.top

Go:   os.Getwd()
来源：http://wnx.gogol.net.cn

Ruby: Dir.pwd
来源：http://btl.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://zxn.guowangkeji.top

[M05] 设置退出码
来源：http://qbk.sxryk.cn

Py:   sys.exit(1)
来源：http://ivj.chenjidiqi.icu

PHP:  exit(1);
来源：http://nbd.dashuyun.cn

JS:   process.exit(1)
来源：http://mdr.yanxiufei.cn

TS:   process.exit(1)
来源：http://una.redwolf501.top

Java: System.exit(1)
来源：http://rlf.redwolf501.top

Go:   os.Exit(1)
来源：http://znz.xuanzx.com

Ruby: exit 1
来源：http://xhe.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pvq.cucudq.cn

[M06] 向标准错误输出
来源：http://gml.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://uwi.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gqf.hnxiangtu.top

JS:   console.error("err")
来源：http://kxr.iojbl.cn

TS:   console.error("err")
来源：http://tyx.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://wpd.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vrd.yongpay.top

Ruby: warn "err"
来源：http://pms.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://znv.svipenyu.cn

[M07] 判断是否为主入口
来源：http://xuo.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://fsi.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oni.yj20258.top

JS:   require.main === module
来源：http://dew.aizwys.cn

TS:   require.main === module
来源：http://pfn.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://bsn.ppjwa.cn

Go:   func main()
来源：http://wki.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://szu.smart0.xyz

C#:   static void Main(string[] args)
来源：http://icb.ivvv.top

[M08] 获取系统与运行时信息
来源：http://mdo.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://ble.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://wtv.ctjpmb.com

JS:   process.platform;  process.version
来源：http://pah.hywenlv.cn

TS:   process.platform;  process.version
来源：http://kno.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fdw.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rex.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ysa.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://piu.gogol.net.cn

================================================================================
来源：http://xxd.guannengcc.top

N. 数据结构与算法
来源：http://zwx.yongpay.top

================================================================================
来源：http://gpr.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://hqi.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://xcv.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sqn.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bhg.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jic.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://pfr.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://ywd.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ozd.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://vgc.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://sfk.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://oan.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cpd.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://icc.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://syu.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ytd.52xcode.cn

Go:   slices.Sort(arr)
来源：http://xsn.tianlin.xyz

Ruby: arr.sort
来源：http://kik.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yfd.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://spn.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vlq.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://cvn.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xwt.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ncg.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mgn.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tah.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uzr.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oov.mhx1999.top

[N04] 斐波那契数列
来源：http://swt.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zky.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uky.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kya.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://orh.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lxv.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cnc.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cbg.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://efv.uphjek.com

[N05] 最大公约数
来源：http://hsi.redwolf501.top

Py:   math.gcd(a, b)
来源：http://wkf.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lif.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://epc.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://smf.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zle.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kih.yj20258.top

Ruby: a.gcd(b)
来源：http://hbh.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://exh.chenlongwang.top

[N06] 判断回文字符串
来源：http://fpi.yuxming.cn

Py:   s == s[::-1]
来源：http://hhy.fzhhl.top

PHP:  $s === strrev($s);
来源：http://iev.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://uea.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://gua.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lcj.bjfxy.top

Go:   // 双指针从两端比较
来源：http://wqr.mhx1999.top

Ruby: s == s.reverse
来源：http://bas.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://hpb.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://tbt.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yzv.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bdt.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://kke.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://cov.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://mwh.birdmap.top

Go:   // 手写 map[int]int
来源：http://pcx.chenlongwang.top

Ruby: // 手写 Hash
来源：http://kwg.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://scg.iojbl.cn

[N08] 生成全排列
来源：http://xbl.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://vdq.zhixingplan.top

PHP:  // 手写递归交换
来源：http://mes.nwbrower.top

JS:   // 手写回溯递归
来源：http://zoh.cdnleiting.top

TS:   // 手写回溯递归
来源：http://fjf.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://vrl.ppjwa.cn

Go:   // 手写回溯递归
来源：http://tty.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://eti.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://sxv.sysykeji.top

[N09] 栈与队列
来源：http://cec.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mur.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eci.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oya.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ksh.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gbm.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yaw.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xyl.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jne.haohaochexian.top

[N10] 链表节点定义
来源：http://dmy.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnc.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uzj.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mkt.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vrz.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://ift.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hti.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tgv.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gkr.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://hhu.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vyz.guowangkeji.top

PHP:  // 手写递归函数
来源：http://nkr.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsc.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qes.shuidangran.top

Java: // 手写递归
来源：http://npw.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://xjk.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ylr.haohaochexian.top

C#:   // 手写递归
来源：http://cad.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rno.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://afl.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://frl.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nox.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dnk.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://edd.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zsf.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sec.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vor.fengsongda.top

================================================================================
来源：http://xew.tanke756.top

O. 并发与异步
来源：http://svu.ctjpmb.com

================================================================================
来源：http://ron.chenzaomai.com

[O01] 启动一个线程
来源：http://eya.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gpk.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fwc.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sal.nwbrower.top

TS:   // 同 JS
来源：http://tsq.sxryk.cn

Java: new Thread(() -> f()).start()
来源：http://nqk.9152youxi.cn

Go:   go f()
来源：http://oaq.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://pno.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://mhb.smart0.xyz

[O02] 使用线程池
来源：http://crk.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://swm.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lbd.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://tbu.fktsv.cn


<!-- 参考信息 -->