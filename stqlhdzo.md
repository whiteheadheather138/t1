代发 wailian999

[K06] 解析 URL 查询串
来源：http://rbj.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fcx.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://suj.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dic.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jny.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ikt.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mfo.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oum.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dik.cashguo.top

[K07] 进制转换
来源：http://dxh.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://chr.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ziq.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wgl.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fks.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hpv.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://krh.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jzg.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iog.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://vvt.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://ybm.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pmb.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://cly.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://eym.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://spt.guannengcc.top

Go:   encoding/gob
来源：http://dbc.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://nym.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kfy.dashuyun.cn

================================================================================
来源：http://rqa.yvedp.cn

L. 网络请求
来源：http://czs.uphjek.com

================================================================================
来源：http://rpb.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://lmv.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pej.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xce.hnqzz.top

JS:   await fetch(url)
来源：http://cjh.xuetiantiany.cn

TS:   await fetch(url)
来源：http://kvo.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://awy.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://wst.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://cew.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sha.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://oun.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://fvb.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qon.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccw.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://owc.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tgl.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://etl.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lgn.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hpl.c1oappe.top

[L03] 设置自定义请求头
来源：http://phq.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bgf.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mbj.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gme.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qxd.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yzm.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dxd.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zoq.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vax.xinyue.icu

[L04] 设置超时
来源：http://gac.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://cgo.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gaw.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uae.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wnv.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://edn.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zdf.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zgb.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qlw.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://qax.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iih.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zvq.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://slp.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vyn.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uxe.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pdg.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cgd.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tmi.andypj.xyz

[L06] 解析响应为 JSON
来源：http://jro.aibaodan.cn

Py:   resp.json()
来源：http://rud.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://egt.hongshengwenyu.top

JS:   await resp.json()
来源：http://eua.yj202588.top

TS:   await resp.json()
来源：http://lxi.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jlq.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kbn.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://loa.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qmt.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://czy.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hnm.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zoz.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://glj.tanke756.top

TS:   resp.ok;  resp.status
来源：http://gip.yj20258.top

Java: resp.statusCode()
来源：http://fwl.52xcode.cn

Go:   resp.StatusCode
来源：http://zic.fengsongda.top

Ruby: resp.code.to_i
来源：http://fbb.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://ppj.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://hzp.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nzy.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://chm.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iyi.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dmf.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oof.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yzl.gogol.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qnv.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hfl.fanxiaobao.xyz

================================================================================
来源：http://alb.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://fgg.shuidangran.top

================================================================================
来源：http://mcu.smart0.xyz

[M01] 读取命令行参数
来源：http://lok.yueranfly.top

Py:   sys.argv[1:]
来源：http://ixp.sysykeji.top

PHP:  $argv;  $argc;
来源：http://cts.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://dvj.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://ivs.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://orv.ehwqpu.com

Go:   os.Args[1:]
来源：http://jok.tian-w.cn

Ruby: ARGV
来源：http://ugc.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://das.gotoacloud.top

[M02] 读取环境变量
来源：http://cyo.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://cqf.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fgk.fengsongda.top

JS:   process.env.HOME
来源：http://zob.52xcode.cn

TS:   process.env.HOME
来源：http://grv.andypj.xyz

Java: System.getenv("HOME")
来源：http://git.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://psr.xuanzx.com

Ruby: ENV["HOME"]
来源：http://stm.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://llm.316326.xyz

[M03] 执行外部命令
来源：http://zlj.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://krd.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qpe.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hxn.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ujb.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kxm.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hpx.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tag.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://wpm.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://anq.zdbjq.cn

Py:   os.getcwd()
来源：http://and.yj20258.top

PHP:  getcwd();
来源：http://itv.sxryk.cn

JS:   process.cwd()
来源：http://cno.tanke756.top

TS:   process.cwd()
来源：http://ahq.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://bzn.fehbvm.com

Go:   os.Getwd()
来源：http://sya.cdnleiting.top

Ruby: Dir.pwd
来源：http://fbz.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://slj.zhoulong.xyz

[M05] 设置退出码
来源：http://ozc.jlsjyb.cn

Py:   sys.exit(1)
来源：http://ktk.yj202588.top

PHP:  exit(1);
来源：http://xvx.316326.xyz

JS:   process.exit(1)
来源：http://kov.yuxming.cn

TS:   process.exit(1)
来源：http://zjv.fehbvm.com

Java: System.exit(1)
来源：http://bae.meibo888.top

Go:   os.Exit(1)
来源：http://ljj.tarul.cn

Ruby: exit 1
来源：http://moo.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ibo.jqgufenzy.top

[M06] 向标准错误输出
来源：http://rrp.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://kmg.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://iwk.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://snm.yvedp.cn

TS:   console.error("err")
来源：http://rop.fengsongda.top

Java: System.err.println("err")
来源：http://hnm.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gih.ppjwa.cn

Ruby: warn "err"
来源：http://zhk.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://xbn.daria6918.cn

[M07] 判断是否为主入口
来源：http://rwq.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://for.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fui.birdmap.top

JS:   require.main === module
来源：http://drs.yongpay.top

TS:   require.main === module
来源：http://uvt.smart0.xyz

Java: public static void main(String[] args)
来源：http://fwr.vehdjk.com

Go:   func main()
来源：http://qxk.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xds.ivvv.top

C#:   static void Main(string[] args)
来源：http://pac.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://qks.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://fdt.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://obe.svipenyu.cn

JS:   process.platform;  process.version
来源：http://ntk.zycfv.cn

TS:   process.platform;  process.version
来源：http://oxx.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ssc.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yaw.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ewo.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pdd.pengpengdd.cyou

================================================================================
来源：http://sqv.wangdashe.top

N. 数据结构与算法
来源：http://uph.xingfuxueyuan.xyz

================================================================================
来源：http://oac.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://res.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xqa.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vkn.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hox.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ahw.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://zhi.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://wwn.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pmb.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://vlh.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://lzn.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://oae.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dyc.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sjd.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uxz.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xka.bbcook.cn

Go:   slices.Sort(arr)
来源：http://sdq.iojbl.cn

Ruby: arr.sort
来源：http://qms.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://mgq.316326.xyz

[N03] 快速排序（分治示例）
来源：http://rco.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://orn.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://pqz.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jhn.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogy.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gej.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zhz.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://msb.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://etn.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://tyr.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tok.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jap.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://efg.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://thy.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lqe.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jbc.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hhc.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://boj.c1oappe.top

[N05] 最大公约数
来源：http://gsv.ybcxt.top

Py:   math.gcd(a, b)
来源：http://fii.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tcp.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bwn.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://riv.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wim.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xfm.cashguo.top

Ruby: a.gcd(b)
来源：http://arq.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fll.wangdashe.top

[N06] 判断回文字符串
来源：http://crp.zhongyouzk.top

Py:   s == s[::-1]
来源：http://yih.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://gky.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://xkq.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://ovy.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zoi.andypj.xyz

Go:   // 双指针从两端比较
来源：http://nbe.tanke756.top

Ruby: s == s.reverse
来源：http://ric.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fap.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://hlb.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xzk.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vup.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jzq.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://rmj.tian-w.cn

Java: // 手写 HashMap
来源：http://xng.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://ici.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://drn.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://zti.cashguo.top

[N08] 生成全排列
来源：http://igm.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://nvc.chenlongwang.top

PHP:  // 手写递归交换
来源：http://nvr.nanxinkj.top

JS:   // 手写回溯递归
来源：http://awd.hnqzz.top

TS:   // 手写回溯递归
来源：http://oph.ydjk.org.cn

Java: // 手写回溯递归
来源：http://vhf.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://oic.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://yni.zycfv.cn

C#:   // 手写回溯递归
来源：http://syd.xuanzx.com

[N09] 栈与队列
来源：http://kwn.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pif.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cae.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pbp.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dby.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ugz.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ldf.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vsp.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xfz.aizwys.cn

[N10] 链表节点定义
来源：http://qse.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://noq.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ufu.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://njb.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://whb.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://vot.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://skg.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mcw.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://uve.yongpay.top

[N11] 二叉树中序遍历
来源：http://umf.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ecs.ppjwa.cn

PHP:  // 手写递归函数
来源：http://hzx.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eik.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://duu.gaohongyu789.top

Java: // 手写递归
来源：http://gqe.yuanzhike.top

Go:   // 手写递归
来源：http://ssz.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mhu.yonumen.top

C#:   // 手写递归
来源：http://egz.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kxe.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aoz.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tkx.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://isc.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgj.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pce.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pdr.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://phm.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://clb.daria6918.cn

================================================================================
来源：http://ump.sufxvd.cn

O. 并发与异步
来源：http://wdz.52xcode.cn

================================================================================
来源：http://uyf.mhx1999.top

[O01] 启动一个线程
来源：http://muw.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rgm.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://slu.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pmx.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://deu.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://pmv.chenzaomai.com

Go:   go f()
来源：http://aht.ybcxt.top

Ruby: Thread.new { f }
来源：http://cxd.ydzc1.top

C#:   Task.Run(() => F());
来源：http://apa.sweek.top


<!-- 参考信息 -->