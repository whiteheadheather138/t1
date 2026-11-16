代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://cmd.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tpf.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gbl.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xcz.smart0.xyz

[K06] 解析 URL 查询串
来源：http://fut.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://prj.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zyq.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ulr.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rfs.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nax.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qcj.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pbx.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lqc.aibaodan.cn

[K07] 进制转换
来源：http://nho.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vza.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gdt.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xsi.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gvm.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://msw.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ujr.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ldm.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nmo.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://ebb.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://qce.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rnp.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://tgl.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://zwg.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hfd.zhoulong.xyz

Go:   encoding/gob
来源：http://xhm.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://ghd.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://asp.yvedp.cn

================================================================================
来源：http://gyo.fanxiaobao.xyz

L. 网络请求
来源：http://lms.fktsv.cn

================================================================================
来源：http://ppt.daria6918.cn

[L01] 发送 GET 请求
来源：http://zre.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://elk.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wje.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://skn.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://gcc.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zem.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://inf.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pws.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zsz.zdqjudy.top

[L02] 发送 POST JSON
来源：http://vhz.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://qqg.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mkr.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfz.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mpp.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://trx.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qpe.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ryd.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ukt.yj202588.top

[L03] 设置自定义请求头
来源：http://ykj.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vce.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jdu.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vic.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iyi.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ylp.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://otc.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zdq.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vym.xinyue.icu

[L04] 设置超时
来源：http://xdc.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://gpy.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ayn.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zaj.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ttp.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tjs.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blr.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yib.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vjq.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://sze.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gaj.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aiv.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tbt.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mnp.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwu.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xlh.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ajy.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pdr.bbcook.cn

[L06] 解析响应为 JSON
来源：http://kao.shzxlz.cn

Py:   resp.json()
来源：http://fvs.yvedp.cn

PHP:  json_decode($body, true);
来源：http://ezu.bbcook.cn

JS:   await resp.json()
来源：http://wqm.yuxming.cn

TS:   await resp.json()
来源：http://wis.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lff.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lfk.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://ujj.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kew.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://kqj.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://okw.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gpm.yj202588.top

JS:   resp.ok;  resp.status
来源：http://uvi.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://lzm.yueranfly.top

Java: resp.statusCode()
来源：http://tby.tianlin.xyz

Go:   resp.StatusCode
来源：http://kef.9152youxi.cn

Ruby: resp.code.to_i
来源：http://vtu.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://ydu.nwbrower.top

[L08] 并发请求多个地址
来源：http://xec.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ole.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://zqd.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uaa.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pug.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hhb.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bkb.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://beu.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zoh.ivvv.top

================================================================================
来源：http://fjd.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://yyk.fengsongda.top

================================================================================
来源：http://ltg.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://yim.sxryk.cn

Py:   sys.argv[1:]
来源：http://mdq.fehbvm.com

PHP:  $argv;  $argc;
来源：http://mqn.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://kka.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://mzk.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://tbl.cucudq.cn

Go:   os.Args[1:]
来源：http://wve.daxiang520.top

Ruby: ARGV
来源：http://qrt.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://rgz.aizwys.cn

[M02] 读取环境变量
来源：http://iiv.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://yze.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yho.shangyingyoupin.top

JS:   process.env.HOME
来源：http://zln.cqqwz.cn

TS:   process.env.HOME
来源：http://rnz.jqgfzy.top

Java: System.getenv("HOME")
来源：http://kjq.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oky.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://neu.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zvc.cdnleiting.top

[M03] 执行外部命令
来源：http://kwe.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sda.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lpf.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kff.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dpf.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fdk.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://syy.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://boy.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://qxt.cdnleiting.top

[M04] 获取当前工作目录
来源：http://noy.nanxinkj.top

Py:   os.getcwd()
来源：http://ytx.ybcxt.top

PHP:  getcwd();
来源：http://zol.yuanzhike.top

JS:   process.cwd()
来源：http://ezq.chenlongwang.top

TS:   process.cwd()
来源：http://yrg.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://rdk.fktsv.cn

Go:   os.Getwd()
来源：http://nfj.wangdashe.top

Ruby: Dir.pwd
来源：http://zoy.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://puz.nwbrower.top

[M05] 设置退出码
来源：http://aof.fzhhl.top

Py:   sys.exit(1)
来源：http://juy.316326.xyz

PHP:  exit(1);
来源：http://qqd.yj20258888.top

JS:   process.exit(1)
来源：http://nql.hnxiangtu.top

TS:   process.exit(1)
来源：http://hpj.hywenlv.cn

Java: System.exit(1)
来源：http://uln.hnqzz.top

Go:   os.Exit(1)
来源：http://vyo.zhiwuduotai.top

Ruby: exit 1
来源：http://hmr.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iks.c1oappe.top

[M06] 向标准错误输出
来源：http://wpf.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://nho.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://umx.cashguo.top

JS:   console.error("err")
来源：http://jyf.xinyue.icu

TS:   console.error("err")
来源：http://lyk.ydjk.org.cn

Java: System.err.println("err")
来源：http://rjb.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dmm.316326.xyz

Ruby: warn "err"
来源：http://isa.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://buj.tarul.cn

[M07] 判断是否为主入口
来源：http://ssq.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://cfm.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://voz.jianghu66.top

JS:   require.main === module
来源：http://tsi.hongshengwenyu.top

TS:   require.main === module
来源：http://tpk.yvedp.cn

Java: public static void main(String[] args)
来源：http://htw.cdnleiting.top

Go:   func main()
来源：http://qxn.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kgi.xuanzx.com

C#:   static void Main(string[] args)
来源：http://ezl.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://msv.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://lst.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://rof.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://hmp.aizwys.cn

TS:   process.platform;  process.version
来源：http://vcf.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fcf.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ojw.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eeq.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hyn.fehbvm.com

================================================================================
来源：http://hbs.bjfxy.top

N. 数据结构与算法
来源：http://ynm.52xcode.cn

================================================================================
来源：http://pcd.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://std.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://wcr.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pgk.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cns.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://luj.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://rvv.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://hcx.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gmt.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://dlb.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://nnu.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://wec.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fvf.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://whk.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ewc.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jcm.wangdashe.top

Go:   slices.Sort(arr)
来源：http://lue.epnwcf.com

Ruby: arr.sort
来源：http://olb.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://omp.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://vhg.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ffp.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://grb.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmr.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iqc.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qkr.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ejg.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qng.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://wjn.xuanzx.com

[N04] 斐波那契数列
来源：http://tlu.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rkw.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vyk.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://elh.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nik.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jtm.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://doc.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dkg.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kmd.snrcjt.cn

[N05] 最大公约数
来源：http://kiv.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://rtt.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ikl.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vop.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ydo.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zvx.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iwe.haohaochexian.top

Ruby: a.gcd(b)
来源：http://dpk.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tge.fzhhl.top

[N06] 判断回文字符串
来源：http://gnz.fzhhl.top

Py:   s == s[::-1]
来源：http://dld.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://euj.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://evg.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://gmi.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qmt.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://ikp.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://hsk.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://doi.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://byq.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vxm.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kvl.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vck.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://fzl.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://has.bjfxy.top

Go:   // 手写 map[int]int
来源：http://nve.cucudq.cn

Ruby: // 手写 Hash
来源：http://ope.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qoe.daria6918.cn

[N08] 生成全排列
来源：http://kxl.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://nip.sysykeji.top

PHP:  // 手写递归交换
来源：http://mux.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://nwe.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://iih.zhixingplan.top

Java: // 手写回溯递归
来源：http://zvt.birdmap.top

Go:   // 手写回溯递归
来源：http://srs.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://rck.redwolf501.top

C#:   // 手写回溯递归
来源：http://mxv.nanxuanxn.top

[N09] 栈与队列
来源：http://sxf.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kep.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dol.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rcd.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tco.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://crf.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fqf.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tug.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ert.jiagoushi.top

[N10] 链表节点定义
来源：http://hqc.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ppo.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tvj.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yql.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fgk.ivvv.top

Java: class Node { int v; Node next; }
来源：http://aer.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://eip.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ajb.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mfs.xuanzx.com

[N11] 二叉树中序遍历
来源：http://xbm.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cuj.xuanzx.com

PHP:  // 手写递归函数
来源：http://onn.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qeu.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://loe.ydjk.org.cn

Java: // 手写递归
来源：http://fuh.sxryk.cn

Go:   // 手写递归
来源：http://glk.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://foh.xuanzx.com

C#:   // 手写递归
来源：http://ckp.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pou.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yua.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xga.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nle.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sjk.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sek.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pmk.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yej.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oej.316326.xyz

================================================================================
来源：http://tkx.fehbvm.com

O. 并发与异步
来源：http://hyl.xuanzx.com

================================================================================
来源：http://itn.hongshengwenyu.top

[O01] 启动一个线程
来源：http://jme.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rcj.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hvc.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zcs.yueranfly.top

TS:   // 同 JS
来源：http://wch.hammf.cn


<!-- 参考信息 -->