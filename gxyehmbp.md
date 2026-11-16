代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oxt.smart0.xyz

[K07] 进制转换
来源：http://tmj.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gnj.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qkn.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cpc.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zou.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hel.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ibr.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xqh.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://phe.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://yyw.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://idd.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sst.xylfe.cn

JS:   v8.serialize(obj)        // Node
来源：http://ble.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://bcy.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jjb.ehwqpu.com

Go:   encoding/gob
来源：http://oww.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://ord.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqx.xuanzx.com

================================================================================
来源：http://ymb.guannengcc.top

L. 网络请求
来源：http://utg.aizwys.cn

================================================================================
来源：http://vjj.sweek.top

[L01] 发送 GET 请求
来源：http://lqp.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eql.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mbf.sufxvd.cn

JS:   await fetch(url)
来源：http://zpu.gotoacloud.top

TS:   await fetch(url)
来源：http://nyd.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kei.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://ebp.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gsz.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://alr.zhixingplan.top

[L02] 发送 POST JSON
来源：http://dzm.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://xvs.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://quk.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wft.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vyu.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kxu.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tjy.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cev.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://swx.yj20258.top

[L03] 设置自定义请求头
来源：http://vgn.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fiy.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ixk.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kka.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ask.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sze.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kfy.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iiz.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://glz.jinyuanbaomall.cn

[L04] 设置超时
来源：http://iiw.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://ecd.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hvw.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ujp.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bln.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hul.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yte.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xms.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://njz.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://lgm.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zdh.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://umc.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://idh.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mqo.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://umg.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vjx.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://phz.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yrq.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://ngv.zhiwuduotai.top

Py:   resp.json()
来源：http://laj.c1oappe.top

PHP:  json_decode($body, true);
来源：http://fgi.jqgfzy.top

JS:   await resp.json()
来源：http://swj.zdbjq.cn

TS:   await resp.json()
来源：http://cpa.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nmz.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rag.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://ozt.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bqc.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://veo.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vnh.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hew.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://rfs.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://caq.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://kaf.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://vso.cucudq.cn

Ruby: resp.code.to_i
来源：http://gch.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://hoz.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://mvr.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://glt.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://imf.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oic.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olp.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xnp.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tiu.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eqn.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ewv.guowangkeji.top

================================================================================
来源：http://bsp.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://jut.aibaodan.cn

================================================================================
来源：http://oka.ctjpmb.com

[M01] 读取命令行参数
来源：http://nxe.gzhubu.top

Py:   sys.argv[1:]
来源：http://fhk.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://znd.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://vtg.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://tfv.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://mxb.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://npl.sysykeji.top

Ruby: ARGV
来源：http://rha.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://bpl.yanxiufei.cn

[M02] 读取环境变量
来源：http://sof.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://pjb.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jik.hesvh.cn

JS:   process.env.HOME
来源：http://ghn.hesvh.cn

TS:   process.env.HOME
来源：http://xub.nanxinkj.top

Java: System.getenv("HOME")
来源：http://lgy.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xvj.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://zwy.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ejv.316326.xyz

[M03] 执行外部命令
来源：http://fyv.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vnq.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cht.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://yhb.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://glk.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fwz.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ekl.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://kdm.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://rjm.316326.xyz

[M04] 获取当前工作目录
来源：http://xbv.jqgufenzy.top

Py:   os.getcwd()
来源：http://byf.jianghu66.top

PHP:  getcwd();
来源：http://mym.shanyushiyangtech.top

JS:   process.cwd()
来源：http://epx.sysykeji.top

TS:   process.cwd()
来源：http://vry.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://jfd.pycfn.com

Go:   os.Getwd()
来源：http://rjr.cashguo.top

Ruby: Dir.pwd
来源：http://eph.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://ofr.yj20258.top

[M05] 设置退出码
来源：http://myk.sxryk.cn

Py:   sys.exit(1)
来源：http://lmm.gogol.net.cn

PHP:  exit(1);
来源：http://jdu.yj202588.top

JS:   process.exit(1)
来源：http://myk.ydzc1.top

TS:   process.exit(1)
来源：http://nxe.gotoacloud.top

Java: System.exit(1)
来源：http://ajk.yj20258.top

Go:   os.Exit(1)
来源：http://tuv.snrcjt.cn

Ruby: exit 1
来源：http://vvn.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xjl.daria6918.cn

[M06] 向标准错误输出
来源：http://dup.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://jor.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://aeh.kuanghao11.cn

JS:   console.error("err")
来源：http://soj.jqgufenzy.top

TS:   console.error("err")
来源：http://evo.kuanghao11.cn

Java: System.err.println("err")
来源：http://kjx.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eon.fengsongda.top

Ruby: warn "err"
来源：http://fcs.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://zuf.shuidangran.top

[M07] 判断是否为主入口
来源：http://gih.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://geo.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://exr.haohaochexian.top

JS:   require.main === module
来源：http://ldo.zhixingplan.top

TS:   require.main === module
来源：http://ipa.316326.xyz

Java: public static void main(String[] args)
来源：http://sjj.xylfe.cn

Go:   func main()
来源：http://dqj.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ccp.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://izm.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://jpc.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://thw.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://suh.fktsv.cn

JS:   process.platform;  process.version
来源：http://bwu.chenlongwang.top

TS:   process.platform;  process.version
来源：http://mte.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://roi.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zza.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qwh.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sme.cucudq.cn

================================================================================
来源：http://klh.shuidangran.top

N. 数据结构与算法
来源：http://ncg.gzhubu.top

================================================================================
来源：http://doj.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://irp.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aic.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vgj.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://syz.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lva.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://skp.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://qmh.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ijc.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://vzt.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://asx.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://eck.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://srn.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cdw.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gas.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gww.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://vrf.guannengcc.top

Ruby: arr.sort
来源：http://keb.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukc.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://nil.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lrz.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://fdo.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmd.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpv.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jvl.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uad.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ubu.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://qzl.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://vhs.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://arw.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kin.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://llk.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xuc.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dyv.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vbp.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://shj.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ztr.hysaishi.cn

[N05] 最大公约数
来源：http://zkx.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://iey.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqg.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxw.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oft.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wfo.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xpu.tianlin.xyz

Ruby: a.gcd(b)
来源：http://gvg.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dmj.zhoulong.xyz

[N06] 判断回文字符串
来源：http://qvy.yanxiufei.cn

Py:   s == s[::-1]
来源：http://oex.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://jkh.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://rzz.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://klp.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jqg.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://jmv.meibo888.top

Ruby: s == s.reverse
来源：http://pyd.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://dff.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://uxm.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ylf.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eyl.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wps.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://pid.redwolf501.top

Java: // 手写 HashMap
来源：http://vlg.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://ggr.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://umz.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://abt.gogol.net.cn

[N08] 生成全排列
来源：http://mdz.sweek.top

Py:   itertools.permutations(arr)
来源：http://fsj.0kj1m.cn

PHP:  // 手写递归交换
来源：http://tah.sysykeji.top

JS:   // 手写回溯递归
来源：http://ten.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://qsu.hysaishi.cn

Java: // 手写回溯递归
来源：http://mef.0kj1m.cn

Go:   // 手写回溯递归
来源：http://dbi.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://jsi.daxiang520.top

C#:   // 手写回溯递归
来源：http://jif.daria6918.cn

[N09] 栈与队列
来源：http://mrc.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ljo.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vyl.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xyw.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://upb.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://edu.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://flk.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fbt.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://njk.daria6918.cn

[N10] 链表节点定义
来源：http://kiy.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://neo.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://vmv.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lxm.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tmb.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://rfb.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tet.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sin.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bup.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://tob.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xdr.zdqjudy.top

PHP:  // 手写递归函数
来源：http://fro.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kng.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cph.sufxvd.cn

Java: // 手写递归
来源：http://lvy.wangshuangyany.cn

Go:   // 手写递归
来源：http://faw.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqp.zdqjudy.top

C#:   // 手写递归
来源：http://nbd.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uvc.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gio.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fll.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oar.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://foc.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fff.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yun.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zcw.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://idp.fktsv.cn

================================================================================
来源：http://sxw.cheryme.top

O. 并发与异步
来源：http://bhr.shuidangran.top

================================================================================
来源：http://jeg.zycfv.cn

[O01] 启动一个线程
来源：http://rbx.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lvo.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bbf.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bei.yanxiufei.cn

TS:   // 同 JS
来源：http://pdz.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://nny.jiagoushi.top

Go:   go f()
来源：http://huc.chenzaomai.com

Ruby: Thread.new { f }
来源：http://kyi.bbcook.cn

C#:   Task.Run(() => F());
来源：http://hek.tian-w.cn

[O02] 使用线程池
来源：http://qfb.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xlx.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uev.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://nvz.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://emk.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://qxb.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cju.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xxi.zhijiandao.cn


<!-- 参考信息 -->