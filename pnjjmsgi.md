代发 wailian999

[K06] 解析 URL 查询串
来源：http://qzn.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wze.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rfy.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fjs.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://koo.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ksk.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pqv.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gal.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mfn.hfpthk.cn

[K07] 进制转换
来源：http://olg.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gmx.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://htz.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lle.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nat.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ldi.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://daz.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mpw.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://png.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://esu.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://uje.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qhe.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://keg.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://pog.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gnv.snrcjt.cn

Go:   encoding/gob
来源：http://bla.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://phc.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fwo.havefunace.top

================================================================================
来源：http://ygo.hywenlv.cn

L. 网络请求
来源：http://cfg.zdqjudy.top

================================================================================
来源：http://vjo.meibo888.top

[L01] 发送 GET 请求
来源：http://tup.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uvp.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ahz.bbcook.cn

JS:   await fetch(url)
来源：http://xlf.sysykeji.top

TS:   await fetch(url)
来源：http://oxq.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zjy.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://rse.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hzx.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xln.fktsv.cn

[L02] 发送 POST JSON
来源：http://wez.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://bax.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eeo.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lon.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lno.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ltz.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wno.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://crq.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mdc.cashguo.top

[L03] 设置自定义请求头
来源：http://uag.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wic.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uxx.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yuc.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uok.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kec.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://toa.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://suf.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ylo.hywenlv.cn

[L04] 设置超时
来源：http://fff.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://bor.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://duu.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ylu.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fty.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://slv.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ofs.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yha.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mnc.guannengcc.top

[L05] 上传文件（multipart）
来源：http://lkz.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kcz.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nxh.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kjp.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wmo.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ajz.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kya.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ryk.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zvw.guannengcc.top

[L06] 解析响应为 JSON
来源：http://eav.haohaochexian.top

Py:   resp.json()
来源：http://pgc.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://ivz.zhoulong.xyz

JS:   await resp.json()
来源：http://gbg.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://qmt.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tpz.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tcf.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://ofh.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://par.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://lty.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jvu.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zzx.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://otv.ivvv.top

TS:   resp.ok;  resp.status
来源：http://xcx.guowangkeji.top

Java: resp.statusCode()
来源：http://dxn.tian-w.cn

Go:   resp.StatusCode
来源：http://jlr.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://qxn.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://osf.birdmap.top

[L08] 并发请求多个地址
来源：http://ahe.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sbc.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://jnb.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bpo.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ueh.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ltt.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ssg.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xbi.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oop.ydjk.org.cn

================================================================================
来源：http://gsr.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://lbz.xuetiantiany.cn

================================================================================
来源：http://lcl.yfazqb.com

[M01] 读取命令行参数
来源：http://xhu.haohaochexian.top

Py:   sys.argv[1:]
来源：http://tsl.tian-w.cn

PHP:  $argv;  $argc;
来源：http://gao.sweek.top

JS:   process.argv.slice(2)
来源：http://cqe.uphjek.com

TS:   process.argv.slice(2)
来源：http://mse.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://nkh.hammf.cn

Go:   os.Args[1:]
来源：http://jck.hesvh.cn

Ruby: ARGV
来源：http://vli.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://faz.nanxinkj.top

[M02] 读取环境变量
来源：http://tav.meibo888.top

Py:   os.environ.get("HOME")
来源：http://pef.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tdo.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://lri.zhongyouzk.top

TS:   process.env.HOME
来源：http://jkt.9152youxi.cn

Java: System.getenv("HOME")
来源：http://bbq.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vnk.hesvh.cn

Ruby: ENV["HOME"]
来源：http://swn.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://znu.yfazqb.com

[M03] 执行外部命令
来源：http://awf.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://svu.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uyv.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pni.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cjp.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wsu.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://pwj.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://hkg.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://nbz.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://gir.ydzc1.top

Py:   os.getcwd()
来源：http://xdm.chenzaomai.com

PHP:  getcwd();
来源：http://onr.tianlin.xyz

JS:   process.cwd()
来源：http://jex.fengsongda.top

TS:   process.cwd()
来源：http://xvs.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://crf.zhongyouzk.top

Go:   os.Getwd()
来源：http://gvu.zhengqikj.top

Ruby: Dir.pwd
来源：http://knm.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://bko.hywenlv.cn

[M05] 设置退出码
来源：http://chu.yongpay.top

Py:   sys.exit(1)
来源：http://ffn.jqgufenzy.top

PHP:  exit(1);
来源：http://qco.yuanzhike.top

JS:   process.exit(1)
来源：http://kzr.hesvh.cn

TS:   process.exit(1)
来源：http://fkq.chenlongwang.top

Java: System.exit(1)
来源：http://zkw.snrcjt.cn

Go:   os.Exit(1)
来源：http://luv.nwbrower.top

Ruby: exit 1
来源：http://ruo.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lui.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://uaj.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://jef.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wta.aizwys.cn

JS:   console.error("err")
来源：http://jxc.hongshengwenyu.top

TS:   console.error("err")
来源：http://vsp.cheryme.top

Java: System.err.println("err")
来源：http://ygr.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ztt.wangdashe.top

Ruby: warn "err"
来源：http://rkj.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://wxn.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://dlj.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://fjv.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bif.ctjpmb.com

JS:   require.main === module
来源：http://eil.sysykeji.top

TS:   require.main === module
来源：http://vdq.nanxuanxn.top

Java: public static void main(String[] args)
来源：http://gqt.chenlongwang.top

Go:   func main()
来源：http://gic.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://adq.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://hhb.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://rgd.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://ypn.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://koe.yj202588.top

JS:   process.platform;  process.version
来源：http://zfo.svipenyu.cn

TS:   process.platform;  process.version
来源：http://tgp.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qwv.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tks.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qub.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vjx.cashguo.top

================================================================================
来源：http://ebt.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://kju.ppjwa.cn

================================================================================
来源：http://btc.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://wbi.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://vic.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dec.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbq.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qeb.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mnv.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://tnj.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lhr.quarkkingdee.top

C#:   Array.BinarySearch(arr, x)
来源：http://idv.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://vud.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://dyk.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qbx.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://agd.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lzn.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://beu.fehbvm.com

Go:   slices.Sort(arr)
来源：http://lrc.hnxiangtu.top

Ruby: arr.sort
来源：http://sjg.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eis.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://ypi.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vxe.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://uwn.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvv.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mdl.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wpj.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cwe.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ibh.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://hjs.tarul.cn

[N04] 斐波那契数列
来源：http://rqj.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yrg.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://znz.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kvv.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zab.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xdo.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ubd.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pqs.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rta.hongshengwenyu.top

[N05] 最大公约数
来源：http://lvp.sysykeji.top

Py:   math.gcd(a, b)
来源：http://yuu.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oew.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zoh.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqn.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kji.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nmi.tianlin.xyz

Ruby: a.gcd(b)
来源：http://ctk.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oee.zhoulong.xyz

[N06] 判断回文字符串
来源：http://rgc.vqdsnc.cn

Py:   s == s[::-1]
来源：http://nal.uphjek.com

PHP:  $s === strrev($s);
来源：http://gjy.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://swd.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://uis.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yxu.nwbrower.top

Go:   // 双指针从两端比较
来源：http://xhs.fengsongda.top

Ruby: s == s.reverse
来源：http://zrv.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nrc.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://tdy.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ixs.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tbi.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://brn.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://qmx.guowangkeji.top

Java: // 手写 HashMap
来源：http://ztq.jianghu66.top

Go:   // 手写 map[int]int
来源：http://qln.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://hcx.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://bxo.yanxiufei.cn

[N08] 生成全排列
来源：http://ukh.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://gyp.vehdjk.com

PHP:  // 手写递归交换
来源：http://ymk.snrcjt.cn

JS:   // 手写回溯递归
来源：http://ced.316326.xyz

TS:   // 手写回溯递归
来源：http://mef.yangfankeji.com

Java: // 手写回溯递归
来源：http://ccv.dashuyun.cn

Go:   // 手写回溯递归
来源：http://jyk.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://dnf.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://vph.jinqigfzy.top

[N09] 栈与队列
来源：http://vvb.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rpg.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfq.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zqq.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cxx.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rkg.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uid.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dsj.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sxa.316326.xyz

[N10] 链表节点定义
来源：http://cra.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jwz.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hpb.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yhc.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vqz.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://nlo.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://ckg.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dns.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jat.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://lqw.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ctd.chenlongwang.top

PHP:  // 手写递归函数
来源：http://ecf.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nhg.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yka.zhaomingkeji.xyz

Java: // 手写递归
来源：http://odl.tanke756.top

Go:   // 手写递归
来源：http://bha.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qqj.iojbl.cn

C#:   // 手写递归
来源：http://qcf.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hcg.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qwd.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xcs.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nhs.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yuw.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jdf.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyl.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sim.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ukd.sufxvd.cn

================================================================================
来源：http://ciw.jiagoushi.top

O. 并发与异步
来源：http://hjq.sysykeji.top

================================================================================
来源：http://bso.fktsv.cn

[O01] 启动一个线程
来源：http://lvw.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pem.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wxq.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rgy.feifeiyinyue.top

TS:   // 同 JS
来源：http://ilc.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://mxm.xziqi.cn

Go:   go f()
来源：http://adj.jqgfzy.top

Ruby: Thread.new { f }
来源：http://mcx.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://jks.shanyushiyangkeji.top


<!-- 参考信息 -->