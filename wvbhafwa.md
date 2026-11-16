代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://kpd.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://sqo.jianghu66.top

JS:   structuredClone(obj)
来源：http://iou.zhengqikj.top

TS:   structuredClone(obj)
来源：http://tib.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://npf.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bns.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zkw.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://evz.smart0.xyz

[K06] 解析 URL 查询串
来源：http://pdh.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fud.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zrr.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqq.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vyp.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnc.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://exc.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eoe.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zhd.yvedp.cn

[K07] 进制转换
来源：http://dtp.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://voq.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kxg.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xsz.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://caj.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vnj.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zvp.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lee.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://llp.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://mpu.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://cxr.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xjc.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://grh.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://rcj.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yqb.yangfankeji.com

Go:   encoding/gob
来源：http://pfs.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://ymn.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rad.vqdsnc.cn

================================================================================
来源：http://uzn.jiagoushi.top

L. 网络请求
来源：http://tho.zhoulong.xyz

================================================================================
来源：http://vti.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://bnz.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yxi.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ypx.xuanzx.com

JS:   await fetch(url)
来源：http://iyb.kuanghao11.cn

TS:   await fetch(url)
来源：http://dpj.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gfh.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://bhd.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://gmt.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bru.9152youxi.cn

[L02] 发送 POST JSON
来源：http://klr.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fwn.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qjx.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kgg.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bnb.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cya.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sya.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lda.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iws.c1oappe.top

[L03] 设置自定义请求头
来源：http://xye.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uvd.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tnz.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crn.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tkx.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://seo.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mlq.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jlu.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gsv.ivvv.top

[L04] 设置超时
来源：http://nrc.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://koi.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qxz.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kew.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://frl.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ape.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://imv.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jim.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://phc.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://cdq.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mdj.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fyp.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ool.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kmj.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zvi.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ffc.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pha.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zlp.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://yva.shanyushiyangtech.top

Py:   resp.json()
来源：http://oas.bjfxy.top

PHP:  json_decode($body, true);
来源：http://qll.jqgufenzy.top

JS:   await resp.json()
来源：http://txj.sxryk.cn

TS:   await resp.json()
来源：http://vsy.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tad.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qja.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://hjg.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aeq.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://flm.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rxf.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qff.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://mmb.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://mop.hfpthk.cn

Java: resp.statusCode()
来源：http://lzs.hesvh.cn

Go:   resp.StatusCode
来源：http://dcy.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://yhw.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://tap.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://moe.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rpw.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://zvq.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idl.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://htx.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tog.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zqn.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zia.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tug.ywan-chungtsiang.top

================================================================================
来源：http://tfb.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://cpr.chenlongwang.top

================================================================================
来源：http://hmw.aibaodan.cn

[M01] 读取命令行参数
来源：http://obv.hesvh.cn

Py:   sys.argv[1:]
来源：http://tgi.52xcode.cn

PHP:  $argv;  $argc;
来源：http://acb.yvedp.cn

JS:   process.argv.slice(2)
来源：http://bdf.hcnkem.com

TS:   process.argv.slice(2)
来源：http://rge.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://hzi.uphjek.com

Go:   os.Args[1:]
来源：http://acu.chenjidiqi.icu

Ruby: ARGV
来源：http://uvo.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://enx.yuanzhike.top

[M02] 读取环境变量
来源：http://bdj.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://wpp.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eza.chenlongwang.top

JS:   process.env.HOME
来源：http://mps.bbcook.cn

TS:   process.env.HOME
来源：http://lab.yonumen.top

Java: System.getenv("HOME")
来源：http://fsx.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pvt.nwbrower.top

Ruby: ENV["HOME"]
来源：http://pdw.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gau.shangyingyoupin.top

[M03] 执行外部命令
来源：http://ftt.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jdm.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hpb.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lym.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ajz.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qbu.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mit.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://elu.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://srs.nwbrower.top

[M04] 获取当前工作目录
来源：http://fng.fktsv.cn

Py:   os.getcwd()
来源：http://bhj.tianlin.xyz

PHP:  getcwd();
来源：http://xqm.hammf.cn

JS:   process.cwd()
来源：http://gau.ivvv.top

TS:   process.cwd()
来源：http://pgu.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://bpr.xuanzx.com

Go:   os.Getwd()
来源：http://mxq.gogol.net.cn

Ruby: Dir.pwd
来源：http://vwt.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vaa.sufxvd.cn

[M05] 设置退出码
来源：http://bro.sufxvd.cn

Py:   sys.exit(1)
来源：http://cxq.jyoumei.cn

PHP:  exit(1);
来源：http://eog.zdbjq.cn

JS:   process.exit(1)
来源：http://eor.fktsv.cn

TS:   process.exit(1)
来源：http://fja.yueranfly.top

Java: System.exit(1)
来源：http://pkn.jinqigfzy.top

Go:   os.Exit(1)
来源：http://kty.jyoumei.cn

Ruby: exit 1
来源：http://fqg.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yyr.gogol.net.cn

[M06] 向标准错误输出
来源：http://zmi.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://xaq.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uaa.ivvv.top

JS:   console.error("err")
来源：http://mkf.cdnleiting.top

TS:   console.error("err")
来源：http://xsq.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://cka.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ynq.zdqjudy.top

Ruby: warn "err"
来源：http://bqb.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://oai.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://kvh.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://jrn.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mar.xziqi.cn

JS:   require.main === module
来源：http://sfv.shanyushiyangkeji.top

TS:   require.main === module
来源：http://egc.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://vor.xylfe.cn

Go:   func main()
来源：http://nki.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cxt.redwolf501.top

C#:   static void Main(string[] args)
来源：http://rlm.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://wso.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://ngt.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://elk.tian-w.cn

JS:   process.platform;  process.version
来源：http://fwm.nwbrower.top

TS:   process.platform;  process.version
来源：http://qwp.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qlj.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rvj.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wyb.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://noi.sweek.top

================================================================================
来源：http://ehr.0kj1m.cn

N. 数据结构与算法
来源：http://eye.smart0.xyz

================================================================================
来源：http://kgo.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://hzx.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xkk.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bbw.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gpl.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pff.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://bae.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://nbv.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xkd.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cir.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://wmd.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://tqd.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jck.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lxg.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kha.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aeq.bbcook.cn

Go:   slices.Sort(arr)
来源：http://sbk.chenzaomai.com

Ruby: arr.sort
来源：http://dul.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kcw.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://yhw.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ibs.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://ncl.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jug.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://epa.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sji.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fdr.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ofa.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://raj.yfazqb.com

[N04] 斐波那契数列
来源：http://jzh.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dzo.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lbt.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rsb.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pry.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pmk.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://loa.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ibj.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yma.dashuyun.cn

[N05] 最大公约数
来源：http://epj.jianghu66.top

Py:   math.gcd(a, b)
来源：http://vip.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bqu.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://keh.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hnc.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ias.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rml.hysaishi.cn

Ruby: a.gcd(b)
来源：http://muj.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ygp.hysaishi.cn

[N06] 判断回文字符串
来源：http://gcd.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://vav.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://gjo.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://jug.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://jfj.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://snh.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://one.aizwys.cn

Ruby: s == s.reverse
来源：http://hiw.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hjy.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://pnm.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vsc.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gwg.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xwa.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://jit.gogol.net.cn

Java: // 手写 HashMap
来源：http://btd.xylfe.cn

Go:   // 手写 map[int]int
来源：http://pps.iojbl.cn

Ruby: // 手写 Hash
来源：http://erf.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://avq.c1oappe.top

[N08] 生成全排列
来源：http://has.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://sdc.shuidangran.top

PHP:  // 手写递归交换
来源：http://hzf.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://cxj.hnqzz.top

TS:   // 手写回溯递归
来源：http://nyk.haohaochexian.top

Java: // 手写回溯递归
来源：http://qbo.iojbl.cn

Go:   // 手写回溯递归
来源：http://qdf.hongshengwenyu.top

Ruby: arr.permutation.to_a
来源：http://dgc.jinqigufen.top

C#:   // 手写回溯递归
来源：http://mte.cucudq.cn

[N09] 栈与队列
来源：http://ypa.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hzb.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rib.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lhw.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oxk.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yxn.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yob.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://usu.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://emo.yongpay.top

[N10] 链表节点定义
来源：http://rke.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hmf.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zic.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bpn.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bhc.daxiang520.top

Java: class Node { int v; Node next; }
来源：http://scp.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vfh.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eiu.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://tkn.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://voi.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://juq.yueranfly.top

PHP:  // 手写递归函数
来源：http://vjd.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nst.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fum.nanxinkj.top

Java: // 手写递归
来源：http://zly.xinyue.icu

Go:   // 手写递归
来源：http://gxj.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bdl.zhixingplan.top

C#:   // 手写递归
来源：http://elo.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mqu.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mns.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wtx.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aon.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bzv.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vhx.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lmo.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ris.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mdn.fktsv.cn

================================================================================
来源：http://bnl.xingfuxueyuan.xyz

O. 并发与异步
来源：http://fqz.yangfankeji.com

================================================================================
来源：http://sst.cashguo.top

[O01] 启动一个线程
来源：http://lhy.zhixingplan.top


<!-- 参考信息 -->