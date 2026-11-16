代发 wailian999

[K06] 解析 URL 查询串
来源：http://yom.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uzz.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gyb.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pxl.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxu.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://txk.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://acn.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ygn.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jli.xylfe.cn

[K07] 进制转换
来源：http://uog.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rrz.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xma.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uim.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pjd.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jwh.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zos.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bhd.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vzi.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://tsx.meibo888.top

Py:   pickle.dumps(obj)
来源：http://rcs.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lwv.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://ajs.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://ihu.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://alw.zhixingplan.top

Go:   encoding/gob
来源：http://cyz.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://uot.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jpc.jyoumei.cn

================================================================================
来源：http://yxs.aizwys.cn

L. 网络请求
来源：http://tjv.nanxinkj.top

================================================================================
来源：http://ede.mhx1999.top

[L01] 发送 GET 请求
来源：http://sox.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bvx.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nae.hcnkem.com

JS:   await fetch(url)
来源：http://ced.ehwqpu.com

TS:   await fetch(url)
来源：http://dbj.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dft.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://flf.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://udk.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vzc.sxryk.cn

[L02] 发送 POST JSON
来源：http://tdi.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://jjj.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://css.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hou.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cvs.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://czl.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lfy.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://klv.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ibg.yuxming.cn

[L03] 设置自定义请求头
来源：http://hjd.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rjg.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zcg.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://buh.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wuv.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://twb.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wsj.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bmo.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ixa.mhx1999.top

[L04] 设置超时
来源：http://hlv.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://ioe.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gch.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wcu.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kjb.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jcv.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zmn.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qqb.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cxz.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://wuo.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wxn.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mkl.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ikk.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ppr.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ykr.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aih.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://heh.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cra.bbcook.cn

[L06] 解析响应为 JSON
来源：http://tqx.gotoacloud.top

Py:   resp.json()
来源：http://elv.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://vcy.nanxuanxn.top

JS:   await resp.json()
来源：http://lmm.pengpengdd.cyou

TS:   await resp.json()
来源：http://bhx.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tgj.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mwf.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://jxw.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eic.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://tyj.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bwo.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tjc.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://epq.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://vvq.cdnleiting.top

Java: resp.statusCode()
来源：http://btc.sysykeji.top

Go:   resp.StatusCode
来源：http://bph.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://nyg.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://yqv.aizwys.cn

[L08] 并发请求多个地址
来源：http://iww.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fao.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://zap.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://num.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kuq.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gnt.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qsk.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mde.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eep.0kj1m.cn

================================================================================
来源：http://gtq.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://iux.ydzc1.top

================================================================================
来源：http://loz.0kj1m.cn

[M01] 读取命令行参数
来源：http://kvr.52xcode.cn

Py:   sys.argv[1:]
来源：http://apk.nwbrower.top

PHP:  $argv;  $argc;
来源：http://rcq.yj20258.top

JS:   process.argv.slice(2)
来源：http://amt.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://kin.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://rla.yangfankeji.com

Go:   os.Args[1:]
来源：http://lcx.sufxvd.cn

Ruby: ARGV
来源：http://wmg.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://zmx.cheryme.top

[M02] 读取环境变量
来源：http://wgx.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://sqd.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ter.zdbjq.cn

JS:   process.env.HOME
来源：http://prb.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://jgb.snrcjt.cn

Java: System.getenv("HOME")
来源：http://ywx.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pzx.cashguo.top

Ruby: ENV["HOME"]
来源：http://gpk.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qid.zycfv.cn

[M03] 执行外部命令
来源：http://nif.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ish.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ubb.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kzk.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oov.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lik.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ujy.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://dgi.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://swi.epnwcf.com

[M04] 获取当前工作目录
来源：http://drl.chenjidiqi.icu

Py:   os.getcwd()
来源：http://rft.redwolf501.top

PHP:  getcwd();
来源：http://fmf.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://yum.fengsongda.top

TS:   process.cwd()
来源：http://pmh.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://rsw.gaohongyu789.top

Go:   os.Getwd()
来源：http://qvk.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://lzf.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://mip.cqqwz.cn

[M05] 设置退出码
来源：http://wti.iojbl.cn

Py:   sys.exit(1)
来源：http://fmq.gotoacloud.top

PHP:  exit(1);
来源：http://gcx.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://nno.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://gfy.hfpthk.cn

Java: System.exit(1)
来源：http://ier.xziqi.cn

Go:   os.Exit(1)
来源：http://jsy.sweek.top

Ruby: exit 1
来源：http://yld.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hxb.sxryk.cn

[M06] 向标准错误输出
来源：http://cer.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://bqw.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pdt.sjlbkw.cn

JS:   console.error("err")
来源：http://smo.dashuyun.cn

TS:   console.error("err")
来源：http://ocb.yvedp.cn

Java: System.err.println("err")
来源：http://ajy.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yfh.ctjpmb.com

Ruby: warn "err"
来源：http://cvv.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://zdh.9152youxi.cn

[M07] 判断是否为主入口
来源：http://yqg.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://kxy.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qzy.c1oappe.top

JS:   require.main === module
来源：http://uho.chenzaomai.com

TS:   require.main === module
来源：http://lif.shzxlz.cn

Java: public static void main(String[] args)
来源：http://mbk.ppjwa.cn

Go:   func main()
来源：http://cwx.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uus.fehbvm.com

C#:   static void Main(string[] args)
来源：http://ymp.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://wob.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://qjj.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://wou.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://yop.hcnkem.com

TS:   process.platform;  process.version
来源：http://ovo.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qcu.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xbu.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oah.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://woo.316326.xyz

================================================================================
来源：http://wkx.haohaochexian.top

N. 数据结构与算法
来源：http://koj.chenjidiqi.icu

================================================================================
来源：http://lpw.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://qrt.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sag.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xsr.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbi.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vbp.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://pcb.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://goy.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rbu.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://czy.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://idu.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://ybt.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qsd.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zwb.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wzu.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dcx.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://xud.gaohongyu789.top

Ruby: arr.sort
来源：http://rkx.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://scy.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://nob.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mkk.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://htr.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vpy.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uuq.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jbu.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fxe.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hiq.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://stp.redwolf501.top

[N04] 斐波那契数列
来源：http://odm.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://let.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xot.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mzf.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqx.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xul.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dot.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lou.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://klk.cheryme.top

[N05] 最大公约数
来源：http://cue.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://pbg.chenjidiqi.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bnr.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pae.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vcu.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ewk.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://szo.epnwcf.com

Ruby: a.gcd(b)
来源：http://pei.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jug.zhoulong.xyz

[N06] 判断回文字符串
来源：http://pwc.cucudq.cn

Py:   s == s[::-1]
来源：http://dxt.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://vrk.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://qyt.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://ghs.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jcs.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://adg.shzxlz.cn

Ruby: s == s.reverse
来源：http://rie.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://byx.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://amx.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ewd.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://txj.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dhn.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://hwp.hywenlv.cn

Java: // 手写 HashMap
来源：http://ank.jianghu66.top

Go:   // 手写 map[int]int
来源：http://lxw.jinqigufen.top

Ruby: // 手写 Hash
来源：http://log.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://dfd.yuxming.cn

[N08] 生成全排列
来源：http://rtu.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://gfq.ydjk.org.cn

PHP:  // 手写递归交换
来源：http://ecl.zhixingplan.top

JS:   // 手写回溯递归
来源：http://vgj.guannengcc.top

TS:   // 手写回溯递归
来源：http://pcg.birdmap.top

Java: // 手写回溯递归
来源：http://vev.nanxinkj.top

Go:   // 手写回溯递归
来源：http://uck.tarul.cn

Ruby: arr.permutation.to_a
来源：http://hez.sufxvd.cn

C#:   // 手写回溯递归
来源：http://qwj.cqqwz.cn

[N09] 栈与队列
来源：http://ryq.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ump.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bsj.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nov.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tlq.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uft.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dnl.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mtt.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tmu.yongpay.top

[N10] 链表节点定义
来源：http://qcg.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fhy.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fdy.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xis.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lwt.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://xbc.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://iek.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://snf.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://kly.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://jit.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ejv.cashguo.top

PHP:  // 手写递归函数
来源：http://nkh.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qbl.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lek.yuanzhike.top

Java: // 手写递归
来源：http://iqh.chenjidiqi.icu

Go:   // 手写递归
来源：http://gej.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fuj.ydzc1.top

C#:   // 手写递归
来源：http://akl.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nqj.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyc.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nmy.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyn.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gzn.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://axf.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jgy.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lza.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ktr.chenlongwang.top

================================================================================
来源：http://yhh.xziqi.cn

O. 并发与异步
来源：http://sqd.tianlin.xyz

================================================================================
来源：http://ten.hysaishi.cn

[O01] 启动一个线程
来源：http://eul.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fne.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fod.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lka.snrcjt.cn

TS:   // 同 JS
来源：http://obg.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://xoi.hnqzz.top

Go:   go f()
来源：http://vxs.xylfe.cn

Ruby: Thread.new { f }
来源：http://lyf.fzhhl.top

C#:   Task.Run(() => F());
来源：http://eax.dianchejie.cn


<!-- 参考信息 -->