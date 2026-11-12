代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzk.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yha.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://tuk.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wgt.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ogq.gzhubu.top

[K07] 进制转换
来源：http://epo.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ont.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ggr.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dxf.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vxb.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rbg.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kfl.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tbj.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fiy.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://twj.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://rkq.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kkn.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://oeu.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://egc.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pnq.yvedp.cn

Go:   encoding/gob
来源：http://rzq.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://ein.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://inq.gaohongyu789.top

================================================================================
来源：http://wlb.zhixingplan.top

L. 网络请求
来源：http://nqp.chenzaomai.com

================================================================================
来源：http://tmx.zhengqikj.top

[L01] 发送 GET 请求
来源：http://lhy.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ljw.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hok.dashuyun.cn

JS:   await fetch(url)
来源：http://qgm.gogol.net.cn

TS:   await fetch(url)
来源：http://maf.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nvz.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://qpy.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jmf.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qwl.yfazqb.com

[L02] 发送 POST JSON
来源：http://wfw.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://qie.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mor.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nyd.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aep.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://auw.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://awh.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sgl.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wnm.yj202588.top

[L03] 设置自定义请求头
来源：http://jnu.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fjw.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://imt.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qdo.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hzl.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kyf.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gtl.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yvm.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bdm.yongpay.top

[L04] 设置超时
来源：http://gwn.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://kps.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qte.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://abl.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsg.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qvz.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xhh.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wng.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ghp.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://kkq.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tsc.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kfx.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ezw.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zbj.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nwg.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aea.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vcz.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zhg.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://nll.redwolf501.top

Py:   resp.json()
来源：http://efr.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://hta.nanxuanxn.top

JS:   await resp.json()
来源：http://bmt.birdmap.top

TS:   await resp.json()
来源：http://zfw.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ipq.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yfo.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://kyf.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kpj.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://dne.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://msz.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mvq.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://eim.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://jhk.yuanzhike.top

Java: resp.statusCode()
来源：http://pzt.iojbl.cn

Go:   resp.StatusCode
来源：http://gbs.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://crq.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://rvm.sxryk.cn

[L08] 并发请求多个地址
来源：http://bic.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mui.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://btw.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nfx.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsf.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xbm.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://irl.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dvl.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qlz.jinqigufen.top

================================================================================
来源：http://txf.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://sap.yj202588.top

================================================================================
来源：http://khh.zhengqikj.top

[M01] 读取命令行参数
来源：http://zni.zhengqikj.top

Py:   sys.argv[1:]
来源：http://lhv.sxryk.cn

PHP:  $argv;  $argc;
来源：http://jqz.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://joq.316326.xyz

TS:   process.argv.slice(2)
来源：http://ivg.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://fth.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://bkh.xuetiantiany.cn

Ruby: ARGV
来源：http://fot.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://jbj.cashguo.top

[M02] 读取环境变量
来源：http://fei.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://wqf.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uxz.yanxiufei.cn

JS:   process.env.HOME
来源：http://wgx.daxiang520.top

TS:   process.env.HOME
来源：http://cla.zdqjudy.top

Java: System.getenv("HOME")
来源：http://ayf.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rvf.nwbrower.top

Ruby: ENV["HOME"]
来源：http://cql.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wzg.xuetiantiany.cn

[M03] 执行外部命令
来源：http://vya.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dio.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://idv.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cxc.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yhz.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ptq.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xkv.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gwm.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://fmm.yangfankeji.com

[M04] 获取当前工作目录
来源：http://uxm.hnqzz.top

Py:   os.getcwd()
来源：http://xkz.meibo888.top

PHP:  getcwd();
来源：http://aye.yueranfly.top

JS:   process.cwd()
来源：http://hla.epnwcf.com

TS:   process.cwd()
来源：http://wpf.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://njp.wangdashe.top

Go:   os.Getwd()
来源：http://ihq.xuanzx.com

Ruby: Dir.pwd
来源：http://dbm.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://atm.bjfxy.top

[M05] 设置退出码
来源：http://cxg.yj202588.top

Py:   sys.exit(1)
来源：http://qbs.wangshuangyany.cn

PHP:  exit(1);
来源：http://wch.snrcjt.cn

JS:   process.exit(1)
来源：http://ofa.pengpengdd.cyou

TS:   process.exit(1)
来源：http://jrl.sjlbkw.cn

Java: System.exit(1)
来源：http://fbm.meibo888.top

Go:   os.Exit(1)
来源：http://jtv.aibaodan.cn

Ruby: exit 1
来源：http://iko.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dsg.snrcjt.cn

[M06] 向标准错误输出
来源：http://soo.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://vrk.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xtk.shangyingyoupin.top

JS:   console.error("err")
来源：http://eis.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://eyn.hnxiangtu.top

Java: System.err.println("err")
来源：http://ldr.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wuu.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://rtj.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://wrt.yj202588.top

[M07] 判断是否为主入口
来源：http://ghk.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://phr.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rmr.xinyue.icu

JS:   require.main === module
来源：http://rzr.mhx1999.top

TS:   require.main === module
来源：http://rcz.guowangkeji.top

Java: public static void main(String[] args)
来源：http://ggd.gzhubu.top

Go:   func main()
来源：http://vxy.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rij.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://ocu.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://oqd.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://uck.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://kvm.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://bgx.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://jfu.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rid.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zsp.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eho.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dlc.sjlbkw.cn

================================================================================
来源：http://mcw.daria6918.cn

N. 数据结构与算法
来源：http://tgm.yuxming.cn

================================================================================
来源：http://lnm.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://yeh.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://ivk.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wur.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vqf.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nfg.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://veo.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://qkw.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://twr.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://ecv.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://uiu.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://gqa.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lhy.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://hie.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rji.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jcu.havefunace.top

Go:   slices.Sort(arr)
来源：http://rfd.haohaochexian.top

Ruby: arr.sort
来源：http://kbk.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ltm.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://log.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zhi.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://kgh.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tpw.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfh.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gyw.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwu.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tvm.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://arz.jinqigfzy.top

[N04] 斐波那契数列
来源：http://oad.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://trg.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fwi.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nsv.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gyq.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nxe.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://szf.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://myq.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://duo.vehdjk.com

[N05] 最大公约数
来源：http://eiz.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://xuy.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://erm.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jur.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cte.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wst.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ses.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://qzr.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ctr.chenzaomai.com

[N06] 判断回文字符串
来源：http://nhw.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://ctd.ybcxt.top

PHP:  $s === strrev($s);
来源：http://erh.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://ffs.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://gau.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jgy.andypj.xyz

Go:   // 双指针从两端比较
来源：http://izt.sweek.top

Ruby: s == s.reverse
来源：http://kmk.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://yuo.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://fby.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bbt.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sgn.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://twy.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://rlu.tianlin.xyz

Java: // 手写 HashMap
来源：http://vrt.cucudq.cn

Go:   // 手写 map[int]int
来源：http://vla.hnqzz.top

Ruby: // 手写 Hash
来源：http://irj.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://rsa.sxryk.cn

[N08] 生成全排列
来源：http://nnt.tanke756.top

Py:   itertools.permutations(arr)
来源：http://ppd.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://dic.xziqi.cn

JS:   // 手写回溯递归
来源：http://spg.mhx1999.top

TS:   // 手写回溯递归
来源：http://dgn.svipenyu.cn

Java: // 手写回溯递归
来源：http://rjp.sysykeji.top

Go:   // 手写回溯递归
来源：http://spt.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://hbz.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://zqq.hongshengwenyu.top

[N09] 栈与队列
来源：http://lrs.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://osi.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qbn.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dlu.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oqu.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://low.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gay.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kla.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://viy.havefunace.top

[N10] 链表节点定义
来源：http://aem.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lhu.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cnm.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tzc.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vcu.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://cvu.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://vzs.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kll.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sqi.hnqzz.top

[N11] 二叉树中序遍历
来源：http://enx.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oui.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://mos.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://npe.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zyx.bbcook.cn

Java: // 手写递归
来源：http://odx.zdqjudy.top

Go:   // 手写递归
来源：http://lnm.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rsb.yfazqb.com

C#:   // 手写递归
来源：http://gqi.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pmz.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wfq.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pit.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpn.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xdu.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nss.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qmj.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qgs.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jqb.hesvh.cn

================================================================================
来源：http://npt.vehdjk.com

O. 并发与异步
来源：http://tez.fzhhl.top

================================================================================
来源：http://scu.fktsv.cn

[O01] 启动一个线程
来源：http://syw.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ttf.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jvj.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ibh.jlsjyb.cn

TS:   // 同 JS
来源：http://axk.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://whk.hnxiangtu.top

Go:   go f()
来源：http://vkl.bbcook.cn

Ruby: Thread.new { f }
来源：http://gtm.gzhubu.top

C#:   Task.Run(() => F());
来源：http://dpb.yueranfly.top

[O02] 使用线程池
来源：http://zmk.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ptn.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uvg.cucudq.cn

JS:   // worker_threads 线程池
来源：http://muk.smart0.xyz


<!-- 参考信息 -->