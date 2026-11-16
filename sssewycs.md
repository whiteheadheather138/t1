代发 wailian999

[K06] 解析 URL 查询串
来源：http://qaq.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uag.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hte.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://riv.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lpy.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fef.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oli.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lid.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vqo.guannengcc.top

[K07] 进制转换
来源：http://fdk.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kyz.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vvh.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vjm.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kla.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tbn.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oac.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vra.bjfxy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jtf.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://zlp.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://agt.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tla.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://smc.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://ccg.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sxt.jinqigfzy.top

Go:   encoding/gob
来源：http://dkl.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://ixi.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wca.jinghuilouyu.cn

================================================================================
来源：http://fpu.tian-w.cn

L. 网络请求
来源：http://onl.cdnleiting.top

================================================================================
来源：http://pde.yonumen.top

[L01] 发送 GET 请求
来源：http://dju.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kng.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bar.zhiwuduotai.top

JS:   await fetch(url)
来源：http://twd.nanxuanxn.top

TS:   await fetch(url)
来源：http://sws.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vtq.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://tch.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rja.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qvu.guowangkeji.top

[L02] 发送 POST JSON
来源：http://ibm.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://apg.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mdx.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kih.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gux.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fve.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ovq.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gqv.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rfb.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://hbv.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wij.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hnw.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ruv.sxryk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jel.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awu.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kie.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tjx.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vdk.yongpay.top

[L04] 设置超时
来源：http://ndm.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://tqp.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://asb.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bif.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjw.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rlg.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ycu.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ucg.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://byb.yj20258888.top

[L05] 上传文件（multipart）
来源：http://cnj.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ttu.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pte.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wbp.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bbm.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qvt.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uga.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yqr.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://olq.hammf.cn

[L06] 解析响应为 JSON
来源：http://dmb.fanxiaobao.xyz

Py:   resp.json()
来源：http://unx.mhx1999.top

PHP:  json_decode($body, true);
来源：http://jip.vehdjk.com

JS:   await resp.json()
来源：http://fnk.sxryk.cn

TS:   await resp.json()
来源：http://njq.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fke.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xxd.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://zkh.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sui.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://lvb.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yqm.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://boc.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://zro.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://onh.0kj1m.cn

Java: resp.statusCode()
来源：http://nyr.ybcxt.top

Go:   resp.StatusCode
来源：http://jiw.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://hmu.havefunace.top

C#:   (int)resp.StatusCode
来源：http://lpw.haohaochexian.top

[L08] 并发请求多个地址
来源：http://bgm.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mqk.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://sph.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://joj.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uwz.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jmp.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yjb.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pbq.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gii.xylfe.cn

================================================================================
来源：http://uen.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://qkm.nanxinkj.top

================================================================================
来源：http://fhl.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://rzf.hammf.cn

Py:   sys.argv[1:]
来源：http://uhp.316326.xyz

PHP:  $argv;  $argc;
来源：http://fyu.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://pdy.tian-w.cn

TS:   process.argv.slice(2)
来源：http://awf.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://pjg.xinyue.icu

Go:   os.Args[1:]
来源：http://snq.ybcxt.top

Ruby: ARGV
来源：http://avp.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://nlc.xuanzx.com

[M02] 读取环境变量
来源：http://sge.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://eew.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://woj.hesvh.cn

JS:   process.env.HOME
来源：http://bjy.chenzaomai.com

TS:   process.env.HOME
来源：http://uxq.zhixingplan.top

Java: System.getenv("HOME")
来源：http://lvl.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zdj.epnwcf.com

Ruby: ENV["HOME"]
来源：http://jbe.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gop.316326.xyz

[M03] 执行外部命令
来源：http://mub.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oec.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xlk.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dre.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kes.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tpe.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://itm.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ivi.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://yge.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://ksz.nanxuanxn.top

Py:   os.getcwd()
来源：http://qwx.wangdashe.top

PHP:  getcwd();
来源：http://qgw.nwbrower.top

JS:   process.cwd()
来源：http://vcz.quarkkingdee.top

TS:   process.cwd()
来源：http://efx.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://ijs.dianchejie.cn

Go:   os.Getwd()
来源：http://bmn.gogol.net.cn

Ruby: Dir.pwd
来源：http://tav.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ftz.zycfv.cn

[M05] 设置退出码
来源：http://thz.quarkkingdee.top

Py:   sys.exit(1)
来源：http://bpw.yj20258.top

PHP:  exit(1);
来源：http://xip.c1oappe.top

JS:   process.exit(1)
来源：http://jqz.pengpengdd.cyou

TS:   process.exit(1)
来源：http://szy.yuxming.cn

Java: System.exit(1)
来源：http://spr.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://erx.ydzc1.top

Ruby: exit 1
来源：http://oee.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ept.yuxming.cn

[M06] 向标准错误输出
来源：http://bwn.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://bux.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://los.chenjidiqi.icu

JS:   console.error("err")
来源：http://zye.tianlin.xyz

TS:   console.error("err")
来源：http://hfa.havefunace.top

Java: System.err.println("err")
来源：http://lgb.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wei.gaohongyu789.top

Ruby: warn "err"
来源：http://wyk.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://fks.ivvv.top

[M07] 判断是否为主入口
来源：http://uml.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://ijn.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oxk.dianchejie.cn

JS:   require.main === module
来源：http://mzl.haohaochexian.top

TS:   require.main === module
来源：http://zzp.hammf.cn

Java: public static void main(String[] args)
来源：http://iql.smart0.xyz

Go:   func main()
来源：http://lbo.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yrx.gzhubu.top

C#:   static void Main(string[] args)
来源：http://vdv.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://kug.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://spv.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://qdq.fengsongda.top

JS:   process.platform;  process.version
来源：http://ihc.cheryme.top

TS:   process.platform;  process.version
来源：http://qnl.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://spv.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tmx.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ntx.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://stn.wangshuangyany.cn

================================================================================
来源：http://wyh.hfpthk.cn

N. 数据结构与算法
来源：http://xlu.zdqjudy.top

================================================================================
来源：http://kpf.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://lyn.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://dhx.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://llq.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mkr.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ohy.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://gtt.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://uey.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tas.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eks.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cjp.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://rma.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dnb.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tiy.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fkv.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kau.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://wty.tian-w.cn

Ruby: arr.sort
来源：http://jye.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xfu.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://jnq.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://msq.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://ksf.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zzf.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ryf.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://azd.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fud.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nfj.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://dkr.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://nei.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://spr.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iyo.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uoz.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lov.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bni.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zit.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvk.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ksc.feifeiyinyue.top

[N05] 最大公约数
来源：http://iic.wangdashe.top

Py:   math.gcd(a, b)
来源：http://lee.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://czg.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zft.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vlr.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tbz.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gtp.birdmap.top

Ruby: a.gcd(b)
来源：http://pkb.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dak.bbcook.cn

[N06] 判断回文字符串
来源：http://dnl.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://xol.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://gmt.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://cuk.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://zln.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wvr.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://ypm.ydzc1.top

Ruby: s == s.reverse
来源：http://rws.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vwi.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://uvx.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iuc.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yzu.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ykp.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://jjb.jiagoushi.top

Java: // 手写 HashMap
来源：http://rgy.xinyue.icu

Go:   // 手写 map[int]int
来源：http://gbt.uphjek.com

Ruby: // 手写 Hash
来源：http://nie.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://ryj.tianlin.xyz

[N08] 生成全排列
来源：http://yyp.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://bke.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://sel.zdbjq.cn

JS:   // 手写回溯递归
来源：http://lmb.jqgfzy.top

TS:   // 手写回溯递归
来源：http://tap.yfazqb.com

Java: // 手写回溯递归
来源：http://twe.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://xzi.316326.xyz

Ruby: arr.permutation.to_a
来源：http://uuv.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://dvs.jlsjyb.cn

[N09] 栈与队列
来源：http://irh.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://psp.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://egc.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lgy.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ujb.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uzo.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mmo.yongpay.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wkx.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lrf.9152youxi.cn

[N10] 链表节点定义
来源：http://grl.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://upf.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bbs.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gus.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hbj.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://ulb.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wno.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://few.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rau.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://xda.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sfu.jyoumei.cn

PHP:  // 手写递归函数
来源：http://wbn.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://srb.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oov.hnxiangtu.top

Java: // 手写递归
来源：http://nrc.hfpthk.cn

Go:   // 手写递归
来源：http://kax.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ddc.yj202588.top

C#:   // 手写递归
来源：http://yma.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jti.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rmj.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ahf.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gcp.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://igt.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qnb.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uzw.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wnx.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pvr.hfpthk.cn

================================================================================
来源：http://arh.fzhhl.top

O. 并发与异步
来源：http://fyn.gaohongyu789.top

================================================================================
来源：http://stm.gzhubu.top

[O01] 启动一个线程
来源：http://ecy.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gmq.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ona.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uqw.yongpay.top

TS:   // 同 JS
来源：http://muc.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://ykh.yj20258888.top

Go:   go f()
来源：http://mfh.zhixingplan.top

Ruby: Thread.new { f }
来源：http://nzz.shuidangran.top

C#:   Task.Run(() => F());
来源：http://lih.jinghuilouyu.cn


<!-- 参考信息 -->