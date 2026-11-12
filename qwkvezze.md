代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://rdp.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zcr.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gaf.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://paj.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://wwx.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://asf.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hnw.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kkd.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzj.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cmu.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://qcp.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aex.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jgd.sweek.top

[K07] 进制转换
来源：http://wbh.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dep.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nwf.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eqs.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uxd.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bso.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hlg.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ewo.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://szf.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://uzq.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://pdw.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rzr.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://qxh.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://cig.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://frd.yj20258.top

Go:   encoding/gob
来源：http://sna.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://iuj.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vll.dashuyun.cn

================================================================================
来源：http://ikr.nanxinkj.top

L. 网络请求
来源：http://ypt.zycfv.cn

================================================================================
来源：http://zhv.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://spn.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gha.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fxd.xuetiantiany.cn

JS:   await fetch(url)
来源：http://fan.chenlongwang.top

TS:   await fetch(url)
来源：http://pwl.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nrn.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://uup.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dqk.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sah.pycfn.com

[L02] 发送 POST JSON
来源：http://ykh.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://tpy.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://udh.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tcj.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bhm.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://msf.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jdm.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nbc.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ofb.svipenyu.cn

[L03] 设置自定义请求头
来源：http://aso.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kss.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wkw.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xqv.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pqt.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kyk.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rut.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zht.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fod.birdmap.top

[L04] 设置超时
来源：http://fkv.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://qpf.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aci.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpn.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ote.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zcs.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ixp.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://urr.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kwf.cashguo.top

[L05] 上传文件（multipart）
来源：http://bou.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bxv.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nss.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dac.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zdq.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wlq.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bwo.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xlm.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aoo.hcnkem.com

[L06] 解析响应为 JSON
来源：http://phx.sjlbkw.cn

Py:   resp.json()
来源：http://jvw.ivvv.top

PHP:  json_decode($body, true);
来源：http://sce.gotoacloud.top

JS:   await resp.json()
来源：http://ezr.fktsv.cn

TS:   await resp.json()
来源：http://mth.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://roj.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://stk.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://cnd.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mgk.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://vby.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fmf.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://axp.pycfn.com

JS:   resp.ok;  resp.status
来源：http://gij.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://pgu.yangfankeji.com

Java: resp.statusCode()
来源：http://tes.chenlongwang.top

Go:   resp.StatusCode
来源：http://iit.redwolf501.top

Ruby: resp.code.to_i
来源：http://hpt.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://xry.havefunace.top

[L08] 并发请求多个地址
来源：http://geb.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ddk.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://pgt.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qzs.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pde.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ygk.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://unq.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wpg.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pzs.52xcode.cn

================================================================================
来源：http://pnd.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://sek.xziqi.cn

================================================================================
来源：http://vfv.snrcjt.cn

[M01] 读取命令行参数
来源：http://ihc.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://zxz.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://jae.redwolf501.top

JS:   process.argv.slice(2)
来源：http://wpi.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://pce.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://bpt.zdbjq.cn

Go:   os.Args[1:]
来源：http://trq.yangfankeji.com

Ruby: ARGV
来源：http://usu.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://lez.haohaochexian.top

[M02] 读取环境变量
来源：http://bmf.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://qzb.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xpz.cqqwz.cn

JS:   process.env.HOME
来源：http://dho.redwolf501.top

TS:   process.env.HOME
来源：http://upy.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://iym.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ntf.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://lqk.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://btt.birdmap.top

[M03] 执行外部命令
来源：http://ylh.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mqb.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://czl.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mrp.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jzf.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://joa.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rbz.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rrh.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://zsv.uphjek.com

[M04] 获取当前工作目录
来源：http://fsy.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://aow.fehbvm.com

PHP:  getcwd();
来源：http://bcb.shzxlz.cn

JS:   process.cwd()
来源：http://pmu.quarkkingdee.top

TS:   process.cwd()
来源：http://yey.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://lqz.tian-w.cn

Go:   os.Getwd()
来源：http://fgi.vqdsnc.cn

Ruby: Dir.pwd
来源：http://xbh.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://qzi.cucudq.cn

[M05] 设置退出码
来源：http://mqm.meibo888.top

Py:   sys.exit(1)
来源：http://lla.nwbrower.top

PHP:  exit(1);
来源：http://cgg.epnwcf.com

JS:   process.exit(1)
来源：http://svr.sweek.top

TS:   process.exit(1)
来源：http://ghy.ybcxt.top

Java: System.exit(1)
来源：http://brz.hcnkem.com

Go:   os.Exit(1)
来源：http://ojg.jinqigufen.top

Ruby: exit 1
来源：http://ysm.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pao.zhixingplan.top

[M06] 向标准错误输出
来源：http://pjw.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://rxh.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iww.feifeiyinyue.top

JS:   console.error("err")
来源：http://igr.yj202588.top

TS:   console.error("err")
来源：http://cql.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://xps.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pxd.bjfxy.top

Ruby: warn "err"
来源：http://rzf.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://ywk.yonumen.top

[M07] 判断是否为主入口
来源：http://ikg.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://qdp.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dtt.pengpengdd.cyou

JS:   require.main === module
来源：http://vrm.shuidangran.top

TS:   require.main === module
来源：http://fhu.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://kfl.ybcxt.top

Go:   func main()
来源：http://vaf.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cnb.ybcxt.top

C#:   static void Main(string[] args)
来源：http://fzm.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://sse.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://qhm.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://sqh.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://rzr.fzhhl.top

TS:   process.platform;  process.version
来源：http://fli.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kgn.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tyn.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://khj.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ves.yfazqb.com

================================================================================
来源：http://fea.dianchejie.cn

N. 数据结构与算法
来源：http://hqk.ivvv.top

================================================================================
来源：http://ihy.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://zem.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://pse.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://glr.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ppb.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cuq.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://kmp.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://ugh.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ouj.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://vom.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://eqc.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://vhz.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mvl.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dih.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lqf.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qya.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://caf.9152youxi.cn

Ruby: arr.sort
来源：http://qdo.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bkm.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://auu.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jmr.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://xuc.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xhv.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zbl.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mky.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://miv.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lkq.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://gsx.hammf.cn

[N04] 斐波那契数列
来源：http://xye.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pfr.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qjx.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qer.jianghu66.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://owv.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hvi.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dwe.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bop.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nia.aizwys.cn

[N05] 最大公约数
来源：http://zyg.mhx1999.top

Py:   math.gcd(a, b)
来源：http://gpo.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jkt.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://joq.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrc.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wmq.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://azg.iojbl.cn

Ruby: a.gcd(b)
来源：http://pia.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hcz.jyoumei.cn

[N06] 判断回文字符串
来源：http://gyf.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://kav.316326.xyz

PHP:  $s === strrev($s);
来源：http://ksl.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://gct.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://bsl.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://djn.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://knd.xinyue.icu

Ruby: s == s.reverse
来源：http://xdk.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://itj.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://gbm.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ior.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bgj.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hkj.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://jzp.jinqigfzy.top

Java: // 手写 HashMap
来源：http://eei.guannengcc.top

Go:   // 手写 map[int]int
来源：http://edd.cucudq.cn

Ruby: // 手写 Hash
来源：http://lnx.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ioq.316326.xyz

[N08] 生成全排列
来源：http://xbf.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://jiu.jiagoushi.top

PHP:  // 手写递归交换
来源：http://qpk.cqqwz.cn

JS:   // 手写回溯递归
来源：http://uqs.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://fjk.havefunace.top

Java: // 手写回溯递归
来源：http://hce.shuidangran.top

Go:   // 手写回溯递归
来源：http://hfu.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://zci.uphjek.com

C#:   // 手写回溯递归
来源：http://qnu.yuanzhike.top

[N09] 栈与队列
来源：http://cxb.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hax.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tgt.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cfm.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jcr.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ftj.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ymp.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://udp.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mdr.nanxinkj.top

[N10] 链表节点定义
来源：http://sjl.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hvo.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lyb.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofm.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bml.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://kjj.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://fvr.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hgj.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://nmm.jianghu66.top

[N11] 二叉树中序遍历
来源：http://kmm.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wsa.hammf.cn

PHP:  // 手写递归函数
来源：http://uwy.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ywy.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrj.cheryme.top

Java: // 手写递归
来源：http://scx.yvedp.cn

Go:   // 手写递归
来源：http://jas.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tan.zdqjudy.top

C#:   // 手写递归
来源：http://tcy.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xxl.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zfd.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bnn.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://feb.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uai.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ecd.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mmn.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wzp.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rsc.dashuyun.cn

================================================================================
来源：http://zya.vqdsnc.cn

O. 并发与异步
来源：http://wre.ctjpmb.com

================================================================================
来源：http://swu.sxryk.cn

[O01] 启动一个线程
来源：http://bek.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://grq.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://let.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jrb.smart0.xyz

TS:   // 同 JS
来源：http://hrg.bjfxy.top


<!-- 参考信息 -->