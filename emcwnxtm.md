代发 wailian999

[K06] 解析 URL 查询串
来源：http://bec.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zkx.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xup.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mkr.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hrj.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sro.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pom.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zmo.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://prb.shuidangran.top

[K07] 进制转换
来源：http://nhg.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bef.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xjq.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://npk.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tec.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dym.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iuq.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iuw.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pdx.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://zor.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://bni.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://pod.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://woo.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://inw.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mzm.dashuyun.cn

Go:   encoding/gob
来源：http://fzn.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://cdj.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hpz.jiagoushi.top

================================================================================
来源：http://yxe.ctjpmb.com

L. 网络请求
来源：http://ytl.mhx1999.top

================================================================================
来源：http://zit.cqqwz.cn

[L01] 发送 GET 请求
来源：http://rvl.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dnb.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://alj.ehwqpu.com

JS:   await fetch(url)
来源：http://waa.gaohongyu789.top

TS:   await fetch(url)
来源：http://kgg.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxq.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://knb.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tok.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bwj.nwbrower.top

[L02] 发送 POST JSON
来源：http://bol.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lll.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://olo.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rwz.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gpp.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://azu.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ovy.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ihr.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pbo.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://dvh.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uoy.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vyy.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pgl.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vpl.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rsk.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xua.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://plq.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bgd.gogol.net.cn

[L04] 设置超时
来源：http://tra.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://ork.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uyy.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://res.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://klf.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://axb.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jcf.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dvy.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yfa.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://ump.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gcx.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lap.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fcz.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wcw.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dmg.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qog.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cro.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sms.zycfv.cn

[L06] 解析响应为 JSON
来源：http://hqj.zhoulong.xyz

Py:   resp.json()
来源：http://yfp.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://ewx.shuidangran.top

JS:   await resp.json()
来源：http://zdn.fanxiaobao.xyz

TS:   await resp.json()
来源：http://ozi.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dve.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sxo.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://tff.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zog.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://orp.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ccz.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ywe.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://zyj.tarul.cn

TS:   resp.ok;  resp.status
来源：http://wit.xuetiantiany.cn

Java: resp.statusCode()
来源：http://imf.cheryme.top

Go:   resp.StatusCode
来源：http://djd.zhengqikj.top

Ruby: resp.code.to_i
来源：http://yvl.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://pmh.dashuyun.cn

[L08] 并发请求多个地址
来源：http://nhj.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://skx.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://fqp.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pdj.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wuh.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zxr.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dnk.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nqc.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://col.ppjwa.cn

================================================================================
来源：http://icg.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://opw.gogol.net.cn

================================================================================
来源：http://cqm.xinyue.icu

[M01] 读取命令行参数
来源：http://gml.hesvh.cn

Py:   sys.argv[1:]
来源：http://ggv.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://uks.guannengcc.top

JS:   process.argv.slice(2)
来源：http://pel.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://mzs.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://pvq.gotoacloud.top

Go:   os.Args[1:]
来源：http://svd.zhijiandao.cn

Ruby: ARGV
来源：http://qvs.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://kre.yj20258888.top

[M02] 读取环境变量
来源：http://tyv.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://hbl.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vdr.nwbrower.top

JS:   process.env.HOME
来源：http://gtm.zhongyouzk.top

TS:   process.env.HOME
来源：http://ynn.jinqigufen.top

Java: System.getenv("HOME")
来源：http://aya.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fhq.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://lom.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xts.316326.xyz

[M03] 执行外部命令
来源：http://jbd.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jvi.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kdm.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vkn.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pan.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zyp.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xsv.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://rsv.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://pyx.iojbl.cn

[M04] 获取当前工作目录
来源：http://esk.fktsv.cn

Py:   os.getcwd()
来源：http://mlu.tarul.cn

PHP:  getcwd();
来源：http://mhf.sjlbkw.cn

JS:   process.cwd()
来源：http://cux.gotoacloud.top

TS:   process.cwd()
来源：http://bco.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://wrz.ehwqpu.com

Go:   os.Getwd()
来源：http://fxh.jinqigufen.top

Ruby: Dir.pwd
来源：http://dgr.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yjp.hcnkem.com

[M05] 设置退出码
来源：http://exn.fehbvm.com

Py:   sys.exit(1)
来源：http://rvo.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://tpp.gaohongyu789.top

JS:   process.exit(1)
来源：http://mfr.tianlin.xyz

TS:   process.exit(1)
来源：http://mew.nanxinkj.top

Java: System.exit(1)
来源：http://vdj.52xcode.cn

Go:   os.Exit(1)
来源：http://aud.sjlbkw.cn

Ruby: exit 1
来源：http://ccf.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qio.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://gfr.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://bka.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ict.tarul.cn

JS:   console.error("err")
来源：http://ymm.epnwcf.com

TS:   console.error("err")
来源：http://ixx.aibaodan.cn

Java: System.err.println("err")
来源：http://smj.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qkl.gaohongyu789.top

Ruby: warn "err"
来源：http://ahk.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://zns.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://jha.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://jzv.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yib.zdbjq.cn

JS:   require.main === module
来源：http://xwp.daria6918.cn

TS:   require.main === module
来源：http://aaj.jyoumei.cn

Java: public static void main(String[] args)
来源：http://bis.c1oappe.top

Go:   func main()
来源：http://lkd.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lxn.meibo888.top

C#:   static void Main(string[] args)
来源：http://nxq.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://eiv.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://oot.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ald.hesvh.cn

JS:   process.platform;  process.version
来源：http://wrb.epnwcf.com

TS:   process.platform;  process.version
来源：http://gxj.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ukg.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://pvz.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zzd.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://agj.tanke756.top

================================================================================
来源：http://ljn.uphjek.com

N. 数据结构与算法
来源：http://zef.yj20258.top

================================================================================
来源：http://yay.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://zsa.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://aqr.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jgf.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cxo.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mkr.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://psm.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://rgd.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ost.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://epj.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://iee.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://lxy.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kxk.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oef.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bty.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vur.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://vkx.sysykeji.top

Ruby: arr.sort
来源：http://jfp.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://anl.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://opq.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cll.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://tav.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipe.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://myk.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ghb.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://syo.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qbl.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ojf.0kj1m.cn

[N04] 斐波那契数列
来源：http://izc.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hnq.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zdp.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsb.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bmo.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://diu.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jvn.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hep.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vei.iojbl.cn

[N05] 最大公约数
来源：http://itf.yj20258.top

Py:   math.gcd(a, b)
来源：http://hpn.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xma.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ils.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zmn.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bal.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xxl.daria6918.cn

Ruby: a.gcd(b)
来源：http://fql.tianlin.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vle.zdbjq.cn

[N06] 判断回文字符串
来源：http://zzz.dashuyun.cn

Py:   s == s[::-1]
来源：http://tvc.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://ben.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://hcs.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://uhy.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mjc.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://ocx.52xcode.cn

Ruby: s == s.reverse
来源：http://cpx.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fcf.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://owr.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://udi.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gtz.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qpx.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://ohk.daria6918.cn

Java: // 手写 HashMap
来源：http://cqy.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://aah.sysykeji.top

Ruby: // 手写 Hash
来源：http://pph.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://elz.jlsjyb.cn

[N08] 生成全排列
来源：http://yat.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://iwy.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://mxk.cucudq.cn

JS:   // 手写回溯递归
来源：http://hml.smart0.xyz

TS:   // 手写回溯递归
来源：http://afn.quarkkingdee.top

Java: // 手写回溯递归
来源：http://rzv.daxiang520.top

Go:   // 手写回溯递归
来源：http://hnp.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://krp.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://zax.hysaishi.cn

[N09] 栈与队列
来源：http://zmn.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fac.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oov.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aea.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ijo.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oyw.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://amj.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eol.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://juo.hesvh.cn

[N10] 链表节点定义
来源：http://imu.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://brz.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eub.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bev.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rae.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://zwh.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hol.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dso.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fyu.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://tlt.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bvy.epnwcf.com

PHP:  // 手写递归函数
来源：http://cvw.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqs.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jzk.chenzaomai.com

Java: // 手写递归
来源：http://vmg.tian-w.cn

Go:   // 手写递归
来源：http://emu.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rhw.yvedp.cn

C#:   // 手写递归
来源：http://ujh.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hky.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pxg.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zxg.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qzb.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbo.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zxf.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pum.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pqz.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yqp.cucudq.cn

================================================================================
来源：http://moa.gotoacloud.top

O. 并发与异步
来源：http://uwx.zycfv.cn

================================================================================
来源：http://awo.ppjwa.cn

[O01] 启动一个线程
来源：http://xtl.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vrp.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zro.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qqu.fktsv.cn

TS:   // 同 JS
来源：http://ujv.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://eud.daxiang520.top

Go:   go f()
来源：http://iej.zdqjudy.top

Ruby: Thread.new { f }
来源：http://lnc.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://okk.jlsjyb.cn


<!-- 参考信息 -->