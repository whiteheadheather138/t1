代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xok.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://niz.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dwf.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ipv.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vzi.uphjek.com

[K07] 进制转换
来源：http://bko.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hjo.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zji.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ipb.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ejm.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ejg.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://byi.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fmz.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uha.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://aqr.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://fiw.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fnw.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://sta.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://acv.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rgf.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://ald.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://iqk.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://guo.ehwqpu.com

================================================================================
来源：http://ihs.svipenyu.cn

L. 网络请求
来源：http://hhw.hnqzz.top

================================================================================
来源：http://apx.jiagoushi.top

[L01] 发送 GET 请求
来源：http://lzm.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zbf.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rsb.gzhubu.top

JS:   await fetch(url)
来源：http://xjq.yj202588.top

TS:   await fetch(url)
来源：http://bep.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dfe.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://lpi.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kth.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://krn.hysaishi.cn

[L02] 发送 POST JSON
来源：http://ibb.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://kxw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://anh.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xbd.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pzj.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://alf.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jco.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tqf.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xrp.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://obt.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xzj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://myz.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://csx.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jzh.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wvg.yueranfly.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fya.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rsx.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xij.tianlin.xyz

[L04] 设置超时
来源：http://eok.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://lpw.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyl.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jlw.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ujs.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rjm.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yas.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dee.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bsj.ctjpmb.com

[L05] 上传文件（multipart）
来源：http://bod.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uxs.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://toe.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nxa.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ccb.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://csw.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fmz.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://huo.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wus.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://ums.sxryk.cn

Py:   resp.json()
来源：http://sus.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://ukj.jlsjyb.cn

JS:   await resp.json()
来源：http://dqu.ivvv.top

TS:   await resp.json()
来源：http://lzt.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mgx.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rxx.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://syp.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bmm.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://gon.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eft.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xib.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://ywu.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://zcc.xylfe.cn

Java: resp.statusCode()
来源：http://udd.tianlin.xyz

Go:   resp.StatusCode
来源：http://fhc.nwbrower.top

Ruby: resp.code.to_i
来源：http://aag.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://ysj.snrcjt.cn

[L08] 并发请求多个地址
来源：http://ucy.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ozp.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://mdq.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgo.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gqh.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ejx.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uuo.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zon.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ukz.ivvv.top

================================================================================
来源：http://zot.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://gcd.xziqi.cn

================================================================================
来源：http://zga.jqgfzy.top

[M01] 读取命令行参数
来源：http://acd.jiagoushi.top

Py:   sys.argv[1:]
来源：http://gae.hammf.cn

PHP:  $argv;  $argc;
来源：http://keu.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://nnx.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://qti.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://xze.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://huv.tian-w.cn

Ruby: ARGV
来源：http://rpc.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://hjf.zdbjq.cn

[M02] 读取环境变量
来源：http://zgn.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://dgg.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://veu.hfpthk.cn

JS:   process.env.HOME
来源：http://yrk.hysaishi.cn

TS:   process.env.HOME
来源：http://qxc.cheryme.top

Java: System.getenv("HOME")
来源：http://apu.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dzm.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://vci.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bzr.birdmap.top

[M03] 执行外部命令
来源：http://cwt.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mqh.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bnb.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://dnk.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wyq.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jsq.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nlq.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yto.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://xlh.bjfxy.top

[M04] 获取当前工作目录
来源：http://qrs.yonumen.top

Py:   os.getcwd()
来源：http://ygz.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://kiq.xinyue.icu

JS:   process.cwd()
来源：http://yjk.bbcook.cn

TS:   process.cwd()
来源：http://wnt.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://djy.hnxiangtu.top

Go:   os.Getwd()
来源：http://ajl.pycfn.com

Ruby: Dir.pwd
来源：http://kct.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://yrk.cdnleiting.top

[M05] 设置退出码
来源：http://sus.chenzaomai.com

Py:   sys.exit(1)
来源：http://tcu.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://nee.sufxvd.cn

JS:   process.exit(1)
来源：http://sjx.c1oappe.top

TS:   process.exit(1)
来源：http://tct.zhiwuduotai.top

Java: System.exit(1)
来源：http://ntu.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://zdf.ctjpmb.com

Ruby: exit 1
来源：http://amq.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jlq.hcnkem.com

[M06] 向标准错误输出
来源：http://vyz.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://pxm.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cnm.redwolf501.top

JS:   console.error("err")
来源：http://uug.cdnleiting.top

TS:   console.error("err")
来源：http://qye.wangshuangyany.cn

Java: System.err.println("err")
来源：http://umi.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://owc.guannengcc.top

Ruby: warn "err"
来源：http://gcs.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://rrs.iojbl.cn

[M07] 判断是否为主入口
来源：http://niv.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://opy.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://svu.fzhhl.top

JS:   require.main === module
来源：http://owi.ppjwa.cn

TS:   require.main === module
来源：http://acl.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://btx.cqqwz.cn

Go:   func main()
来源：http://jyu.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wvt.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://sxu.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://qoe.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://jda.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://kpl.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://jdw.chenlongwang.top

TS:   process.platform;  process.version
来源：http://tla.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tjx.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://kup.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dgy.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://llz.zdbjq.cn

================================================================================
来源：http://rup.meibo888.top

N. 数据结构与算法
来源：http://eli.0kj1m.cn

================================================================================
来源：http://yrr.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://wcj.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://lza.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tuu.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwb.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://krs.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://yax.yj20258888.top

Go:   sort.SearchInts(arr, x)
来源：http://zdw.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://man.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ooq.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://jqo.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://ypo.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://btn.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://vxf.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aly.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eek.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://wln.cucudq.cn

Ruby: arr.sort
来源：http://zcv.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lrk.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://rid.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://irs.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://wie.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxl.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hlf.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lnj.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mmn.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zse.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://sqx.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://coo.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpf.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tet.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oda.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ors.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wfk.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gpo.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zwv.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vsi.yonumen.top

[N05] 最大公约数
来源：http://ear.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://jng.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xcg.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovh.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxv.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tyo.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yre.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://mam.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cry.guannengcc.top

[N06] 判断回文字符串
来源：http://fik.yj202588.top

Py:   s == s[::-1]
来源：http://hfh.52xcode.cn

PHP:  $s === strrev($s);
来源：http://nyc.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://tfy.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://gpp.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kik.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://qkd.yuxming.cn

Ruby: s == s.reverse
来源：http://swf.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://faf.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://vat.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sxb.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aju.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://khx.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://hzp.birdmap.top

Java: // 手写 HashMap
来源：http://chb.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://dls.zhixingplan.top

Ruby: // 手写 Hash
来源：http://vkm.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://zjb.ybcxt.top

[N08] 生成全排列
来源：http://xnt.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://bqs.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://sao.sxryk.cn

JS:   // 手写回溯递归
来源：http://sho.shzxlz.cn

TS:   // 手写回溯递归
来源：http://gsk.aibaodan.cn

Java: // 手写回溯递归
来源：http://uff.smart0.xyz

Go:   // 手写回溯递归
来源：http://ksi.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://dbt.sysykeji.top

C#:   // 手写回溯递归
来源：http://pfh.0kj1m.cn

[N09] 栈与队列
来源：http://gpj.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hma.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gne.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xex.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sxn.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzb.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vdc.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://adv.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zyt.yvedp.cn

[N10] 链表节点定义
来源：http://irm.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://znu.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tdh.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://smp.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nyu.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://swo.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://rrj.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ryw.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ihf.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://kxf.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uac.tian-w.cn

PHP:  // 手写递归函数
来源：http://hvn.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cor.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zse.yonumen.top

Java: // 手写递归
来源：http://plu.jiagoushi.top

Go:   // 手写递归
来源：http://jcu.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oyx.zhijiandao.cn

C#:   // 手写递归
来源：http://vzv.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jag.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tjj.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ynj.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xwu.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzq.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lak.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mbt.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qzx.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://izw.zhaomingkeji.xyz

================================================================================
来源：http://zcb.yvedp.cn

O. 并发与异步
来源：http://agm.jlsjyb.cn

================================================================================
来源：http://vly.zycfv.cn

[O01] 启动一个线程
来源：http://vrs.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vbt.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bbt.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rvu.daxiang520.top

TS:   // 同 JS
来源：http://ick.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://vqe.ehwqpu.com

Go:   go f()
来源：http://wsc.jianghu66.top

Ruby: Thread.new { f }
来源：http://xdb.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://dir.snrcjt.cn

[O02] 使用线程池
来源：http://epj.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lem.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blh.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://cey.bjfxy.top


<!-- 参考信息 -->