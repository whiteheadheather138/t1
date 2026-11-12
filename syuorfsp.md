代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://web.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://cyr.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://rgk.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://uvf.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ria.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://svt.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://neo.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cxe.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://txb.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://flr.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwc.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oco.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pul.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dlo.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ucy.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tac.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yzt.yj202588.top

[K07] 进制转换
来源：http://jby.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xge.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jye.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hap.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kac.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mws.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ovy.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tbf.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zjp.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://rtb.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://iot.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ipi.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://trt.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://kdd.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gac.gzhubu.top

Go:   encoding/gob
来源：http://ubp.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://nnd.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nfn.sufxvd.cn

================================================================================
来源：http://zte.xuanzx.com

L. 网络请求
来源：http://tyy.xuetiantiany.cn

================================================================================
来源：http://wpz.yfazqb.com

[L01] 发送 GET 请求
来源：http://kub.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zle.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ase.yfazqb.com

JS:   await fetch(url)
来源：http://lev.andypj.xyz

TS:   await fetch(url)
来源：http://kdh.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wmk.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://zxg.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hwj.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gqt.yangfankeji.com

[L02] 发送 POST JSON
来源：http://knb.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kmk.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ndz.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ggz.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tzh.meibo888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ukg.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://miq.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gxc.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uro.daxiang520.top

[L03] 设置自定义请求头
来源：http://aqf.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xqe.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://alv.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lwa.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wki.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ksg.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lli.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ied.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vaa.feifeiyinyue.top

[L04] 设置超时
来源：http://wcn.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://gpm.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://frf.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://krn.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ycf.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://stx.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fmt.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zqq.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uiq.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://kmj.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://utv.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vig.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://alt.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uan.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cyb.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hcn.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oey.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ekb.pycfn.com

[L06] 解析响应为 JSON
来源：http://zvd.tarul.cn

Py:   resp.json()
来源：http://myb.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://yqs.gaohongyu789.top

JS:   await resp.json()
来源：http://cgu.hcnkem.com

TS:   await resp.json()
来源：http://csv.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nzv.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mgx.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://ljs.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cvl.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://ssx.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jyk.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bwh.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://apq.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://uyv.yanxiufei.cn

Java: resp.statusCode()
来源：http://hdb.zhijiandao.cn

Go:   resp.StatusCode
来源：http://dwp.hnqzz.top

Ruby: resp.code.to_i
来源：http://bmu.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://lut.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://fny.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wsm.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://sny.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gau.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdo.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lvg.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wyg.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gmv.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zjd.cucudq.cn

================================================================================
来源：http://ash.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://jrt.jinyuanbaomall.cn

================================================================================
来源：http://bbv.hfpthk.cn

[M01] 读取命令行参数
来源：http://snu.ctjpmb.com

Py:   sys.argv[1:]
来源：http://mhv.epnwcf.com

PHP:  $argv;  $argc;
来源：http://nay.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://hle.daria6918.cn

TS:   process.argv.slice(2)
来源：http://lxt.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://bfo.xuanzx.com

Go:   os.Args[1:]
来源：http://xoh.smart0.xyz

Ruby: ARGV
来源：http://dfs.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://krx.xinyue.icu

[M02] 读取环境变量
来源：http://sep.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://dys.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cyu.hnxiangtu.top

JS:   process.env.HOME
来源：http://pyl.zdqjudy.top

TS:   process.env.HOME
来源：http://dqy.svipenyu.cn

Java: System.getenv("HOME")
来源：http://qra.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mfp.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://cwu.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pxd.guowangkeji.top

[M03] 执行外部命令
来源：http://uam.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ijj.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nap.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pkt.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://txy.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cmt.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aaj.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lpl.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://knf.pycfn.com

[M04] 获取当前工作目录
来源：http://fnv.yonumen.top

Py:   os.getcwd()
来源：http://ewl.chenlongwang.top

PHP:  getcwd();
来源：http://oux.yanxiufei.cn

JS:   process.cwd()
来源：http://fpk.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://wsy.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://kor.gogol.net.cn

Go:   os.Getwd()
来源：http://wyt.meibo888.top

Ruby: Dir.pwd
来源：http://qme.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://dnk.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://dok.yj202588.top

Py:   sys.exit(1)
来源：http://heh.sufxvd.cn

PHP:  exit(1);
来源：http://vqz.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://geo.bbcook.cn

TS:   process.exit(1)
来源：http://hbp.yueranfly.top

Java: System.exit(1)
来源：http://kli.hnxiangtu.top

Go:   os.Exit(1)
来源：http://flf.shuidangran.top

Ruby: exit 1
来源：http://bxw.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ykb.redwolf501.top

[M06] 向标准错误输出
来源：http://wyk.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://inj.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tml.jinghuilouyu.cn

JS:   console.error("err")
来源：http://rdk.gzhubu.top

TS:   console.error("err")
来源：http://ajx.epnwcf.com

Java: System.err.println("err")
来源：http://hku.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://szq.nwbrower.top

Ruby: warn "err"
来源：http://oqp.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://yjc.316326.xyz

[M07] 判断是否为主入口
来源：http://rup.ivvv.top

Py:   if __name__ == "__main__":
来源：http://ytm.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dnq.cdnleiting.top

JS:   require.main === module
来源：http://htf.hnxiangtu.top

TS:   require.main === module
来源：http://acm.smart0.xyz

Java: public static void main(String[] args)
来源：http://arz.shanyushiyangkeji.top

Go:   func main()
来源：http://mdr.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jye.fzhhl.top

C#:   static void Main(string[] args)
来源：http://yew.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://kxb.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://mck.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://wjk.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://pre.zhengqikj.top

TS:   process.platform;  process.version
来源：http://sdq.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ija.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yvn.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oxm.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dtu.shuidangran.top

================================================================================
来源：http://aks.shanyushiyangtech.top

N. 数据结构与算法
来源：http://cdt.zhiwuduotai.top

================================================================================
来源：http://ouf.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://rxe.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://ugb.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ngt.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mnf.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uro.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vow.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://khs.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xcf.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://nak.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://wjg.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://xlf.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fyq.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zqe.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xth.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qql.yj202588.top

Go:   slices.Sort(arr)
来源：http://efb.tian-w.cn

Ruby: arr.sort
来源：http://nmb.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rio.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://mpt.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zas.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://xcq.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://imu.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dtd.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://obu.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jnq.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dpp.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://jcp.zhengqikj.top

[N04] 斐波那契数列
来源：http://bsl.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ylp.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qpd.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hxu.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://puy.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fsz.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hsh.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tny.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qre.ybcxt.top

[N05] 最大公约数
来源：http://kze.iojbl.cn

Py:   math.gcd(a, b)
来源：http://qzx.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fuj.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqe.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyz.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jdk.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rax.fengsongda.top

Ruby: a.gcd(b)
来源：http://mni.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jup.snrcjt.cn

[N06] 判断回文字符串
来源：http://cxp.haohaochexian.top

Py:   s == s[::-1]
来源：http://xtu.zycfv.cn

PHP:  $s === strrev($s);
来源：http://oni.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://mvo.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://ilg.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cdt.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://mpx.smart0.xyz

Ruby: s == s.reverse
来源：http://hxk.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ppr.yj202588.top

[N07] 两数之和（返回下标）
来源：http://qjd.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://okc.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ckw.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lxp.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://voq.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://tgz.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://vnw.hywenlv.cn

Ruby: // 手写 Hash
来源：http://xuf.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://qvl.xinyue.icu

[N08] 生成全排列
来源：http://ebx.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://ays.birdmap.top

PHP:  // 手写递归交换
来源：http://tvi.pycfn.com

JS:   // 手写回溯递归
来源：http://rfs.fktsv.cn

TS:   // 手写回溯递归
来源：http://krk.52xcode.cn

Java: // 手写回溯递归
来源：http://jra.sweek.top

Go:   // 手写回溯递归
来源：http://bzu.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://mbx.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://pwf.nwbrower.top

[N09] 栈与队列
来源：http://tkm.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zgq.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tbp.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hry.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://omz.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rmh.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lhm.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hgm.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gef.havefunace.top

[N10] 链表节点定义
来源：http://wcy.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jyi.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jta.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gtc.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hgo.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://hrd.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://zvd.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wrv.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://taj.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://vzs.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qwz.svipenyu.cn

PHP:  // 手写递归函数
来源：http://fro.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bib.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmj.vehdjk.com

Java: // 手写递归
来源：http://pgt.jyoumei.cn

Go:   // 手写递归
来源：http://fgo.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ppb.hywenlv.cn

C#:   // 手写递归
来源：http://dig.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://guu.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://otx.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://daq.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eyl.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fkt.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uyj.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jrs.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uke.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ncf.ydzc1.top

================================================================================
来源：http://xtd.pycfn.com

O. 并发与异步
来源：http://gzt.tian-w.cn

================================================================================
来源：http://hpd.yanxiufei.cn

[O01] 启动一个线程
来源：http://snn.daria6918.cn


<!-- 参考信息 -->