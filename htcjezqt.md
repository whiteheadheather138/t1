代发 wailian999

[K06] 解析 URL 查询串
来源：http://ebl.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xoz.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lam.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ooy.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://npr.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ecr.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jtu.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fxu.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sub.shanyushiyangtech.top

[K07] 进制转换
来源：http://omm.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://daq.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tme.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qdc.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mlz.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cdg.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xzk.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jjw.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yof.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://uij.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://eta.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bde.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://ztc.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://vrp.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://isn.andypj.xyz

Go:   encoding/gob
来源：http://gwl.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://fmz.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ypf.gaohongyu789.top

================================================================================
来源：http://isb.yonumen.top

L. 网络请求
来源：http://jos.guannengcc.top

================================================================================
来源：http://xfy.xuanzx.com

[L01] 发送 GET 请求
来源：http://rzg.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://diz.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ueb.yfazqb.com

JS:   await fetch(url)
来源：http://hdh.birdmap.top

TS:   await fetch(url)
来源：http://nxt.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ljr.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://cds.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kbp.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sjy.hysaishi.cn

[L02] 发送 POST JSON
来源：http://cmq.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bbx.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kii.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ogb.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qww.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://enc.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hox.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://njj.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uin.jianghu66.top

[L03] 设置自定义请求头
来源：http://rnx.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hmh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://des.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmj.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdw.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mat.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mbt.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ayc.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cxk.jiagoushi.top

[L04] 设置超时
来源：http://fkw.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://nxe.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://naf.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kst.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vow.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rcc.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://deh.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aoc.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nrx.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://zew.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oyd.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ugq.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nny.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ebo.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vfw.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jix.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gfj.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oil.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://mwa.ctjpmb.com

Py:   resp.json()
来源：http://txy.hammf.cn

PHP:  json_decode($body, true);
来源：http://edd.yj20258.top

JS:   await resp.json()
来源：http://whr.yangfankeji.com

TS:   await resp.json()
来源：http://tbn.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://glj.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://whb.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://cav.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rsp.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://uhd.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ceh.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wdy.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://hse.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://iob.birdmap.top

Java: resp.statusCode()
来源：http://tcy.jqgufenzy.top

Go:   resp.StatusCode
来源：http://nsf.gzhubu.top

Ruby: resp.code.to_i
来源：http://efa.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://upf.aizwys.cn

[L08] 并发请求多个地址
来源：http://uyc.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ybd.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://did.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dzu.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqs.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gdx.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://erf.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nts.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uyg.ydjk.org.cn

================================================================================
来源：http://lll.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://taf.shzxlz.cn

================================================================================
来源：http://tua.hesvh.cn

[M01] 读取命令行参数
来源：http://rlk.tanke756.top

Py:   sys.argv[1:]
来源：http://ajg.daxiang520.top

PHP:  $argv;  $argc;
来源：http://ofo.tarul.cn

JS:   process.argv.slice(2)
来源：http://trk.aizwys.cn

TS:   process.argv.slice(2)
来源：http://kxa.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://tdi.yangfankeji.com

Go:   os.Args[1:]
来源：http://sko.sufxvd.cn

Ruby: ARGV
来源：http://rpe.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://qkk.pengpengdd.cyou

[M02] 读取环境变量
来源：http://mts.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://hpm.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ufi.wangdashe.top

JS:   process.env.HOME
来源：http://bra.aizwys.cn

TS:   process.env.HOME
来源：http://mqb.c1oappe.top

Java: System.getenv("HOME")
来源：http://qra.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://csm.fengsongda.top

Ruby: ENV["HOME"]
来源：http://acd.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yxf.tian-w.cn

[M03] 执行外部命令
来源：http://csu.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mzq.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ktg.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cdc.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dzq.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://esc.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uzm.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cyv.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://tfi.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://iyw.zhiwuduotai.top

Py:   os.getcwd()
来源：http://phw.hywenlv.cn

PHP:  getcwd();
来源：http://asq.tianlin.xyz

JS:   process.cwd()
来源：http://soo.tarul.cn

TS:   process.cwd()
来源：http://xzi.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://oog.cucudq.cn

Go:   os.Getwd()
来源：http://qum.c1oappe.top

Ruby: Dir.pwd
来源：http://gjc.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://fbg.ybcxt.top

[M05] 设置退出码
来源：http://yxx.andypj.xyz

Py:   sys.exit(1)
来源：http://jma.hnxiangtu.top

PHP:  exit(1);
来源：http://sxx.fengsongda.top

JS:   process.exit(1)
来源：http://dps.xinyue.icu

TS:   process.exit(1)
来源：http://xwk.vqdsnc.cn

Java: System.exit(1)
来源：http://mov.jqgufenzy.top

Go:   os.Exit(1)
来源：http://hgl.jyoumei.cn

Ruby: exit 1
来源：http://pbp.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zqd.jianghu66.top

[M06] 向标准错误输出
来源：http://hyw.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://ozw.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://uzp.epnwcf.com

JS:   console.error("err")
来源：http://vrt.9152youxi.cn

TS:   console.error("err")
来源：http://ldo.hesvh.cn

Java: System.err.println("err")
来源：http://agd.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rfz.daxiang520.top

Ruby: warn "err"
来源：http://ele.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://msa.andypj.xyz

[M07] 判断是否为主入口
来源：http://znm.cheryme.top

Py:   if __name__ == "__main__":
来源：http://yif.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mjr.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://vie.quarkkingdee.top

TS:   require.main === module
来源：http://mja.zycfv.cn

Java: public static void main(String[] args)
来源：http://ukl.zdqjudy.top

Go:   func main()
来源：http://ety.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cyx.pycfn.com

C#:   static void Main(string[] args)
来源：http://fwy.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://nvo.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://kvt.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://eof.nanxinkj.top

JS:   process.platform;  process.version
来源：http://xmh.haohaochexian.top

TS:   process.platform;  process.version
来源：http://hiv.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://awf.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mdf.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zkf.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pag.bjfxy.top

================================================================================
来源：http://hjj.shuidangran.top

N. 数据结构与算法
来源：http://gdk.chenlongwang.top

================================================================================
来源：http://ddp.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://kwg.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://tar.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://whh.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcu.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dcc.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://izp.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://inw.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yer.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://qcp.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://kep.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ide.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vrg.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xwf.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gia.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oox.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://fdw.tarul.cn

Ruby: arr.sort
来源：http://nbk.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qgt.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://qzq.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lbs.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://bgt.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uug.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogo.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nux.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://phv.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bnp.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dum.iojbl.cn

[N04] 斐波那契数列
来源：http://pei.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vgs.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kvs.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cph.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pna.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sew.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hno.zhiwuduotai.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mlw.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://syn.sysykeji.top

[N05] 最大公约数
来源：http://ydm.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://szj.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aei.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxi.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwx.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hqx.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uex.dashuyun.cn

Ruby: a.gcd(b)
来源：http://ujm.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yfb.aibaodan.cn

[N06] 判断回文字符串
来源：http://yfh.nwbrower.top

Py:   s == s[::-1]
来源：http://ivq.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://ayy.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://wvh.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://vvt.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vpx.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://iim.yueranfly.top

Ruby: s == s.reverse
来源：http://tak.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://inv.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://kwi.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qnz.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xwj.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gky.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://opo.chenzaomai.com

Java: // 手写 HashMap
来源：http://bjp.fktsv.cn

Go:   // 手写 map[int]int
来源：http://jbf.sysykeji.top

Ruby: // 手写 Hash
来源：http://vmg.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ygq.zdbjq.cn

[N08] 生成全排列
来源：http://ccl.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://lhb.dashuyun.cn

PHP:  // 手写递归交换
来源：http://dcr.tianlin.xyz

JS:   // 手写回溯递归
来源：http://fij.jqgfzy.top

TS:   // 手写回溯递归
来源：http://mrx.zhijiandao.cn

Java: // 手写回溯递归
来源：http://afu.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://hav.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://try.snrcjt.cn

C#:   // 手写回溯递归
来源：http://hzj.guannengcc.top

[N09] 栈与队列
来源：http://izx.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oyi.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vim.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dlb.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vjj.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mli.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kzz.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pud.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bjm.daria6918.cn

[N10] 链表节点定义
来源：http://huk.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xnh.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zyq.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pyd.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ktp.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://edx.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://puy.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bgy.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ymb.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://zck.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://huz.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://wkz.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzs.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yvz.yj20258.top

Java: // 手写递归
来源：http://zkv.guannengcc.top

Go:   // 手写递归
来源：http://yrg.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aen.chenlongwang.top

C#:   // 手写递归
来源：http://nta.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ygg.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nim.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://knp.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://evb.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovs.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kfj.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xbp.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zff.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://npp.ybcxt.top

================================================================================
来源：http://ves.smart0.xyz

O. 并发与异步
来源：http://sbc.ydzc1.top

================================================================================
来源：http://dzh.chenjidiqi.icu

[O01] 启动一个线程
来源：http://wzt.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://exs.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ksx.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kzs.havefunace.top

TS:   // 同 JS
来源：http://rsq.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://wgi.yj20258888.top

Go:   go f()
来源：http://ftj.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://ped.yj20258888.top

C#:   Task.Run(() => F());
来源：http://fqs.ywan-chungtsiang.top


<!-- 参考信息 -->