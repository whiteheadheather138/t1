代发 wailian999

[K06] 解析 URL 查询串
来源：http://xrq.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://obc.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vzi.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pur.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kbf.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wxi.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://nzc.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tlv.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://trw.guowangkeji.top

[K07] 进制转换
来源：http://izx.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zpo.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nim.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fbt.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mix.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qwa.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xwh.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yke.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ace.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://ihq.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://qgb.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://val.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://jzb.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://lwm.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fxr.uphjek.com

Go:   encoding/gob
来源：http://enz.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://hat.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wic.c1oappe.top

================================================================================
来源：http://wyl.shuidangran.top

L. 网络请求
来源：http://iwu.kuanghao11.cn

================================================================================
来源：http://ixg.chenlongwang.top

[L01] 发送 GET 请求
来源：http://rhf.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://noa.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dxf.nwbrower.top

JS:   await fetch(url)
来源：http://jbo.dashuyun.cn

TS:   await fetch(url)
来源：http://otq.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gkx.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://vkx.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gzt.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://svb.yonumen.top

[L02] 发送 POST JSON
来源：http://wtn.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nmu.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fyp.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbh.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ddt.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jjg.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xgx.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://grx.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qod.tarul.cn

[L03] 设置自定义请求头
来源：http://twz.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uij.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://adl.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://svk.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tbm.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cpk.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xzc.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ztu.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ypw.hnqzz.top

[L04] 设置超时
来源：http://jvk.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://vlx.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nvb.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mxh.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hcg.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zsr.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ltr.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ekv.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://otw.ybcxt.top

[L05] 上传文件（multipart）
来源：http://vou.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://axb.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xlc.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lkw.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cpx.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vvs.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lld.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rbt.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://glr.yuxming.cn

[L06] 解析响应为 JSON
来源：http://akz.bbcook.cn

Py:   resp.json()
来源：http://vru.redwolf501.top

PHP:  json_decode($body, true);
来源：http://ufj.dianchejie.cn

JS:   await resp.json()
来源：http://bko.bbcook.cn

TS:   await resp.json()
来源：http://iod.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vxx.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sax.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://sgd.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lvx.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://nrj.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ffz.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dgi.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://hdu.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://kgm.ydzc1.top

Java: resp.statusCode()
来源：http://ohc.yj20258.top

Go:   resp.StatusCode
来源：http://per.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://pau.yongpay.top

C#:   (int)resp.StatusCode
来源：http://izq.svipenyu.cn

[L08] 并发请求多个地址
来源：http://qsp.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bka.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://bew.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bqu.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nql.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ryj.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bgo.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://syp.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tbu.52xcode.cn

================================================================================
来源：http://nic.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://srz.jinyuanbaomall.cn

================================================================================
来源：http://pgg.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://xzu.bjfxy.top

Py:   sys.argv[1:]
来源：http://wty.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://lxh.birdmap.top

JS:   process.argv.slice(2)
来源：http://url.yj20258.top

TS:   process.argv.slice(2)
来源：http://zhg.havefunace.top

Java: args 数组（main 方法参数）
来源：http://mar.pycfn.com

Go:   os.Args[1:]
来源：http://yio.feifeiyinyue.top

Ruby: ARGV
来源：http://ocv.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://xke.xinyue.icu

[M02] 读取环境变量
来源：http://rxi.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://ell.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ycp.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://fyj.yfazqb.com

TS:   process.env.HOME
来源：http://myc.yj20258.top

Java: System.getenv("HOME")
来源：http://jhp.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xps.ydzc1.top

Ruby: ENV["HOME"]
来源：http://ngb.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nhy.sufxvd.cn

[M03] 执行外部命令
来源：http://mnq.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://stv.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eof.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vii.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ngk.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://exu.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://iah.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://kuy.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://eyl.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://ybe.yj202588.top

Py:   os.getcwd()
来源：http://chu.cdnleiting.top

PHP:  getcwd();
来源：http://qsm.zhongyouzk.top

JS:   process.cwd()
来源：http://tcd.sweek.top

TS:   process.cwd()
来源：http://kak.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://kcb.yuanzhike.top

Go:   os.Getwd()
来源：http://qss.snrcjt.cn

Ruby: Dir.pwd
来源：http://wzr.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://lgb.hongshengwenyu.top

[M05] 设置退出码
来源：http://wzv.sjlbkw.cn

Py:   sys.exit(1)
来源：http://dsa.nanxuanxn.top

PHP:  exit(1);
来源：http://xvn.sweek.top

JS:   process.exit(1)
来源：http://ebr.svipenyu.cn

TS:   process.exit(1)
来源：http://phe.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://bcg.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://xgf.yueranfly.top

Ruby: exit 1
来源：http://mpa.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zua.ydjk.org.cn

[M06] 向标准错误输出
来源：http://ihu.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://gdy.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oqw.gotoacloud.top

JS:   console.error("err")
来源：http://oia.birdmap.top

TS:   console.error("err")
来源：http://fic.fzhhl.top

Java: System.err.println("err")
来源：http://drk.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://adq.uphjek.com

Ruby: warn "err"
来源：http://upn.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://kbq.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://rni.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://xar.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gif.9152youxi.cn

JS:   require.main === module
来源：http://apn.chenlongwang.top

TS:   require.main === module
来源：http://xuw.vehdjk.com

Java: public static void main(String[] args)
来源：http://lsj.nanxinkj.top

Go:   func main()
来源：http://snf.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ygn.bbcook.cn

C#:   static void Main(string[] args)
来源：http://wfc.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://pef.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://gjq.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://bjn.gogol.net.cn

JS:   process.platform;  process.version
来源：http://tay.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://jmf.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ofj.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wnm.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tob.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://tws.zhoulong.xyz

================================================================================
来源：http://mnw.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://otz.ydjk.org.cn

================================================================================
来源：http://hgx.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://dbs.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://ran.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ggh.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mwl.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pxi.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://knl.yj20258888.top

Go:   sort.SearchInts(arr, x)
来源：http://mqg.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gvg.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://zou.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://zgb.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://xrc.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mdi.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uvh.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://inl.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ayv.andypj.xyz

Go:   slices.Sort(arr)
来源：http://jpk.xylfe.cn

Ruby: arr.sort
来源：http://pfw.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fkq.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://xpz.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zzx.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://uvc.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gic.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jkg.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sqw.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dik.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hyt.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://rrs.hesvh.cn

[N04] 斐波那契数列
来源：http://dwr.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qsg.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fjk.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrr.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gou.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://duq.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tuz.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kcn.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ptf.hnxiangtu.top

[N05] 最大公约数
来源：http://iwn.xinyue.icu

Py:   math.gcd(a, b)
来源：http://big.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cjx.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yjo.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ina.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ldj.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zux.cashguo.top

Ruby: a.gcd(b)
来源：http://vtm.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://orq.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://kll.vehdjk.com

Py:   s == s[::-1]
来源：http://qdt.sweek.top

PHP:  $s === strrev($s);
来源：http://hss.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://ekt.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://hip.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://apc.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://nbz.dianchejie.cn

Ruby: s == s.reverse
来源：http://gxk.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://czu.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://vms.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdg.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uxz.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gik.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://plv.vehdjk.com

Java: // 手写 HashMap
来源：http://dip.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://xpn.hnqzz.top

Ruby: // 手写 Hash
来源：http://rgn.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://yss.daria6918.cn

[N08] 生成全排列
来源：http://rsa.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://cjp.cheryme.top

PHP:  // 手写递归交换
来源：http://eav.aizwys.cn

JS:   // 手写回溯递归
来源：http://jpx.cashguo.top

TS:   // 手写回溯递归
来源：http://ogq.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://wxi.daria6918.cn

Go:   // 手写回溯递归
来源：http://kid.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://gbi.xuanzx.com

C#:   // 手写回溯递归
来源：http://mxn.yfazqb.com

[N09] 栈与队列
来源：http://ttm.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dpw.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lsg.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ykq.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mgz.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wyr.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ral.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://upk.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jca.nwbrower.top

[N10] 链表节点定义
来源：http://rcy.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsd.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jor.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qev.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cyg.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://uxr.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://dhp.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gxi.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nvz.yj20258888.top

[N11] 二叉树中序遍历
来源：http://sip.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lce.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://uqe.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjr.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvr.c1oappe.top

Java: // 手写递归
来源：http://pai.ybcxt.top

Go:   // 手写递归
来源：http://adx.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ysb.epnwcf.com

C#:   // 手写递归
来源：http://ilh.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jmq.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wrs.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mgl.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epr.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqn.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kyv.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oad.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eit.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bce.shuidangran.top

================================================================================
来源：http://tns.fktsv.cn

O. 并发与异步
来源：http://tdq.yuanzhike.top

================================================================================
来源：http://iof.zhongyouzk.top

[O01] 启动一个线程
来源：http://bni.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tyt.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ubj.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tig.zycfv.cn

TS:   // 同 JS
来源：http://nff.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://zqt.ppjwa.cn

Go:   go f()
来源：http://gza.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://mfy.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://kmy.chenzaomai.com


<!-- 参考信息 -->