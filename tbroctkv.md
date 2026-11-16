代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://nnm.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://wcm.tarul.cn

JS:   structuredClone(obj)
来源：http://wfq.iojbl.cn

TS:   structuredClone(obj)
来源：http://nmb.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eev.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jyk.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://plu.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://urc.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://txv.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dfb.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://plz.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://obu.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wlh.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yfg.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gke.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pma.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zfr.bbcook.cn

[K07] 进制转换
来源：http://qqg.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://orr.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://quh.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://odp.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fvq.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gxz.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://txg.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pcm.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://voa.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://lbx.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://kye.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://saw.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://vhx.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://qsr.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vhf.shuidangran.top

Go:   encoding/gob
来源：http://xpo.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://dyc.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bmg.dianchejie.cn

================================================================================
来源：http://wim.jiagoushi.top

L. 网络请求
来源：http://rwa.yfazqb.com

================================================================================
来源：http://vcu.daria6918.cn

[L01] 发送 GET 请求
来源：http://ylm.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kpu.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vjl.vehdjk.com

JS:   await fetch(url)
来源：http://stt.yj202588.top

TS:   await fetch(url)
来源：http://seu.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aar.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://pru.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pff.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjv.meibo888.top

[L02] 发送 POST JSON
来源：http://zoe.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hez.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://spd.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tma.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hny.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wfn.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://foo.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bwd.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jad.mhx1999.top

[L03] 设置自定义请求头
来源：http://zwz.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qmb.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bna.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://voe.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yna.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kax.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pcu.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lft.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://stx.hnqzz.top

[L04] 设置超时
来源：http://vdn.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://vsx.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cox.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpd.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ymg.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zvy.cheryme.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vqf.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qyh.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://agv.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://koh.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rnx.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rzc.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zqa.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cns.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qwi.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zpp.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://err.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zct.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://cnp.cqqwz.cn

Py:   resp.json()
来源：http://ycd.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://lzq.haohaochexian.top

JS:   await resp.json()
来源：http://qeo.ctjpmb.com

TS:   await resp.json()
来源：http://jvo.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zwt.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jzn.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ldo.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vez.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://adt.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xhc.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wcs.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://jvx.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://jsv.9152youxi.cn

Java: resp.statusCode()
来源：http://ceb.zhixingplan.top

Go:   resp.StatusCode
来源：http://vqv.yj20258888.top

Ruby: resp.code.to_i
来源：http://edp.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://fvw.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://kor.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wte.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://ujw.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgp.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pdd.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://elh.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tkf.gogol.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kql.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://efy.52xcode.cn

================================================================================
来源：http://bnx.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://mzf.yj20258.top

================================================================================
来源：http://mgo.dianchejie.cn

[M01] 读取命令行参数
来源：http://khv.fktsv.cn

Py:   sys.argv[1:]
来源：http://kcn.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://esv.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://tuw.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://hvl.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://yrh.xuanzx.com

Go:   os.Args[1:]
来源：http://ukz.shanyushiyangkeji.top

Ruby: ARGV
来源：http://txo.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://csh.iojbl.cn

[M02] 读取环境变量
来源：http://wsj.yj202588.top

Py:   os.environ.get("HOME")
来源：http://jbr.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://unx.nwbrower.top

JS:   process.env.HOME
来源：http://dra.chenzaomai.com

TS:   process.env.HOME
来源：http://cod.xylfe.cn

Java: System.getenv("HOME")
来源：http://zya.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iqw.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://lat.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lai.fehbvm.com

[M03] 执行外部命令
来源：http://pxn.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://crr.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vue.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://esw.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nei.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wtq.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fwa.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://rry.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://cwb.snrcjt.cn

[M04] 获取当前工作目录
来源：http://rro.svipenyu.cn

Py:   os.getcwd()
来源：http://dyo.meibo888.top

PHP:  getcwd();
来源：http://hzy.wangshuangyany.cn

JS:   process.cwd()
来源：http://vcf.0kj1m.cn

TS:   process.cwd()
来源：http://bkg.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://eum.hysaishi.cn

Go:   os.Getwd()
来源：http://xdp.hnxiangtu.top

Ruby: Dir.pwd
来源：http://rda.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://jow.zhengqikj.top

[M05] 设置退出码
来源：http://swj.yanxiufei.cn

Py:   sys.exit(1)
来源：http://che.cucudq.cn

PHP:  exit(1);
来源：http://czt.zhiwuduotai.top

JS:   process.exit(1)
来源：http://udf.52xcode.cn

TS:   process.exit(1)
来源：http://ixf.yonumen.top

Java: System.exit(1)
来源：http://gnn.jianghu66.top

Go:   os.Exit(1)
来源：http://hij.zhongyouzk.top

Ruby: exit 1
来源：http://ddg.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://znm.iojbl.cn

[M06] 向标准错误输出
来源：http://axl.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://pwy.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vtk.guowangkeji.top

JS:   console.error("err")
来源：http://ess.sxryk.cn

TS:   console.error("err")
来源：http://doq.nwbrower.top

Java: System.err.println("err")
来源：http://bse.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yzc.zdbjq.cn

Ruby: warn "err"
来源：http://rio.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://lcy.aizwys.cn

[M07] 判断是否为主入口
来源：http://ttv.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://ofl.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qih.feifeiyinyue.top

JS:   require.main === module
来源：http://sgf.yvedp.cn

TS:   require.main === module
来源：http://buj.yangfankeji.com

Java: public static void main(String[] args)
来源：http://esv.zhaomingkeji.xyz

Go:   func main()
来源：http://fvs.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ehh.sxryk.cn

C#:   static void Main(string[] args)
来源：http://jxl.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://jyx.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://zyq.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://mte.birdmap.top

JS:   process.platform;  process.version
来源：http://fen.aizwys.cn

TS:   process.platform;  process.version
来源：http://qjz.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jzo.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://gqj.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nqt.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xww.c1oappe.top

================================================================================
来源：http://lvk.jyoumei.cn

N. 数据结构与算法
来源：http://cfx.iojbl.cn

================================================================================
来源：http://ksr.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://nof.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://lgu.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zud.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxg.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vye.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://icu.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://zgb.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wnt.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://rjn.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ksd.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ucd.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vkw.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mpw.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://pes.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yob.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://ddi.fanxiaobao.xyz

Ruby: arr.sort
来源：http://fxb.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cfd.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://ffi.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xup.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://dbd.gzhubu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfz.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kbs.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iqe.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://axx.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kxy.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sxc.jyoumei.cn

[N04] 斐波那契数列
来源：http://uaf.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wsu.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ctc.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iuc.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bvq.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ern.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qzj.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qxa.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://row.zhoulong.xyz

[N05] 最大公约数
来源：http://uam.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://dje.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hnj.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxl.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iko.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://grt.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mjh.jinqigufen.top

Ruby: a.gcd(b)
来源：http://bps.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yqv.fzhhl.top

[N06] 判断回文字符串
来源：http://xga.jiagoushi.top

Py:   s == s[::-1]
来源：http://fik.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://znk.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://csi.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://ovf.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ymn.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://mtz.jiagoushi.top

Ruby: s == s.reverse
来源：http://ccf.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://jja.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://wsr.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://duv.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://omm.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vkp.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://emy.svipenyu.cn

Java: // 手写 HashMap
来源：http://vhu.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://hky.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://quk.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://vic.chenlongwang.top

[N08] 生成全排列
来源：http://jjd.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://woh.xylfe.cn

PHP:  // 手写递归交换
来源：http://rck.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://gwx.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://ksk.vehdjk.com

Java: // 手写回溯递归
来源：http://egl.tanke756.top

Go:   // 手写回溯递归
来源：http://kpr.yonumen.top

Ruby: arr.permutation.to_a
来源：http://yys.c1oappe.top

C#:   // 手写回溯递归
来源：http://nck.xuanzx.com

[N09] 栈与队列
来源：http://zsi.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dfq.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cht.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aoh.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jel.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rfw.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bbs.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wui.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qzu.aibaodan.cn

[N10] 链表节点定义
来源：http://lvo.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ubl.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dkh.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://syn.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tfk.yj20258.top

Java: class Node { int v; Node next; }
来源：http://qqp.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://gea.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zek.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wwi.mhx1999.top

[N11] 二叉树中序遍历
来源：http://yac.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lvi.cqqwz.cn

PHP:  // 手写递归函数
来源：http://qts.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://apn.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ret.fehbvm.com

Java: // 手写递归
来源：http://lkn.zhiwuduotai.top

Go:   // 手写递归
来源：http://eog.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wky.nwbrower.top

C#:   // 手写递归
来源：http://zsf.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hlm.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://axd.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dnf.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xpt.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfv.hysaishi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vqe.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tde.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vbv.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vuj.yueranfly.top

================================================================================
来源：http://gif.zhiwuduotai.top

O. 并发与异步
来源：http://slr.fktsv.cn

================================================================================
来源：http://jyw.jqgfzy.top

[O01] 启动一个线程
来源：http://cqj.fktsv.cn


<!-- 参考信息 -->