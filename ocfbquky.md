代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://kmm.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://mcb.vehdjk.com

JS:   structuredClone(obj)
来源：http://plc.yangfankeji.com

TS:   structuredClone(obj)
来源：http://epe.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://sed.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wxd.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ehb.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mms.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://unr.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://owo.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iyu.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dkc.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eva.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xjz.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pfc.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qzg.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://owe.smart0.xyz

[K07] 进制转换
来源：http://sok.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://icb.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xap.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iuu.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ldp.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gxm.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ymu.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vbz.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cqb.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ecs.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://kvn.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://amd.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://zan.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://vou.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ycd.ybcxt.top

Go:   encoding/gob
来源：http://yma.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://aga.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sos.feifeiyinyue.top

================================================================================
来源：http://zfp.jianghu66.top

L. 网络请求
来源：http://api.fanxiaobao.xyz

================================================================================
来源：http://ggf.hfpthk.cn

[L01] 发送 GET 请求
来源：http://avg.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mpi.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://soe.sxryk.cn

JS:   await fetch(url)
来源：http://xuc.tian-w.cn

TS:   await fetch(url)
来源：http://wvq.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://odk.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://bpl.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eqn.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bwk.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://bmg.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pnw.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qot.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvk.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdl.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ibl.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xde.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dtr.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iyw.jinqigufen.top

[L03] 设置自定义请求头
来源：http://wfy.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pzr.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://daf.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvr.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wbl.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jti.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xjt.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://scy.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rbq.52xcode.cn

[L04] 设置超时
来源：http://ncl.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://gio.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rva.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lym.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://msj.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fus.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ncr.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fmt.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jbk.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://ybt.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rsb.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gna.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://unw.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://seh.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nvl.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yoi.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qlt.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vmp.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://atw.cdnleiting.top

Py:   resp.json()
来源：http://cni.cheryme.top

PHP:  json_decode($body, true);
来源：http://pmt.ctjpmb.com

JS:   await resp.json()
来源：http://abj.xuanzx.com

TS:   await resp.json()
来源：http://eyn.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://des.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wva.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://kfg.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ywj.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://uot.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tpb.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fae.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://bgt.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://gqz.yj20258888.top

Java: resp.statusCode()
来源：http://ayl.ivvv.top

Go:   resp.StatusCode
来源：http://qec.shuidangran.top

Ruby: resp.code.to_i
来源：http://wfr.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://hdj.snrcjt.cn

[L08] 并发请求多个地址
来源：http://fld.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://urg.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://ffe.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://num.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ghw.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://trd.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hyw.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://htx.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gsm.bbcook.cn

================================================================================
来源：http://thj.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://pon.cashguo.top

================================================================================
来源：http://vab.jiagoushi.top

[M01] 读取命令行参数
来源：http://lzj.sweek.top

Py:   sys.argv[1:]
来源：http://mdd.xylfe.cn

PHP:  $argv;  $argc;
来源：http://ocd.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://lfu.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://xdg.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://rex.pycfn.com

Go:   os.Args[1:]
来源：http://dad.hywenlv.cn

Ruby: ARGV
来源：http://xst.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://qfn.zhixingplan.top

[M02] 读取环境变量
来源：http://inl.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://qdd.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uzv.hnqzz.top

JS:   process.env.HOME
来源：http://dkf.c1oappe.top

TS:   process.env.HOME
来源：http://gwm.zycfv.cn

Java: System.getenv("HOME")
来源：http://dgw.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hnz.yj20258888.top

Ruby: ENV["HOME"]
来源：http://xdx.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fhd.yonumen.top

[M03] 执行外部命令
来源：http://szx.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wnz.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pkd.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bjk.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hwq.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://alu.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qsq.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://nre.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://vgd.gogol.net.cn

[M04] 获取当前工作目录
来源：http://hbs.zhixingplan.top

Py:   os.getcwd()
来源：http://pbt.ehwqpu.com

PHP:  getcwd();
来源：http://oez.andypj.xyz

JS:   process.cwd()
来源：http://frk.sufxvd.cn

TS:   process.cwd()
来源：http://ecy.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://mjx.hnqzz.top

Go:   os.Getwd()
来源：http://qlk.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://bnz.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://kya.zhiwuduotai.top

[M05] 设置退出码
来源：http://ahw.fzhhl.top

Py:   sys.exit(1)
来源：http://taf.zhixingplan.top

PHP:  exit(1);
来源：http://nwr.bbcook.cn

JS:   process.exit(1)
来源：http://rcn.smart0.xyz

TS:   process.exit(1)
来源：http://ivr.bjfxy.top

Java: System.exit(1)
来源：http://ccr.nwbrower.top

Go:   os.Exit(1)
来源：http://css.chenjidiqi.icu

Ruby: exit 1
来源：http://yyu.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uqf.hysaishi.cn

[M06] 向标准错误输出
来源：http://ptx.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://uaf.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bdz.andypj.xyz

JS:   console.error("err")
来源：http://kom.sjlbkw.cn

TS:   console.error("err")
来源：http://pma.sweek.top

Java: System.err.println("err")
来源：http://oao.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ati.ydzc1.top

Ruby: warn "err"
来源：http://gmv.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://dwr.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://vkb.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://sat.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ate.yonumen.top

JS:   require.main === module
来源：http://mjv.sjlbkw.cn

TS:   require.main === module
来源：http://idt.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://hsy.chenjidiqi.icu

Go:   func main()
来源：http://koh.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mma.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://hsq.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://zrh.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://jmc.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://yko.yj20258888.top

JS:   process.platform;  process.version
来源：http://myc.dianchejie.cn

TS:   process.platform;  process.version
来源：http://olz.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sip.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ryu.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vxt.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uda.shanyushiyangkeji.top

================================================================================
来源：http://ppm.sxryk.cn

N. 数据结构与算法
来源：http://dkw.snrcjt.cn

================================================================================
来源：http://zfy.yongpay.top

[N01] 二分查找（有序数组）
来源：http://qts.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://yki.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jri.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bjq.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ofx.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://itj.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://bsv.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://mpm.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://qmv.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://zht.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://xcd.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xcf.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dxi.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wjc.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://puc.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://kdz.quarkkingdee.top

Ruby: arr.sort
来源：http://kwt.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xst.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://lqp.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ajs.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://cii.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lmp.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkq.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ifp.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zxa.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kae.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://egx.gotoacloud.top

[N04] 斐波那契数列
来源：http://qno.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxg.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://djo.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdg.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nsj.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uej.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nid.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://njk.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mvi.cashguo.top

[N05] 最大公约数
来源：http://gch.sysykeji.top

Py:   math.gcd(a, b)
来源：http://iad.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wlg.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://trf.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bue.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://riq.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ifk.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://asq.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zxw.aibaodan.cn

[N06] 判断回文字符串
来源：http://byy.yueranfly.top

Py:   s == s[::-1]
来源：http://qsr.52xcode.cn

PHP:  $s === strrev($s);
来源：http://alk.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://ucr.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://bdm.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gxo.daxiang520.top

Go:   // 双指针从两端比较
来源：http://fni.zhongyouzk.top

Ruby: s == s.reverse
来源：http://cjy.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bxr.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://cyz.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sfk.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qnn.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://slo.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://buh.yuxming.cn

Java: // 手写 HashMap
来源：http://wno.andypj.xyz

Go:   // 手写 map[int]int
来源：http://tbd.yuanzhike.top

Ruby: // 手写 Hash
来源：http://vmo.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://dql.tian-w.cn

[N08] 生成全排列
来源：http://iun.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://rjw.mhx1999.top

PHP:  // 手写递归交换
来源：http://mah.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://bwl.daxiang520.top

TS:   // 手写回溯递归
来源：http://oma.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://nfb.yfazqb.com

Go:   // 手写回溯递归
来源：http://ycj.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://qip.316326.xyz

C#:   // 手写回溯递归
来源：http://dny.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://ogy.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qrt.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mox.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mpo.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dsj.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yol.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cyi.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lfj.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pky.0kj1m.cn

[N10] 链表节点定义
来源：http://iws.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xnv.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://cud.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gzi.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mzw.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://dlb.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://avv.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://uyb.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lht.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://mnt.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://put.wangdashe.top

PHP:  // 手写递归函数
来源：http://fcg.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://etb.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://abk.shangyingyoupin.top

Java: // 手写递归
来源：http://whd.jinghuilouyu.cn

Go:   // 手写递归
来源：http://qtc.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zqp.fengsongda.top

C#:   // 手写递归
来源：http://nhr.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qrn.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baw.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qeg.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mkj.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jqf.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nja.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xoj.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qid.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zjs.fktsv.cn

================================================================================
来源：http://xok.feifeiyinyue.top

O. 并发与异步
来源：http://fid.zhixingplan.top

================================================================================
来源：http://cap.hfpthk.cn

[O01] 启动一个线程
来源：http://wfj.chenzaomai.com


<!-- 参考信息 -->