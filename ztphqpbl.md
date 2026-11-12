代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oev.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ljt.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tzs.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uer.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nra.chenjidiqi.icu

[K07] 进制转换
来源：http://etz.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ddo.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bwq.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vrl.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xvk.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ddm.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tsg.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://auk.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ivv.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://vfq.hammf.cn

Py:   pickle.dumps(obj)
来源：http://oji.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zay.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://glz.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://bhs.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ggj.svipenyu.cn

Go:   encoding/gob
来源：http://ddr.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://lnd.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tuw.fktsv.cn

================================================================================
来源：http://ljy.uphjek.com

L. 网络请求
来源：http://jij.haohaochexian.top

================================================================================
来源：http://vfx.0kj1m.cn

[L01] 发送 GET 请求
来源：http://pid.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uwu.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xgi.yueranfly.top

JS:   await fetch(url)
来源：http://lrj.zdqjudy.top

TS:   await fetch(url)
来源：http://kot.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rua.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://hdi.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dll.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://suy.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://awq.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xtv.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hpj.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpg.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ybt.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wcw.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://olw.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://slb.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://scr.nwbrower.top

[L03] 设置自定义请求头
来源：http://faj.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://klz.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tmz.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cnj.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cmu.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dpl.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://puj.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bwx.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zhg.316326.xyz

[L04] 设置超时
来源：http://tnl.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://xyy.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yeg.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kuw.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vlk.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mjn.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ztl.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bnm.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wio.daxiang520.top

[L05] 上传文件（multipart）
来源：http://xtl.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mbr.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jfu.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ygz.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zkm.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zdc.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nxh.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxe.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fpw.xziqi.cn

[L06] 解析响应为 JSON
来源：http://hhe.hnxiangtu.top

Py:   resp.json()
来源：http://zzk.hammf.cn

PHP:  json_decode($body, true);
来源：http://jcn.pycfn.com

JS:   await resp.json()
来源：http://oqz.vqdsnc.cn

TS:   await resp.json()
来源：http://bys.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nfo.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ods.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://eac.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cbe.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://jwk.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ifa.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zoy.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://ajw.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://sfx.ctjpmb.com

Java: resp.statusCode()
来源：http://pxh.dianchejie.cn

Go:   resp.StatusCode
来源：http://xbw.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://tkr.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://ewa.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://bai.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mew.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://jgv.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eub.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://udg.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qsx.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hsq.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nhl.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rec.epnwcf.com

================================================================================
来源：http://wzo.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://fic.hcnkem.com

================================================================================
来源：http://tpe.yonumen.top

[M01] 读取命令行参数
来源：http://iyx.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://ijj.gzhubu.top

PHP:  $argv;  $argc;
来源：http://pzv.hammf.cn

JS:   process.argv.slice(2)
来源：http://jke.jianghu66.top

TS:   process.argv.slice(2)
来源：http://exx.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://gad.yuxming.cn

Go:   os.Args[1:]
来源：http://mkk.mhx1999.top

Ruby: ARGV
来源：http://vmw.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://hle.xziqi.cn

[M02] 读取环境变量
来源：http://jsu.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://ebh.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://khe.hfpthk.cn

JS:   process.env.HOME
来源：http://tzr.chenjidiqi.icu

TS:   process.env.HOME
来源：http://hic.tianlin.xyz

Java: System.getenv("HOME")
来源：http://oxs.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://usg.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://jxn.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mou.tarul.cn

[M03] 执行外部命令
来源：http://acw.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ejn.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ejs.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ito.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ofz.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yjw.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tyq.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://udp.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://jsq.jyoumei.cn

[M04] 获取当前工作目录
来源：http://xoz.hywenlv.cn

Py:   os.getcwd()
来源：http://veb.yonumen.top

PHP:  getcwd();
来源：http://byv.vqdsnc.cn

JS:   process.cwd()
来源：http://csg.snrcjt.cn

TS:   process.cwd()
来源：http://bfw.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ppm.cucudq.cn

Go:   os.Getwd()
来源：http://thk.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://eum.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://hlw.yangfankeji.com

[M05] 设置退出码
来源：http://lav.daria6918.cn

Py:   sys.exit(1)
来源：http://wus.yfazqb.com

PHP:  exit(1);
来源：http://ult.zhoulong.xyz

JS:   process.exit(1)
来源：http://tmo.haohaochexian.top

TS:   process.exit(1)
来源：http://mlo.ivvv.top

Java: System.exit(1)
来源：http://xzj.yonumen.top

Go:   os.Exit(1)
来源：http://cga.fanxiaobao.xyz

Ruby: exit 1
来源：http://qss.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zsn.tian-w.cn

[M06] 向标准错误输出
来源：http://lcj.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://qsc.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yhb.snrcjt.cn

JS:   console.error("err")
来源：http://sqy.c1oappe.top

TS:   console.error("err")
来源：http://qld.sweek.top

Java: System.err.println("err")
来源：http://ejt.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xin.zhongyouzk.top

Ruby: warn "err"
来源：http://lpw.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://vhn.jiagoushi.top

[M07] 判断是否为主入口
来源：http://mpt.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://kpr.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dbo.yueranfly.top

JS:   require.main === module
来源：http://dgk.sufxvd.cn

TS:   require.main === module
来源：http://jgs.zhixingplan.top

Java: public static void main(String[] args)
来源：http://lud.dashuyun.cn

Go:   func main()
来源：http://bxv.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oiz.xinyue.icu

C#:   static void Main(string[] args)
来源：http://emo.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://fia.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://nra.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://epm.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://sso.dianchejie.cn

TS:   process.platform;  process.version
来源：http://nqr.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xbh.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kgk.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xfr.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://aoc.vehdjk.com

================================================================================
来源：http://yap.andypj.xyz

N. 数据结构与算法
来源：http://dkp.sxryk.cn

================================================================================
来源：http://qqn.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://rzp.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fiq.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hns.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://apl.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysf.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pgn.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://dch.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://esz.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://qpq.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://afr.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://pyg.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drl.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yrd.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eat.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gnb.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://dcj.pengpengdd.cyou

Ruby: arr.sort
来源：http://apn.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bii.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://udi.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eds.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://mzw.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cef.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lcl.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ooy.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vqd.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zga.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://vno.bbcook.cn

[N04] 斐波那契数列
来源：http://tbv.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tww.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uvl.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aqo.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozo.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://odz.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yuf.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rum.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pii.tarul.cn

[N05] 最大公约数
来源：http://fne.sxryk.cn

Py:   math.gcd(a, b)
来源：http://idx.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gkd.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obc.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bhz.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zyz.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rgm.yj20258.top

Ruby: a.gcd(b)
来源：http://mnk.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eib.jiagoushi.top

[N06] 判断回文字符串
来源：http://lxk.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://nlq.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://sfv.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://bob.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://ohe.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wag.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://xjq.yj20258.top

Ruby: s == s.reverse
来源：http://pwy.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rzl.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://uop.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yhj.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hhu.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rdh.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://ytx.hammf.cn

Java: // 手写 HashMap
来源：http://bwb.yj202588.top

Go:   // 手写 map[int]int
来源：http://ija.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://xrw.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://wcn.birdmap.top

[N08] 生成全排列
来源：http://xod.havefunace.top

Py:   itertools.permutations(arr)
来源：http://ilc.xziqi.cn

PHP:  // 手写递归交换
来源：http://kup.sxryk.cn

JS:   // 手写回溯递归
来源：http://fdz.tianlin.xyz

TS:   // 手写回溯递归
来源：http://qfv.gzhubu.top

Java: // 手写回溯递归
来源：http://myp.zhixingplan.top

Go:   // 手写回溯递归
来源：http://upu.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://zph.jiagoushi.top

C#:   // 手写回溯递归
来源：http://auc.cashguo.top

[N09] 栈与队列
来源：http://jle.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ulx.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://enw.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://how.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghc.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swy.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nng.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gxx.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cmi.gzhubu.top

[N10] 链表节点定义
来源：http://nvw.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bky.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xsc.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wdj.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pdy.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://ihl.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://cpv.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fmx.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ehk.cheryme.top

[N11] 二叉树中序遍历
来源：http://pld.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zoe.gogol.net.cn

PHP:  // 手写递归函数
来源：http://cgz.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nlg.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ppq.andypj.xyz

Java: // 手写递归
来源：http://vve.shangyingyoupin.top

Go:   // 手写递归
来源：http://aac.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rnq.sufxvd.cn

C#:   // 手写递归
来源：http://hvh.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cam.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zms.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jvy.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jju.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bnx.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xmt.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pwq.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://adw.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nzt.gotoacloud.top

================================================================================
来源：http://ibq.gzhubu.top

O. 并发与异步
来源：http://tzz.dianchejie.cn

================================================================================
来源：http://jqa.quarkkingdee.top

[O01] 启动一个线程
来源：http://ico.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lzf.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bre.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dpi.xuetiantiany.cn

TS:   // 同 JS
来源：http://jhu.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://rtw.kuanghao11.cn

Go:   go f()
来源：http://wup.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://mgc.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://vzi.sysykeji.top

[O02] 使用线程池
来源：http://hov.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sid.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jpu.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://fnq.quarkkingdee.top


<!-- 参考信息 -->