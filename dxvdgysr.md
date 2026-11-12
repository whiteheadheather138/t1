代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://tpu.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ofv.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://hpd.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rrx.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jqj.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kbw.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uty.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fbr.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zrr.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uep.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wjw.yuanzhike.top

[K05] 深拷贝对象
来源：http://gfb.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://veq.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://ewz.9152youxi.cn

JS:   structuredClone(obj)
来源：http://kyt.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://jie.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nwm.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mcs.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://krx.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uzq.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://diu.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ajp.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xot.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dys.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ezz.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ndg.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cui.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mmr.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tcw.fzhhl.top

[K07] 进制转换
来源：http://zce.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lqe.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ppj.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rvu.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mbl.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iwr.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lgz.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pky.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wch.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://oen.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://vly.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kjg.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://lpd.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://fdy.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fhp.jinqigufen.top

Go:   encoding/gob
来源：http://mkx.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://opg.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lag.hongshengwenyu.top

================================================================================
来源：http://vcq.yj20258.top

L. 网络请求
来源：http://dgd.guowangkeji.top

================================================================================
来源：http://myn.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://jee.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yus.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jtg.iojbl.cn

JS:   await fetch(url)
来源：http://igg.gaohongyu789.top

TS:   await fetch(url)
来源：http://oxd.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bqu.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://rgd.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ris.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tgd.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://mjz.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://iqx.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lce.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://itj.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bxv.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xnv.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://caa.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xmk.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ode.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://apb.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qnr.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nay.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwl.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ogq.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ybf.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ery.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kfm.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rlj.bbcook.cn

[L04] 设置超时
来源：http://fyj.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://hta.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rzx.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jsi.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxf.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cut.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rdv.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yub.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ktv.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://qmp.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tjb.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vfo.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ich.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vxq.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qgw.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hnu.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ltr.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bjq.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://lei.ybcxt.top

Py:   resp.json()
来源：http://ewx.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://qwe.9152youxi.cn

JS:   await resp.json()
来源：http://eeb.tian-w.cn

TS:   await resp.json()
来源：http://zzw.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sci.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xdk.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://rdz.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wuo.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://qcc.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rlx.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tle.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://ouq.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://onm.ehwqpu.com

Java: resp.statusCode()
来源：http://vid.ivvv.top

Go:   resp.StatusCode
来源：http://wud.cheryme.top

Ruby: resp.code.to_i
来源：http://bnm.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://vwt.yj20258888.top

[L08] 并发请求多个地址
来源：http://izs.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dwj.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://itp.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxf.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gxx.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://txp.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://laq.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bay.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://akv.yvedp.cn

================================================================================
来源：http://xhs.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://mlm.yuanzhike.top

================================================================================
来源：http://uxw.gotoacloud.top

[M01] 读取命令行参数
来源：http://vmh.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://ivl.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://rri.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://nbr.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://xuo.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://dbz.fengsongda.top

Go:   os.Args[1:]
来源：http://hpw.jinghuilouyu.cn

Ruby: ARGV
来源：http://cow.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://gwx.zhixingplan.top

[M02] 读取环境变量
来源：http://sek.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://zhp.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xea.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://cpw.kuanghao11.cn

TS:   process.env.HOME
来源：http://nam.svipenyu.cn

Java: System.getenv("HOME")
来源：http://zht.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sqn.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://qtj.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qdz.bjfxy.top

[M03] 执行外部命令
来源：http://wwh.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://raf.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ffg.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pcb.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://thf.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oyl.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sxm.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tnx.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://hya.wangdashe.top

[M04] 获取当前工作目录
来源：http://kuo.aibaodan.cn

Py:   os.getcwd()
来源：http://lye.316326.xyz

PHP:  getcwd();
来源：http://vxn.pycfn.com

JS:   process.cwd()
来源：http://gig.fktsv.cn

TS:   process.cwd()
来源：http://fdf.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://oiu.bjfxy.top

Go:   os.Getwd()
来源：http://con.uphjek.com

Ruby: Dir.pwd
来源：http://uid.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rhy.yonumen.top

[M05] 设置退出码
来源：http://dkb.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://rot.zhixingplan.top

PHP:  exit(1);
来源：http://muw.0kj1m.cn

JS:   process.exit(1)
来源：http://mpf.pengpengdd.cyou

TS:   process.exit(1)
来源：http://yie.52xcode.cn

Java: System.exit(1)
来源：http://bbt.ctjpmb.com

Go:   os.Exit(1)
来源：http://ywd.9152youxi.cn

Ruby: exit 1
来源：http://hpv.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tcr.ivvv.top

[M06] 向标准错误输出
来源：http://nht.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://ezr.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://arh.xziqi.cn

JS:   console.error("err")
来源：http://mst.cqqwz.cn

TS:   console.error("err")
来源：http://ktz.jqgufenzy.top

Java: System.err.println("err")
来源：http://ryo.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://onz.ctjpmb.com

Ruby: warn "err"
来源：http://crl.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://kon.xziqi.cn

[M07] 判断是否为主入口
来源：http://cad.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://ruy.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xau.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://uer.smart0.xyz

TS:   require.main === module
来源：http://ysm.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://dnj.fzhhl.top

Go:   func main()
来源：http://frt.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zwx.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://pst.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://sni.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://ebh.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://uee.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://yfo.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://xfl.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sdh.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ykv.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zcr.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hiu.nwbrower.top

================================================================================
来源：http://qma.jyoumei.cn

N. 数据结构与算法
来源：http://dbb.birdmap.top

================================================================================
来源：http://lid.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://xtc.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eir.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qtn.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://elv.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://awt.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://fmy.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xcl.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://iid.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://wfo.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://fip.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fcr.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xpm.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bjm.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uui.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://ewy.cdnleiting.top

Ruby: arr.sort
来源：http://hvv.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xrq.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://uoe.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uda.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://cdo.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hqm.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://grr.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bhv.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://clx.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cck.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://vrj.gaohongyu789.top

[N04] 斐波那契数列
来源：http://bbm.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://usq.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mfr.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tch.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eab.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tsk.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uhq.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tfe.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://izh.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://adf.hcnkem.com

Py:   math.gcd(a, b)
来源：http://wnw.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mcn.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gdx.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dzv.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sdi.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vuk.fktsv.cn

Ruby: a.gcd(b)
来源：http://wcg.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kdd.jinqigufen.top

[N06] 判断回文字符串
来源：http://jbw.316326.xyz

Py:   s == s[::-1]
来源：http://sdz.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://orq.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://bja.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://wec.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bcv.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://zey.hesvh.cn

Ruby: s == s.reverse
来源：http://fbv.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://enj.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://yay.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cmd.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yhj.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://jeo.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://vde.jqgfzy.top

Java: // 手写 HashMap
来源：http://wnb.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://byt.yongpay.top

Ruby: // 手写 Hash
来源：http://sdl.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://epl.fzhhl.top

[N08] 生成全排列
来源：http://rqq.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://wia.xylfe.cn

PHP:  // 手写递归交换
来源：http://zok.jinqigufen.top

JS:   // 手写回溯递归
来源：http://sxd.redwolf501.top

TS:   // 手写回溯递归
来源：http://geh.guowangkeji.top

Java: // 手写回溯递归
来源：http://kjy.ydzc1.top

Go:   // 手写回溯递归
来源：http://lqx.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://nox.xziqi.cn

C#:   // 手写回溯递归
来源：http://fvq.quarkkingdee.top

[N09] 栈与队列
来源：http://ior.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eyt.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tvy.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nvc.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fru.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eoa.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wrf.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ggm.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hmr.gotoacloud.top

[N10] 链表节点定义
来源：http://cyq.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ixv.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lif.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ruk.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cjv.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://oat.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://per.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ucl.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ghd.xziqi.cn

[N11] 二叉树中序遍历
来源：http://zwr.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://afh.bjfxy.top

PHP:  // 手写递归函数
来源：http://akj.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rqg.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zwi.ydjk.org.cn

Java: // 手写递归
来源：http://lfs.yanxiufei.cn

Go:   // 手写递归
来源：http://gdb.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yxt.jinqigfzy.top

C#:   // 手写递归
来源：http://puo.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xtc.nanxinkj.top


<!-- 参考信息 -->