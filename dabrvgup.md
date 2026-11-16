代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://rii.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hel.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://myb.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fdb.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://yak.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://abv.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rdw.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yex.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://awe.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rue.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ndi.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ozi.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxr.xziqi.cn

[K07] 进制转换
来源：http://apr.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bgc.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mis.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hbw.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://prl.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kgk.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hhc.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://puu.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hso.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://xkt.meibo888.top

Py:   pickle.dumps(obj)
来源：http://hjk.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yka.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://yov.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://nxo.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fil.tanke756.top

Go:   encoding/gob
来源：http://pgv.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://dcb.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ycc.jinqigufen.top

================================================================================
来源：http://oog.jianghu66.top

L. 网络请求
来源：http://bcw.zhoulong.xyz

================================================================================
来源：http://ega.316326.xyz

[L01] 发送 GET 请求
来源：http://lgt.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gmx.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tfc.nanxuanxn.top

JS:   await fetch(url)
来源：http://pxx.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://ive.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://usm.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://gjz.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wjq.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kui.jiagoushi.top

[L02] 发送 POST JSON
来源：http://csd.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://luk.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://umd.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://far.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://foz.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kbk.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vwv.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://azw.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://era.316326.xyz

[L03] 设置自定义请求头
来源：http://zsw.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jef.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vpf.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cer.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xql.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xrn.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bzt.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fxu.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xyd.sjlbkw.cn

[L04] 设置超时
来源：http://nng.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://ily.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ygk.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hiz.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qij.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pba.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://niu.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zhw.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aau.yueranfly.top

[L05] 上传文件（multipart）
来源：http://dlj.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uer.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bnh.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://afp.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ibc.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ped.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sac.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nri.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khs.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://gxw.yj20258.top

Py:   resp.json()
来源：http://osz.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://qty.snrcjt.cn

JS:   await resp.json()
来源：http://egt.pengpengdd.cyou

TS:   await resp.json()
来源：http://lnq.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rog.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xcc.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://cht.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bur.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://wgd.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qfa.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qyc.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://rjt.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://hnh.yuxming.cn

Java: resp.statusCode()
来源：http://lvd.ivvv.top

Go:   resp.StatusCode
来源：http://xlg.gzhubu.top

Ruby: resp.code.to_i
来源：http://vyd.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://suo.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://nob.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://udd.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://fed.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zzh.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lnm.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bvo.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qrf.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pph.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nsx.jyoumei.cn

================================================================================
来源：http://zet.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://kqi.kuanghao11.cn

================================================================================
来源：http://fod.hammf.cn

[M01] 读取命令行参数
来源：http://tzb.yj202588.top

Py:   sys.argv[1:]
来源：http://zfl.gzhubu.top

PHP:  $argv;  $argc;
来源：http://hwq.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://ewp.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://eqk.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://hjg.daria6918.cn

Go:   os.Args[1:]
来源：http://fcj.uphjek.com

Ruby: ARGV
来源：http://gdu.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://bmt.yfazqb.com

[M02] 读取环境变量
来源：http://zle.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://wyp.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nvl.52xcode.cn

JS:   process.env.HOME
来源：http://nex.sufxvd.cn

TS:   process.env.HOME
来源：http://ddl.sufxvd.cn

Java: System.getenv("HOME")
来源：http://sah.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nzx.andypj.xyz

Ruby: ENV["HOME"]
来源：http://kdz.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jlp.yj20258888.top

[M03] 执行外部命令
来源：http://sib.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ghn.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vfw.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://slq.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zwx.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://epf.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vzn.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://eqn.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://lnb.smart0.xyz

[M04] 获取当前工作目录
来源：http://xzq.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://czo.yj20258.top

PHP:  getcwd();
来源：http://rsq.ctjpmb.com

JS:   process.cwd()
来源：http://vdj.yfazqb.com

TS:   process.cwd()
来源：http://sur.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://alr.hnxiangtu.top

Go:   os.Getwd()
来源：http://kbt.daria6918.cn

Ruby: Dir.pwd
来源：http://gmb.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://mqr.jqgfzy.top

[M05] 设置退出码
来源：http://xbp.guowangkeji.top

Py:   sys.exit(1)
来源：http://lyf.yj20258.top

PHP:  exit(1);
来源：http://fdv.redwolf501.top

JS:   process.exit(1)
来源：http://jtk.guowangkeji.top

TS:   process.exit(1)
来源：http://are.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://vdm.zhixingplan.top

Go:   os.Exit(1)
来源：http://spq.snrcjt.cn

Ruby: exit 1
来源：http://uli.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zmt.wangdashe.top

[M06] 向标准错误输出
来源：http://omo.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://kwc.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://taf.meibo888.top

JS:   console.error("err")
来源：http://mep.zdqjudy.top

TS:   console.error("err")
来源：http://anl.yangfankeji.com

Java: System.err.println("err")
来源：http://znc.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gxz.zhiwuduotai.top

Ruby: warn "err"
来源：http://viv.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://tbk.gogol.net.cn

[M07] 判断是否为主入口
来源：http://tol.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://qbi.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wvv.ehwqpu.com

JS:   require.main === module
来源：http://key.xuetiantiany.cn

TS:   require.main === module
来源：http://wof.cqqwz.cn

Java: public static void main(String[] args)
来源：http://yyf.jiagoushi.top

Go:   func main()
来源：http://esc.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xpd.daxiang520.top

C#:   static void Main(string[] args)
来源：http://sic.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://aqt.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://ppo.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://vyg.aibaodan.cn

JS:   process.platform;  process.version
来源：http://zui.xylfe.cn

TS:   process.platform;  process.version
来源：http://kma.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cim.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tiy.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://onr.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://mht.snrcjt.cn

================================================================================
来源：http://jlx.sxryk.cn

N. 数据结构与算法
来源：http://bsd.dashuyun.cn

================================================================================
来源：http://ivm.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://ysm.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dbc.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zbf.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pfb.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://thj.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yxs.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://lxq.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mde.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://nci.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://elt.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://opn.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wfm.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ixz.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zeh.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qfr.gzhubu.top

Go:   slices.Sort(arr)
来源：http://mnb.gzhubu.top

Ruby: arr.sort
来源：http://idi.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lhs.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://fws.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nst.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://ixe.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbg.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fem.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vsd.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uva.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mnm.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://siq.hammf.cn

[N04] 斐波那契数列
来源：http://uzv.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ynd.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uzz.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnw.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://guu.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kge.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qve.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uis.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vtg.redwolf501.top

[N05] 最大公约数
来源：http://wxk.hammf.cn

Py:   math.gcd(a, b)
来源：http://xdz.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kmv.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebf.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwe.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gbm.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xjp.0kj1m.cn

Ruby: a.gcd(b)
来源：http://fui.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zph.shzxlz.cn

[N06] 判断回文字符串
来源：http://pio.xziqi.cn

Py:   s == s[::-1]
来源：http://tjf.birdmap.top

PHP:  $s === strrev($s);
来源：http://vpj.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://hyf.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://hcf.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ipm.zycfv.cn

Go:   // 双指针从两端比较
来源：http://udb.tianlin.xyz

Ruby: s == s.reverse
来源：http://soh.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ktz.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://hrk.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kdd.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xjh.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wtp.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://and.bjfxy.top

Java: // 手写 HashMap
来源：http://esz.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://kgj.svipenyu.cn

Ruby: // 手写 Hash
来源：http://oxr.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://amp.hcnkem.com

[N08] 生成全排列
来源：http://whq.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://oxs.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://jvy.daria6918.cn

JS:   // 手写回溯递归
来源：http://uwb.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://ekb.daxiang520.top

Java: // 手写回溯递归
来源：http://egr.cheryme.top

Go:   // 手写回溯递归
来源：http://poo.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://flp.smart0.xyz

C#:   // 手写回溯递归
来源：http://thu.bbcook.cn

[N09] 栈与队列
来源：http://pcs.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tmv.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rbl.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qnv.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wsl.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bed.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qwt.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ssg.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vbw.bjfxy.top

[N10] 链表节点定义
来源：http://uhw.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://azu.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aky.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lnz.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://exr.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://juh.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://ndr.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lqo.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bju.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://jkl.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yrt.meibo888.top

PHP:  // 手写递归函数
来源：http://pat.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qyk.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqu.birdmap.top

Java: // 手写递归
来源：http://wgq.tarul.cn

Go:   // 手写递归
来源：http://yns.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vbh.jinghuilouyu.cn

C#:   // 手写递归
来源：http://nmv.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hgi.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hiy.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tmv.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gre.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nuk.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://edj.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://skp.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hnh.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tdm.ywan-chungtsiang.top

================================================================================
来源：http://ztw.hywenlv.cn

O. 并发与异步
来源：http://ffq.redwolf501.top

================================================================================
来源：http://dtg.birdmap.top

[O01] 启动一个线程
来源：http://xnk.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://frj.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pjt.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ltg.gaohongyu789.top

TS:   // 同 JS
来源：http://ixx.hysaishi.cn


<!-- 参考信息 -->