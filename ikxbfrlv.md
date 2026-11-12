代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vep.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gbp.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fer.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rmr.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uyg.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ydo.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ctx.0kj1m.cn

[K05] 深拷贝对象
来源：http://trf.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://pfq.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://rop.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://kfx.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://vlw.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zyq.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vqo.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zks.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tfw.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://yhg.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uew.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cht.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gbo.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xxg.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pth.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mpc.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jbg.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rgv.vehdjk.com

[K07] 进制转换
来源：http://tii.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mro.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rhw.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cbf.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://esw.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iok.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qvf.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://abg.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rtu.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://awl.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://bwq.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://rij.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://rdj.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://plt.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://win.ivvv.top

Go:   encoding/gob
来源：http://bft.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://gok.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqp.jqgfzy.top

================================================================================
来源：http://udr.uphjek.com

L. 网络请求
来源：http://neh.hfpthk.cn

================================================================================
来源：http://orh.hfpthk.cn

[L01] 发送 GET 请求
来源：http://goy.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cyr.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tnn.guowangkeji.top

JS:   await fetch(url)
来源：http://hbl.fengsongda.top

TS:   await fetch(url)
来源：http://ngw.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://euc.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://pyc.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aju.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cjb.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://wle.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://ymi.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qjn.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ftu.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsf.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qmv.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zhj.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ylh.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://byl.daxiang520.top

[L03] 设置自定义请求头
来源：http://cuy.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://duk.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uxa.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ifo.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ole.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yek.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oym.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lny.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pcp.shuidangran.top

[L04] 设置超时
来源：http://rti.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://mwh.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ecl.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ebt.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iqv.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://crd.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sht.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hre.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uvs.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://guy.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yjz.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lzf.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zzw.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cmv.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://liw.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mcm.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zbu.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mnp.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://pvj.pengpengdd.cyou

Py:   resp.json()
来源：http://vcm.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://ydf.yuxming.cn

JS:   await resp.json()
来源：http://umh.jiagoushi.top

TS:   await resp.json()
来源：http://pqa.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wwp.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ixa.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://swu.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://huk.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://jxu.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://imh.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oku.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://abt.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://jyg.dashuyun.cn

Java: resp.statusCode()
来源：http://zbe.vqdsnc.cn

Go:   resp.StatusCode
来源：http://qaw.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://oiz.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://csw.daria6918.cn

[L08] 并发请求多个地址
来源：http://say.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vuh.sweek.top

PHP:  curl_multi_init() 系列
来源：http://xup.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ekc.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tpq.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gdi.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pil.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rwl.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ojd.redwolf501.top

================================================================================
来源：http://zrq.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://mzy.haohaochexian.top

================================================================================
来源：http://ycf.nwbrower.top

[M01] 读取命令行参数
来源：http://eks.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://jfn.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://hqu.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://meg.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://vpp.havefunace.top

Java: args 数组（main 方法参数）
来源：http://rqy.xinyue.icu

Go:   os.Args[1:]
来源：http://kmo.bbcook.cn

Ruby: ARGV
来源：http://ulh.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://qey.svipenyu.cn

[M02] 读取环境变量
来源：http://ppv.pycfn.com

Py:   os.environ.get("HOME")
来源：http://bds.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iir.chenlongwang.top

JS:   process.env.HOME
来源：http://xwy.ctjpmb.com

TS:   process.env.HOME
来源：http://xsf.uphjek.com

Java: System.getenv("HOME")
来源：http://ooz.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lvb.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://iun.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vlv.nanxuanxn.top

[M03] 执行外部命令
来源：http://lxb.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vec.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ozg.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rrm.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zkl.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zpp.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vfm.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yqi.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://wnn.bjfxy.top

[M04] 获取当前工作目录
来源：http://egq.hnqzz.top

Py:   os.getcwd()
来源：http://wsg.yvedp.cn

PHP:  getcwd();
来源：http://epn.cucudq.cn

JS:   process.cwd()
来源：http://rmf.chenjidiqi.icu

TS:   process.cwd()
来源：http://jeg.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ove.daxiang520.top

Go:   os.Getwd()
来源：http://ylk.yj20258.top

Ruby: Dir.pwd
来源：http://bel.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://ggp.sjlbkw.cn

[M05] 设置退出码
来源：http://qkj.yj20258888.top

Py:   sys.exit(1)
来源：http://cbt.kuanghao11.cn

PHP:  exit(1);
来源：http://cck.0kj1m.cn

JS:   process.exit(1)
来源：http://etg.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://pec.zdqjudy.top

Java: System.exit(1)
来源：http://ucb.epnwcf.com

Go:   os.Exit(1)
来源：http://egp.hysaishi.cn

Ruby: exit 1
来源：http://dtx.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ygx.havefunace.top

[M06] 向标准错误输出
来源：http://iop.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://axd.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nte.sweek.top

JS:   console.error("err")
来源：http://ufs.chenjidiqi.icu

TS:   console.error("err")
来源：http://msr.fzhhl.top

Java: System.err.println("err")
来源：http://weq.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dli.hywenlv.cn

Ruby: warn "err"
来源：http://tdh.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://pso.xylfe.cn

[M07] 判断是否为主入口
来源：http://zdn.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://qiu.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gdf.ehwqpu.com

JS:   require.main === module
来源：http://lef.vqdsnc.cn

TS:   require.main === module
来源：http://qcy.zhengqikj.top

Java: public static void main(String[] args)
来源：http://ter.smart0.xyz

Go:   func main()
来源：http://org.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bzr.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://asv.ivvv.top

[M08] 获取系统与运行时信息
来源：http://fsx.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://hmq.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://vvh.c1oappe.top

JS:   process.platform;  process.version
来源：http://inn.chenlongwang.top

TS:   process.platform;  process.version
来源：http://jnf.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yos.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hft.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rdd.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://did.dashuyun.cn

================================================================================
来源：http://nsl.birdmap.top

N. 数据结构与算法
来源：http://tmj.redwolf501.top

================================================================================
来源：http://ibd.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://rce.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vnz.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ywr.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://guy.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ryp.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://swc.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://yol.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xew.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://aio.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://smf.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://vfo.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://frm.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://syo.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ona.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jbv.fehbvm.com

Go:   slices.Sort(arr)
来源：http://qyl.yanxiufei.cn

Ruby: arr.sort
来源：http://rag.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kdt.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://yvf.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dgr.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://wsx.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxz.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wtd.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://upc.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jii.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dtl.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://svm.316326.xyz

[N04] 斐波那契数列
来源：http://awp.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vcn.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hms.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xjn.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jch.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vns.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://usc.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nfv.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eij.zhongyouzk.top

[N05] 最大公约数
来源：http://cas.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://qzx.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://srn.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvq.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgk.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fos.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cca.svipenyu.cn

Ruby: a.gcd(b)
来源：http://ndg.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ftx.zhongyouzk.top

[N06] 判断回文字符串
来源：http://ffq.yangfankeji.com

Py:   s == s[::-1]
来源：http://jyu.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://paf.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://hrx.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://nxa.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uzk.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://jea.hcnkem.com

Ruby: s == s.reverse
来源：http://fqy.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hwf.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://xkn.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cnl.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://raf.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ngx.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://msz.haohaochexian.top

Java: // 手写 HashMap
来源：http://rws.vehdjk.com

Go:   // 手写 map[int]int
来源：http://lue.hfpthk.cn

Ruby: // 手写 Hash
来源：http://jba.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jti.havefunace.top

[N08] 生成全排列
来源：http://xwr.meibo888.top

Py:   itertools.permutations(arr)
来源：http://hqk.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://hnb.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://fml.0kj1m.cn

TS:   // 手写回溯递归
来源：http://ril.yvedp.cn

Java: // 手写回溯递归
来源：http://glx.hysaishi.cn

Go:   // 手写回溯递归
来源：http://aec.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://uoe.yongpay.top

C#:   // 手写回溯递归
来源：http://wxf.fktsv.cn

[N09] 栈与队列
来源：http://jnv.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rkz.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bsc.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fvf.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vjn.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fxt.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hoo.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ynt.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yic.yangfankeji.com

[N10] 链表节点定义
来源：http://eqd.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dmc.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lkf.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ucu.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qlh.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://rha.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://xtv.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gwy.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://hgz.daxiang520.top

[N11] 二叉树中序遍历
来源：http://biw.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kue.sufxvd.cn

PHP:  // 手写递归函数
来源：http://mdv.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eqd.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovd.hfpthk.cn

Java: // 手写递归
来源：http://bfj.zdbjq.cn

Go:   // 手写递归
来源：http://kcn.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://udd.daxiang520.top

C#:   // 手写递归
来源：http://lng.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pyq.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://awn.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xkf.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tqx.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xyo.tanke756.top


<!-- 参考信息 -->