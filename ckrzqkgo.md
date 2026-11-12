代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jtk.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vfq.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://isd.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yxw.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://usp.kuanghao11.cn

[K07] 进制转换
来源：http://zcv.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qej.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xwc.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gpy.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pyv.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dke.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ffn.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evs.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zer.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://lbt.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://scx.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wqo.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://jsf.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://eob.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vwn.fktsv.cn

Go:   encoding/gob
来源：http://lgh.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://cef.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oea.uphjek.com

================================================================================
来源：http://xxb.ydzc1.top

L. 网络请求
来源：http://nve.birdmap.top

================================================================================
来源：http://cdg.sufxvd.cn

[L01] 发送 GET 请求
来源：http://csr.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://smy.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rxf.jianghu66.top

JS:   await fetch(url)
来源：http://fgt.yonumen.top

TS:   await fetch(url)
来源：http://ltm.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bqm.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://ndr.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wkp.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pyp.fehbvm.com

[L02] 发送 POST JSON
来源：http://rdy.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://lxa.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bbi.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbt.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uoe.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ciy.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yez.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvu.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://glo.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://fah.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nxo.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hkq.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qcm.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rju.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hga.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eqh.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zvh.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mrd.ywan-chungtsiang.top

[L04] 设置超时
来源：http://hig.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://fdi.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qqy.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://phl.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ggl.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xft.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cdy.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bei.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://whk.yj20258888.top

[L05] 上传文件（multipart）
来源：http://qtp.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tdp.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sfl.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jim.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://muo.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cuu.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oat.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zgb.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ljr.yonumen.top

[L06] 解析响应为 JSON
来源：http://vgh.jinqigufen.top

Py:   resp.json()
来源：http://gcj.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://opr.yuanzhike.top

JS:   await resp.json()
来源：http://kuv.sjlbkw.cn

TS:   await resp.json()
来源：http://ack.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://asu.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qoc.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://xxm.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qlz.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://mzv.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://niw.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hrr.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://hfb.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://tmz.jinqigfzy.top

Java: resp.statusCode()
来源：http://dnt.tian-w.cn

Go:   resp.StatusCode
来源：http://zei.yongpay.top

Ruby: resp.code.to_i
来源：http://fai.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://ema.yangfankeji.com

[L08] 并发请求多个地址
来源：http://eii.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kug.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://oxg.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zjr.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xxv.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ezz.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cml.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xhx.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lhx.gotoacloud.top

================================================================================
来源：http://edv.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://png.tian-w.cn

================================================================================
来源：http://kbj.pycfn.com

[M01] 读取命令行参数
来源：http://kic.andypj.xyz

Py:   sys.argv[1:]
来源：http://gxd.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://cgn.bbcook.cn

JS:   process.argv.slice(2)
来源：http://ptj.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://cmh.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://oqt.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://djp.shangyingyoupin.top

Ruby: ARGV
来源：http://wru.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://qef.cdnleiting.top

[M02] 读取环境变量
来源：http://zny.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://eeg.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yzv.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://kyt.hywenlv.cn

TS:   process.env.HOME
来源：http://mwe.hesvh.cn

Java: System.getenv("HOME")
来源：http://mff.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tfi.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://htn.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vcx.hcnkem.com

[M03] 执行外部命令
来源：http://wyi.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tyd.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fml.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mau.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gar.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fxg.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ydf.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://sjl.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://tkj.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://nji.fengsongda.top

Py:   os.getcwd()
来源：http://qrt.cdnleiting.top

PHP:  getcwd();
来源：http://ssf.ehwqpu.com

JS:   process.cwd()
来源：http://jqb.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://qqu.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://opk.hcnkem.com

Go:   os.Getwd()
来源：http://rmi.jinqigfzy.top

Ruby: Dir.pwd
来源：http://lsn.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dls.0kj1m.cn

[M05] 设置退出码
来源：http://duc.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://xay.yuanzhike.top

PHP:  exit(1);
来源：http://hbt.havefunace.top

JS:   process.exit(1)
来源：http://ssa.yueranfly.top

TS:   process.exit(1)
来源：http://cab.fanxiaobao.xyz

Java: System.exit(1)
来源：http://hfy.cucudq.cn

Go:   os.Exit(1)
来源：http://npd.feifeiyinyue.top

Ruby: exit 1
来源：http://xbn.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hzw.zycfv.cn

[M06] 向标准错误输出
来源：http://ktr.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://wnz.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bqo.smart0.xyz

JS:   console.error("err")
来源：http://ria.daria6918.cn

TS:   console.error("err")
来源：http://ilw.gzhubu.top

Java: System.err.println("err")
来源：http://cou.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://olj.andypj.xyz

Ruby: warn "err"
来源：http://tpj.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://krw.bjfxy.top

[M07] 判断是否为主入口
来源：http://mwg.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://nhs.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bfa.snrcjt.cn

JS:   require.main === module
来源：http://pvb.jqgfzy.top

TS:   require.main === module
来源：http://opq.cdnleiting.top

Java: public static void main(String[] args)
来源：http://xpg.shanyushiyangkeji.top

Go:   func main()
来源：http://cez.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://moz.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://ayh.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://ddz.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://gro.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://agb.gotoacloud.top

JS:   process.platform;  process.version
来源：http://hlq.cqqwz.cn

TS:   process.platform;  process.version
来源：http://xel.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rgz.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nqx.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sic.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmq.ctjpmb.com

================================================================================
来源：http://sqm.dashuyun.cn

N. 数据结构与算法
来源：http://bfi.yongpay.top

================================================================================
来源：http://gfq.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://xjm.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://jny.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gji.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gdr.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sjn.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qws.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://nsn.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pte.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://qty.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://rmj.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://qzf.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mct.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://glb.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ekl.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://twl.ybcxt.top

Go:   slices.Sort(arr)
来源：http://taw.yangfankeji.com

Ruby: arr.sort
来源：http://brj.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ibb.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://dko.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rui.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://ynw.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvm.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jkr.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wim.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bgn.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tih.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fkl.ydzc1.top

[N04] 斐波那契数列
来源：http://xhg.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vxt.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ulp.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://psa.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pyt.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jic.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ztq.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zcx.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qom.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://hyr.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://amm.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvx.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekf.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yrk.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ilk.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qra.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://puv.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dbf.cashguo.top

[N06] 判断回文字符串
来源：http://tdt.yj20258.top

Py:   s == s[::-1]
来源：http://ofd.guannengcc.top

PHP:  $s === strrev($s);
来源：http://ueh.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://xch.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://cal.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://svy.hcnkem.com

Go:   // 双指针从两端比较
来源：http://guo.chenzaomai.com

Ruby: s == s.reverse
来源：http://rke.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ppm.yj20258.top

[N07] 两数之和（返回下标）
来源：http://zrv.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hyn.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jdl.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vwm.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://evz.nanxuanxn.top

Java: // 手写 HashMap
来源：http://yrv.c1oappe.top

Go:   // 手写 map[int]int
来源：http://awl.chenzaomai.com

Ruby: // 手写 Hash
来源：http://lvm.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nmu.tianlin.xyz

[N08] 生成全排列
来源：http://fnd.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://isf.0kj1m.cn

PHP:  // 手写递归交换
来源：http://ptv.xinyue.icu

JS:   // 手写回溯递归
来源：http://mma.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://huh.hammf.cn

Java: // 手写回溯递归
来源：http://uya.andypj.xyz

Go:   // 手写回溯递归
来源：http://yxk.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://lmt.zdbjq.cn

C#:   // 手写回溯递归
来源：http://mpv.nwbrower.top

[N09] 栈与队列
来源：http://abb.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yqd.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hdm.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ojj.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://chx.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ory.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iyu.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qaw.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ebp.zhongyouzk.top

[N10] 链表节点定义
来源：http://tzn.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpv.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://awt.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ccb.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dbt.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://zft.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://brq.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://shx.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jzf.mhx1999.top

[N11] 二叉树中序遍历
来源：http://rxt.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dtb.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://gjo.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndy.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qjo.jinqigfzy.top

Java: // 手写递归
来源：http://lss.pycfn.com

Go:   // 手写递归
来源：http://apn.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uuk.316326.xyz

C#:   // 手写递归
来源：http://imr.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://myt.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dvf.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exw.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xke.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jlg.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tyx.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqc.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ghj.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sfw.jqgufenzy.top

================================================================================
来源：http://zpg.52xcode.cn

O. 并发与异步
来源：http://acw.bjfxy.top

================================================================================
来源：http://rsw.guannengcc.top

[O01] 启动一个线程
来源：http://tlt.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lkd.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yqe.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aux.dashuyun.cn

TS:   // 同 JS
来源：http://dge.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://oqf.kuanghao11.cn

Go:   go f()
来源：http://ikj.ctjpmb.com

Ruby: Thread.new { f }
来源：http://cph.hammf.cn

C#:   Task.Run(() => F());
来源：http://cds.hysaishi.cn

[O02] 使用线程池
来源：http://kwe.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zyd.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lpp.sweek.top

JS:   // worker_threads 线程池
来源：http://ijz.jinqigufen.top


<!-- 参考信息 -->