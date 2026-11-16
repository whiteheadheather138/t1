代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zcn.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://san.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dki.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eia.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fkm.kuanghao11.cn

[K07] 进制转换
来源：http://wnh.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wkn.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zfs.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fig.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kzi.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://opt.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ued.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://muc.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jif.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://pps.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://zrl.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bpu.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://brw.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://aom.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gmp.andypj.xyz

Go:   encoding/gob
来源：http://lbk.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://zxk.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhf.yueranfly.top

================================================================================
来源：http://wuu.zhaomingkeji.xyz

L. 网络请求
来源：http://sgn.fktsv.cn

================================================================================
来源：http://wjf.andypj.xyz

[L01] 发送 GET 请求
来源：http://xiy.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ufz.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wem.jqgfzy.top

JS:   await fetch(url)
来源：http://iqh.gogol.net.cn

TS:   await fetch(url)
来源：http://tyd.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ajn.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://vim.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hka.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bar.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://vea.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://ixu.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tet.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://asu.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://shv.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://etc.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rub.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yaa.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://acl.aizwys.cn

[L03] 设置自定义请求头
来源：http://ejf.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aoy.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mqt.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xim.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rxy.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dja.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fvs.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fog.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ozl.shuidangran.top

[L04] 设置超时
来源：http://mhn.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://maf.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bhu.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kow.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pna.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bnh.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nbl.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bwy.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tfy.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://uaw.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bks.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wtr.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wdq.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vsi.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eiz.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qcn.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xgv.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://toc.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://zrx.cheryme.top

Py:   resp.json()
来源：http://zsu.yj202588.top

PHP:  json_decode($body, true);
来源：http://crt.sweek.top

JS:   await resp.json()
来源：http://xzn.gogol.net.cn

TS:   await resp.json()
来源：http://pck.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cln.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jdr.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://ooi.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ays.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://iis.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pvu.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yjm.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://bmq.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://jai.aizwys.cn

Java: resp.statusCode()
来源：http://rqp.hywenlv.cn

Go:   resp.StatusCode
来源：http://fid.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://rfn.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://siq.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://bsd.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mft.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://azm.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xst.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hal.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kzf.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kni.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ogp.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://epp.vehdjk.com

================================================================================
来源：http://rte.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://gui.feifeiyinyue.top

================================================================================
来源：http://gaa.guowangkeji.top

[M01] 读取命令行参数
来源：http://jet.tarul.cn

Py:   sys.argv[1:]
来源：http://zpt.havefunace.top

PHP:  $argv;  $argc;
来源：http://ccj.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://xzx.smart0.xyz

TS:   process.argv.slice(2)
来源：http://lri.ivvv.top

Java: args 数组（main 方法参数）
来源：http://xih.yj20258.top

Go:   os.Args[1:]
来源：http://ofw.0kj1m.cn

Ruby: ARGV
来源：http://jvw.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://cbp.zhixingplan.top

[M02] 读取环境变量
来源：http://kxi.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://mzm.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://isc.yonumen.top

JS:   process.env.HOME
来源：http://vbn.quarkkingdee.top

TS:   process.env.HOME
来源：http://vqx.jyoumei.cn

Java: System.getenv("HOME")
来源：http://lbj.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://itu.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://sme.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mcr.jqgfzy.top

[M03] 执行外部命令
来源：http://ezt.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://snz.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iyq.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yje.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gbp.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ror.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qlr.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bfe.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://izx.nwbrower.top

[M04] 获取当前工作目录
来源：http://dtd.yueranfly.top

Py:   os.getcwd()
来源：http://esd.fanxiaobao.xyz

PHP:  getcwd();
来源：http://hcr.aibaodan.cn

JS:   process.cwd()
来源：http://uki.dianchejie.cn

TS:   process.cwd()
来源：http://kfu.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://mxj.snrcjt.cn

Go:   os.Getwd()
来源：http://jln.cucudq.cn

Ruby: Dir.pwd
来源：http://urk.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://uel.fzhhl.top

[M05] 设置退出码
来源：http://bgn.yj20258.top

Py:   sys.exit(1)
来源：http://cxj.cqqwz.cn

PHP:  exit(1);
来源：http://fgx.redwolf501.top

JS:   process.exit(1)
来源：http://kiy.yj20258888.top

TS:   process.exit(1)
来源：http://zyg.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://pnc.bjfxy.top

Go:   os.Exit(1)
来源：http://bzz.jinghuilouyu.cn

Ruby: exit 1
来源：http://qkz.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kyn.yueranfly.top

[M06] 向标准错误输出
来源：http://gnd.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://zpo.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ypb.ppjwa.cn

JS:   console.error("err")
来源：http://bxz.xuanzx.com

TS:   console.error("err")
来源：http://xiw.0kj1m.cn

Java: System.err.println("err")
来源：http://cpj.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vbd.c1oappe.top

Ruby: warn "err"
来源：http://xbp.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ule.hnqzz.top

[M07] 判断是否为主入口
来源：http://nvo.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://yct.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://scx.zhaomingkeji.xyz

JS:   require.main === module
来源：http://gpj.pycfn.com

TS:   require.main === module
来源：http://isi.hnqzz.top

Java: public static void main(String[] args)
来源：http://xlp.ywan-chungtsiang.top

Go:   func main()
来源：http://bwy.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hxg.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://aqj.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://ygg.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://pdj.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://dhc.tanke756.top

JS:   process.platform;  process.version
来源：http://uyj.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://imb.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jko.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fhc.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ckj.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iyq.quarkkingdee.top

================================================================================
来源：http://fhr.cdnleiting.top

N. 数据结构与算法
来源：http://wrx.sjlbkw.cn

================================================================================
来源：http://gon.yj202588.top

[N01] 二分查找（有序数组）
来源：http://pou.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://nrt.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qwm.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zwj.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xph.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://msl.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://icy.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mhg.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://zty.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://nob.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://ies.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://duz.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://roe.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ojx.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tgf.zycfv.cn

Go:   slices.Sort(arr)
来源：http://stx.aizwys.cn

Ruby: arr.sort
来源：http://zcv.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyv.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://udt.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://szt.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://gzz.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whl.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xle.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://npp.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uvv.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xyj.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://ygt.xziqi.cn

[N04] 斐波那契数列
来源：http://ivq.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uvw.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sew.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fjs.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://trc.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hgd.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bwj.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ikc.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://onj.chenlongwang.top

[N05] 最大公约数
来源：http://mnj.sxryk.cn

Py:   math.gcd(a, b)
来源：http://lzk.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bnx.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bjw.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hrq.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jto.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zbd.redwolf501.top

Ruby: a.gcd(b)
来源：http://kwe.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jcy.hnxiangtu.top

[N06] 判断回文字符串
来源：http://kxs.tanke756.top

Py:   s == s[::-1]
来源：http://xml.redwolf501.top

PHP:  $s === strrev($s);
来源：http://xnw.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://caf.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://ngv.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ksq.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://vcy.guannengcc.top

Ruby: s == s.reverse
来源：http://ssn.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://djy.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://bgx.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bfk.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axj.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://wof.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://wel.yj20258.top

Java: // 手写 HashMap
来源：http://phl.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://lja.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://tgh.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fmp.pycfn.com

[N08] 生成全排列
来源：http://zqj.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://hfn.bjfxy.top

PHP:  // 手写递归交换
来源：http://pkb.hysaishi.cn

JS:   // 手写回溯递归
来源：http://otx.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://idy.zdqjudy.top

Java: // 手写回溯递归
来源：http://tag.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://qmy.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://dfj.gogol.net.cn

C#:   // 手写回溯递归
来源：http://fue.ydjk.org.cn

[N09] 栈与队列
来源：http://ksb.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ugn.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wso.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubz.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kuj.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aig.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yda.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nev.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nom.zdbjq.cn

[N10] 链表节点定义
来源：http://dsp.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dua.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://xye.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://urs.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qci.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ucs.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://amq.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://muj.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://udk.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://acj.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ypz.cheryme.top

PHP:  // 手写递归函数
来源：http://fes.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dgu.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ehg.jlsjyb.cn

Java: // 手写递归
来源：http://zwv.hywenlv.cn

Go:   // 手写递归
来源：http://fmu.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://unh.mhx1999.top

C#:   // 手写递归
来源：http://hzt.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yxt.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oyz.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bys.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gwr.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epu.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lpf.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wpo.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xwn.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jla.yueranfly.top

================================================================================
来源：http://zvc.redwolf501.top

O. 并发与异步
来源：http://wzt.316326.xyz

================================================================================
来源：http://wsf.vqdsnc.cn

[O01] 启动一个线程
来源：http://muk.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jkn.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ndf.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ccp.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://ewa.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://gaz.ydjk.org.cn

Go:   go f()
来源：http://ltj.ivvv.top

Ruby: Thread.new { f }
来源：http://pxq.daxiang520.top

C#:   Task.Run(() => F());
来源：http://mss.aizwys.cn

[O02] 使用线程池
来源：http://fwc.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rlf.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uag.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://jnc.tian-w.cn


<!-- 参考信息 -->