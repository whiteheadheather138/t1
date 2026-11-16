代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ima.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ijn.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jyx.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ksa.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tew.52xcode.cn

[K07] 进制转换
来源：http://ags.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vtm.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mme.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lzo.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wdg.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gzk.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zab.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dbz.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://apl.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://umr.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://teg.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gbj.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://rzy.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://qfp.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sqi.zhoulong.xyz

Go:   encoding/gob
来源：http://ybk.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://jog.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yld.ivvv.top

================================================================================
来源：http://zlw.zhoulong.xyz

L. 网络请求
来源：http://dud.uphjek.com

================================================================================
来源：http://tek.jyoumei.cn

[L01] 发送 GET 请求
来源：http://ekc.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://php.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xax.zhiwuduotai.top

JS:   await fetch(url)
来源：http://fdl.sufxvd.cn

TS:   await fetch(url)
来源：http://snz.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pab.sweek.top

Go:   resp, err := http.Get(url)
来源：http://yga.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xkf.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://spc.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://ubj.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://fvh.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dhv.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ttb.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptp.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://llg.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://crq.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qmx.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://igm.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://fdn.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uza.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://isk.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qxq.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uje.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cbv.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sor.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cxr.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zhu.c1oappe.top

[L04] 设置超时
来源：http://mxn.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://cpd.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://prj.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uut.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bwq.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ajr.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wgu.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eii.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ons.shuidangran.top

[L05] 上传文件（multipart）
来源：http://jgw.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vse.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xtt.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tkc.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tyq.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tam.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ylk.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zye.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zrq.ydzc1.top

[L06] 解析响应为 JSON
来源：http://ztg.zhixingplan.top

Py:   resp.json()
来源：http://mkm.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://hde.yj20258.top

JS:   await resp.json()
来源：http://iot.haohaochexian.top

TS:   await resp.json()
来源：http://hsv.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cfg.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bwx.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://eze.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mfk.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://ysc.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fne.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fup.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://eaa.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://bli.hfpthk.cn

Java: resp.statusCode()
来源：http://per.zdqjudy.top

Go:   resp.StatusCode
来源：http://ktq.xinyue.icu

Ruby: resp.code.to_i
来源：http://pha.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://vui.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://ykk.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://old.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://syd.tarul.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fwy.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dqd.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eae.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://stg.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ihs.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://udm.hysaishi.cn

================================================================================
来源：http://tjv.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://tyc.zhijiandao.cn

================================================================================
来源：http://bdp.andypj.xyz

[M01] 读取命令行参数
来源：http://cnd.xziqi.cn

Py:   sys.argv[1:]
来源：http://vma.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://rru.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://wtw.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://eij.yongpay.top

Java: args 数组（main 方法参数）
来源：http://odu.tianlin.xyz

Go:   os.Args[1:]
来源：http://fbd.yanxiufei.cn

Ruby: ARGV
来源：http://mzs.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://awi.redwolf501.top

[M02] 读取环境变量
来源：http://amz.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://rlm.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xmd.zycfv.cn

JS:   process.env.HOME
来源：http://xqq.yonumen.top

TS:   process.env.HOME
来源：http://ljb.yj202588.top

Java: System.getenv("HOME")
来源：http://bkt.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pxx.smart0.xyz

Ruby: ENV["HOME"]
来源：http://ago.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dti.chenjidiqi.icu

[M03] 执行外部命令
来源：http://iar.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tkz.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://prp.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qxn.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fim.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://acx.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ahi.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yja.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://syv.yuxming.cn

[M04] 获取当前工作目录
来源：http://rbu.jlsjyb.cn

Py:   os.getcwd()
来源：http://jpp.xinyue.icu

PHP:  getcwd();
来源：http://oqv.xuetiantiany.cn

JS:   process.cwd()
来源：http://fjd.smart0.xyz

TS:   process.cwd()
来源：http://wbw.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://ddq.xuanzx.com

Go:   os.Getwd()
来源：http://xvy.xuanzx.com

Ruby: Dir.pwd
来源：http://jsc.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://xmo.zycfv.cn

[M05] 设置退出码
来源：http://pff.xinyue.icu

Py:   sys.exit(1)
来源：http://fej.aizwys.cn

PHP:  exit(1);
来源：http://gkf.jqgufenzy.top

JS:   process.exit(1)
来源：http://ehs.snrcjt.cn

TS:   process.exit(1)
来源：http://tfb.uphjek.com

Java: System.exit(1)
来源：http://fbm.guowangkeji.top

Go:   os.Exit(1)
来源：http://yrh.yj20258888.top

Ruby: exit 1
来源：http://kma.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zns.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://dwf.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://cjy.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vvy.316326.xyz

JS:   console.error("err")
来源：http://nas.cucudq.cn

TS:   console.error("err")
来源：http://bbm.xinyue.icu

Java: System.err.println("err")
来源：http://tmh.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zda.tianlin.xyz

Ruby: warn "err"
来源：http://nfc.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://tum.pengpengdd.cyou

[M07] 判断是否为主入口
来源：http://kdl.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://kif.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rcb.chenlongwang.top

JS:   require.main === module
来源：http://zrt.52xcode.cn

TS:   require.main === module
来源：http://dqi.jiagoushi.top

Java: public static void main(String[] args)
来源：http://nhk.shuidangran.top

Go:   func main()
来源：http://xsl.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ofc.gzhubu.top

C#:   static void Main(string[] args)
来源：http://sxh.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://pcm.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://ywk.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://tku.ehwqpu.com

JS:   process.platform;  process.version
来源：http://hre.cashguo.top

TS:   process.platform;  process.version
来源：http://yue.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://diu.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lgz.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qkp.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eps.52xcode.cn

================================================================================
来源：http://pbs.hongshengwenyu.top

N. 数据结构与算法
来源：http://suz.hysaishi.cn

================================================================================
来源：http://obz.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://kzx.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://eci.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://guh.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pnc.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ley.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://ewg.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://mht.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cee.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://ach.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://esr.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lwh.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sza.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uth.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rsr.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pap.tarul.cn

Go:   slices.Sort(arr)
来源：http://xan.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://oae.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://oyn.yj20258.top

[N03] 快速排序（分治示例）
来源：http://mvr.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ghb.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://klx.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gaf.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aif.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://otw.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eam.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fjm.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rvt.meibo888.top

[N04] 斐波那契数列
来源：http://pvg.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fdq.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sby.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tyc.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxg.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bcl.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cvl.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hcs.tianlin.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zev.hongshengwenyu.top

[N05] 最大公约数
来源：http://jsq.hesvh.cn

Py:   math.gcd(a, b)
来源：http://ynl.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ltb.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://njq.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fol.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xsv.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uoj.cheryme.top

Ruby: a.gcd(b)
来源：http://bgf.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://enx.birdmap.top

[N06] 判断回文字符串
来源：http://tfn.hnqzz.top

Py:   s == s[::-1]
来源：http://dci.redwolf501.top

PHP:  $s === strrev($s);
来源：http://jes.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://gee.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://yoz.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lbd.iojbl.cn

Go:   // 双指针从两端比较
来源：http://hba.yanxiufei.cn

Ruby: s == s.reverse
来源：http://tom.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iyj.sweek.top

[N07] 两数之和（返回下标）
来源：http://cmj.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nen.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oix.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dlz.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://lrl.yj20258888.top

Java: // 手写 HashMap
来源：http://pny.sxryk.cn

Go:   // 手写 map[int]int
来源：http://cjz.jyoumei.cn

Ruby: // 手写 Hash
来源：http://zgi.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://qhe.bbcook.cn

[N08] 生成全排列
来源：http://ddu.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://swn.yongpay.top

PHP:  // 手写递归交换
来源：http://tdh.mhx1999.top

JS:   // 手写回溯递归
来源：http://kdq.xinyue.icu

TS:   // 手写回溯递归
来源：http://czf.daxiang520.top

Java: // 手写回溯递归
来源：http://glv.dianchejie.cn

Go:   // 手写回溯递归
来源：http://vvj.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://sca.gzhubu.top

C#:   // 手写回溯递归
来源：http://ppv.316326.xyz

[N09] 栈与队列
来源：http://aze.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mis.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://olv.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://drt.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qwa.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ypc.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://odd.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uxb.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lxp.wangdashe.top

[N10] 链表节点定义
来源：http://ggo.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ykm.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wac.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hwy.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mpi.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://mbq.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xxx.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rka.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://wxn.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://dxm.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ozo.sxryk.cn

PHP:  // 手写递归函数
来源：http://ccr.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ygf.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oxj.smart0.xyz

Java: // 手写递归
来源：http://zzi.haohaochexian.top

Go:   // 手写递归
来源：http://ozh.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zuc.svipenyu.cn

C#:   // 手写递归
来源：http://yyc.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dxf.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fzb.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://obm.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fcu.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mpw.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hwk.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cqt.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zma.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ryq.yuxming.cn

================================================================================
来源：http://ieu.shanyushiyangkeji.top

O. 并发与异步
来源：http://tdk.bjfxy.top

================================================================================
来源：http://hry.zdbjq.cn

[O01] 启动一个线程
来源：http://dmg.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ozl.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kid.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tlr.tarul.cn

TS:   // 同 JS
来源：http://rrf.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://mic.gogol.net.cn

Go:   go f()
来源：http://ruo.redwolf501.top

Ruby: Thread.new { f }
来源：http://kki.0kj1m.cn

C#:   Task.Run(() => F());
来源：http://olb.yfazqb.com

[O02] 使用线程池
来源：http://wuf.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rtn.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vwv.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://ygp.fengsongda.top


<!-- 参考信息 -->