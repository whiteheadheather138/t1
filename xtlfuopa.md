代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://izt.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://blu.bjfxy.top

JS:   structuredClone(obj)
来源：http://whf.zycfv.cn

TS:   structuredClone(obj)
来源：http://gaj.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cyg.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://htp.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sou.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cps.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://pdl.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vvz.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://skb.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pij.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjh.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ils.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zwh.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rbv.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ppr.nanxuanxn.top

[K07] 进制转换
来源：http://plj.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://und.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://spo.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxh.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cfn.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hav.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kfd.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bya.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vlr.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://dlh.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://umr.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vvd.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://stk.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://zkz.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cnl.quarkkingdee.top

Go:   encoding/gob
来源：http://npn.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://vtf.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fid.redwolf501.top

================================================================================
来源：http://gxw.tanke756.top

L. 网络请求
来源：http://ows.quarkkingdee.top

================================================================================
来源：http://iuk.hesvh.cn

[L01] 发送 GET 请求
来源：http://tpg.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tiu.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iom.fengsongda.top

JS:   await fetch(url)
来源：http://lof.sufxvd.cn

TS:   await fetch(url)
来源：http://qvr.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tmw.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://mqn.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dif.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zvy.gogol.net.cn

[L02] 发送 POST JSON
来源：http://vux.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://xvf.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vng.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ott.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jfv.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://quy.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://urq.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vun.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tvu.c1oappe.top

[L03] 设置自定义请求头
来源：http://hho.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ulu.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qkt.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cfc.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://csq.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mzb.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lsq.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pnz.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dom.ydzc1.top

[L04] 设置超时
来源：http://xkb.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://ghc.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://udf.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tig.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iaf.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hug.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hcv.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://obp.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sag.xuanzx.com

[L05] 上传文件（multipart）
来源：http://srj.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fjx.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bhb.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pcg.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://grp.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fje.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqh.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wjb.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oyv.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://hwe.zhengqikj.top

Py:   resp.json()
来源：http://pdr.hesvh.cn

PHP:  json_decode($body, true);
来源：http://pmk.nwbrower.top

JS:   await resp.json()
来源：http://wym.meibo888.top

TS:   await resp.json()
来源：http://ebr.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lff.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zwc.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://rjb.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gxd.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://ehh.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://whh.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rsd.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://cvr.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://vyj.fehbvm.com

Java: resp.statusCode()
来源：http://ujg.daxiang520.top

Go:   resp.StatusCode
来源：http://xjh.zycfv.cn

Ruby: resp.code.to_i
来源：http://coh.ivvv.top

C#:   (int)resp.StatusCode
来源：http://wsz.jianghu66.top

[L08] 并发请求多个地址
来源：http://ujc.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wvh.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://meh.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhs.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lqk.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eoz.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vhb.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jpx.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kzz.xziqi.cn

================================================================================
来源：http://aak.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://zko.nwbrower.top

================================================================================
来源：http://ypg.hcnkem.com

[M01] 读取命令行参数
来源：http://cng.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://tnj.ybcxt.top

PHP:  $argv;  $argc;
来源：http://yid.tanke756.top

JS:   process.argv.slice(2)
来源：http://htk.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://vvy.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://gbk.ydjk.org.cn

Go:   os.Args[1:]
来源：http://pkl.chenzaomai.com

Ruby: ARGV
来源：http://tbb.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://xcw.jyoumei.cn

[M02] 读取环境变量
来源：http://hmm.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://ilw.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://slw.cqqwz.cn

JS:   process.env.HOME
来源：http://bdg.yj20258888.top

TS:   process.env.HOME
来源：http://wlt.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://mhs.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dat.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://rtd.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tqu.havefunace.top

[M03] 执行外部命令
来源：http://nek.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kpl.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bjg.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kjv.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jzi.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bvj.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://unv.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pjx.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://gms.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://oak.gzhubu.top

Py:   os.getcwd()
来源：http://ret.fktsv.cn

PHP:  getcwd();
来源：http://fgo.zhoulong.xyz

JS:   process.cwd()
来源：http://xkv.yuanzhike.top

TS:   process.cwd()
来源：http://fvi.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://sfe.hysaishi.cn

Go:   os.Getwd()
来源：http://foo.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://tkr.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://wld.nanxuanxn.top

[M05] 设置退出码
来源：http://wjv.chenzaomai.com

Py:   sys.exit(1)
来源：http://bch.316326.xyz

PHP:  exit(1);
来源：http://toe.yuxming.cn

JS:   process.exit(1)
来源：http://usc.yj202588.top

TS:   process.exit(1)
来源：http://sxf.fehbvm.com

Java: System.exit(1)
来源：http://jfk.52xcode.cn

Go:   os.Exit(1)
来源：http://beu.ybcxt.top

Ruby: exit 1
来源：http://skn.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ovu.yangfankeji.com

[M06] 向标准错误输出
来源：http://gqu.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://tlb.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://fpq.bjfxy.top

JS:   console.error("err")
来源：http://zau.mhx1999.top

TS:   console.error("err")
来源：http://yhs.bbcook.cn

Java: System.err.println("err")
来源：http://kvb.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dby.sysykeji.top

Ruby: warn "err"
来源：http://jhs.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://otk.jianghu66.top

[M07] 判断是否为主入口
来源：http://goc.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://gvc.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://edn.sufxvd.cn

JS:   require.main === module
来源：http://emw.c1oappe.top

TS:   require.main === module
来源：http://jch.mhx1999.top

Java: public static void main(String[] args)
来源：http://dnn.zhengqikj.top

Go:   func main()
来源：http://gzs.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mtf.hcnkem.com

C#:   static void Main(string[] args)
来源：http://yjh.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://cfh.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://mwd.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://jal.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://quq.gotoacloud.top

TS:   process.platform;  process.version
来源：http://kws.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aat.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://fgj.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ajv.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zui.tanke756.top

================================================================================
来源：http://fmw.sxryk.cn

N. 数据结构与算法
来源：http://hox.c1oappe.top

================================================================================
来源：http://ina.yj20258.top

[N01] 二分查找（有序数组）
来源：http://rzh.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tgs.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dms.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kix.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://prr.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://aih.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://skj.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kfr.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://pqf.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://xmw.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://svv.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bnd.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pwn.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pgb.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uwn.fktsv.cn

Go:   slices.Sort(arr)
来源：http://tmw.dashuyun.cn

Ruby: arr.sort
来源：http://zwh.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dkl.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://dhk.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ukn.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://tee.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lsh.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mty.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lxk.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mwj.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aze.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wdr.bjfxy.top

[N04] 斐波那契数列
来源：http://emz.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jqs.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aja.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oon.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpb.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tpe.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cht.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rjo.ydjk.org.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ztz.hesvh.cn

[N05] 最大公约数
来源：http://fhs.daria6918.cn

Py:   math.gcd(a, b)
来源：http://jjg.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yxg.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://haw.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qwl.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sdx.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hlz.ydzc1.top

Ruby: a.gcd(b)
来源：http://mmi.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gro.yj20258888.top

[N06] 判断回文字符串
来源：http://mag.ybcxt.top

Py:   s == s[::-1]
来源：http://gnn.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://rtk.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://cqk.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://pqn.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ddb.daxiang520.top

Go:   // 双指针从两端比较
来源：http://eqq.nwbrower.top

Ruby: s == s.reverse
来源：http://smg.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gkm.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://fqt.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jje.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vqh.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ygn.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://kxw.fktsv.cn

Java: // 手写 HashMap
来源：http://zzd.jianghu66.top

Go:   // 手写 map[int]int
来源：http://esb.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://bbd.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ecp.kuanghao11.cn

[N08] 生成全排列
来源：http://hsz.cheryme.top

Py:   itertools.permutations(arr)
来源：http://jkc.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://she.jqgfzy.top

JS:   // 手写回溯递归
来源：http://ccs.nanxinkj.top

TS:   // 手写回溯递归
来源：http://zax.chenzaomai.com

Java: // 手写回溯递归
来源：http://duz.yj20258.top

Go:   // 手写回溯递归
来源：http://bqy.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://vux.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://ocj.shzxlz.cn

[N09] 栈与队列
来源：http://pvd.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cgs.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zdf.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dik.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tqc.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sze.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oel.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uqi.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://klt.meibo888.top

[N10] 链表节点定义
来源：http://rne.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ptf.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://pja.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uke.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ruy.tanke756.top

Java: class Node { int v; Node next; }
来源：http://zsv.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://lfz.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mun.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://npc.yfazqb.com

[N11] 二叉树中序遍历
来源：http://bpr.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xrc.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://utk.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izg.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xrl.gzhubu.top

Java: // 手写递归
来源：http://nxm.cashguo.top

Go:   // 手写递归
来源：http://zci.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ihj.hongshengwenyu.top

C#:   // 手写递归
来源：http://bdr.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://drz.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lty.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nwt.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xln.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ccu.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lwv.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lyu.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fry.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ouq.ywan-chungtsiang.top

================================================================================
来源：http://fzb.feifeiyinyue.top

O. 并发与异步
来源：http://uxc.316326.xyz

================================================================================
来源：http://plx.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://pir.tianlin.xyz


<!-- 参考信息 -->