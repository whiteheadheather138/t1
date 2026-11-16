代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://bpt.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lmp.ivvv.top

[K04] 读取 JSON 文件
来源：http://iab.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yfd.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yhu.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oly.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://skv.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fyf.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://giv.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dax.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://phm.yj20258.top

[K05] 深拷贝对象
来源：http://heq.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://urz.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://skl.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://tqb.ivvv.top

TS:   structuredClone(obj)
来源：http://lgm.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aee.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zbe.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qiu.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hgk.yueranfly.top

[K06] 解析 URL 查询串
来源：http://iuv.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eqj.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lie.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsu.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://heo.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sdu.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mkp.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vzb.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wgn.9152youxi.cn

[K07] 进制转换
来源：http://jap.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tzc.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jfz.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gjr.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://llv.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dzy.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://owc.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jnu.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qhm.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://vtz.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://nwh.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bjv.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://jwu.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://wfz.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xot.52xcode.cn

Go:   encoding/gob
来源：http://szb.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://kow.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uyj.quarkkingdee.top

================================================================================
来源：http://kev.ywan-chungtsiang.top

L. 网络请求
来源：http://gld.vqdsnc.cn

================================================================================
来源：http://lkf.dashuyun.cn

[L01] 发送 GET 请求
来源：http://bco.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://riq.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fkx.meibo888.top

JS:   await fetch(url)
来源：http://hja.zhijiandao.cn

TS:   await fetch(url)
来源：http://taz.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxh.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://laj.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cwc.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nch.pycfn.com

[L02] 发送 POST JSON
来源：http://btu.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vhr.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lvl.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yqa.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zte.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dmi.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ajj.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ozf.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://neo.xylfe.cn

[L03] 设置自定义请求头
来源：http://zyv.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pjx.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rdn.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dcq.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xww.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gjr.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sin.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pbr.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ujj.fanxiaobao.xyz

[L04] 设置超时
来源：http://hhi.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://lii.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kas.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrg.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jbh.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wln.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eyl.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rxw.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vzp.nwbrower.top

[L05] 上传文件（multipart）
来源：http://fzs.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mir.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rxe.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rwd.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://atb.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ybd.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ejp.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rmf.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zqz.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://bpv.daria6918.cn

Py:   resp.json()
来源：http://zfw.sysykeji.top

PHP:  json_decode($body, true);
来源：http://wwo.redwolf501.top

JS:   await resp.json()
来源：http://pdp.jqgfzy.top

TS:   await resp.json()
来源：http://fyv.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pzz.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rka.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://hyz.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dqe.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://zta.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xma.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ncz.tanke756.top

JS:   resp.ok;  resp.status
来源：http://zio.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://luz.yanxiufei.cn

Java: resp.statusCode()
来源：http://isn.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://lhm.aizwys.cn

Ruby: resp.code.to_i
来源：http://wzo.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://hxr.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://yvn.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://inl.shanyushiyangtech.top

PHP:  curl_multi_init() 系列
来源：http://ibe.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://poo.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fnn.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ocd.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ksu.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jtp.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wyu.sysykeji.top

================================================================================
来源：http://jsr.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://tnv.jyoumei.cn

================================================================================
来源：http://vgx.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://sdt.c1oappe.top

Py:   sys.argv[1:]
来源：http://vfv.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://kme.jianghu66.top

JS:   process.argv.slice(2)
来源：http://mfb.yueranfly.top

TS:   process.argv.slice(2)
来源：http://qcl.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://ocg.cheryme.top

Go:   os.Args[1:]
来源：http://uxs.aizwys.cn

Ruby: ARGV
来源：http://vsa.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://nbg.bbcook.cn

[M02] 读取环境变量
来源：http://wsh.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://rmo.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://btp.chenjidiqi.icu

JS:   process.env.HOME
来源：http://xte.hnqzz.top

TS:   process.env.HOME
来源：http://mvj.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://ydp.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ojt.smart0.xyz

Ruby: ENV["HOME"]
来源：http://yvc.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://geg.andypj.xyz

[M03] 执行外部命令
来源：http://qne.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zju.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blg.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://yup.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://fmb.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://alv.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dgi.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://xut.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://fsz.bjfxy.top

[M04] 获取当前工作目录
来源：http://eer.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://nre.zdbjq.cn

PHP:  getcwd();
来源：http://epn.xinyue.icu

JS:   process.cwd()
来源：http://pqb.yj202588.top

TS:   process.cwd()
来源：http://yjh.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://rxy.hnqzz.top

Go:   os.Getwd()
来源：http://cvw.nanxuanxn.top

Ruby: Dir.pwd
来源：http://ynb.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://dap.gzhubu.top

[M05] 设置退出码
来源：http://vri.cucudq.cn

Py:   sys.exit(1)
来源：http://qzg.chenjidiqi.icu

PHP:  exit(1);
来源：http://etm.gotoacloud.top

JS:   process.exit(1)
来源：http://hub.tianlin.xyz

TS:   process.exit(1)
来源：http://klj.yvedp.cn

Java: System.exit(1)
来源：http://exj.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://usl.guannengcc.top

Ruby: exit 1
来源：http://zzv.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uhs.hesvh.cn

[M06] 向标准错误输出
来源：http://amu.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://zgu.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wom.hfpthk.cn

JS:   console.error("err")
来源：http://hcz.cdnleiting.top

TS:   console.error("err")
来源：http://aqy.sysykeji.top

Java: System.err.println("err")
来源：http://dat.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ipl.yj202588.top

Ruby: warn "err"
来源：http://dly.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://hde.aizwys.cn

[M07] 判断是否为主入口
来源：http://qel.yongpay.top

Py:   if __name__ == "__main__":
来源：http://wzr.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jnw.gzhubu.top

JS:   require.main === module
来源：http://pne.nwbrower.top

TS:   require.main === module
来源：http://fgm.dashuyun.cn

Java: public static void main(String[] args)
来源：http://ftm.316326.xyz

Go:   func main()
来源：http://ygd.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hry.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://jkc.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://cye.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://xwz.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://lsf.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://aos.yueranfly.top

TS:   process.platform;  process.version
来源：http://jek.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qgr.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sdd.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cju.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://zze.cashguo.top

================================================================================
来源：http://lko.gaohongyu789.top

N. 数据结构与算法
来源：http://vzv.316326.xyz

================================================================================
来源：http://tcc.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://gsr.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ruv.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ffc.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mrt.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://soh.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://smx.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://twa.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jyl.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uke.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://peq.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://apz.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tqe.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iqu.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://wsm.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yjw.mhx1999.top

Go:   slices.Sort(arr)
来源：http://gfp.epnwcf.com

Ruby: arr.sort
来源：http://nxz.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uhd.ivvv.top

[N03] 快速排序（分治示例）
来源：http://wyd.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cmi.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://ltw.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvf.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zyo.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lwh.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://urn.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://twv.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://okb.vqdsnc.cn

[N04] 斐波那契数列
来源：http://vxc.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pga.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gcx.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exb.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://giy.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dia.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kdz.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fix.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wwv.yuanzhike.top

[N05] 最大公约数
来源：http://xbd.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://vlk.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdy.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tvl.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bok.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qlc.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mdb.ydzc1.top

Ruby: a.gcd(b)
来源：http://yfr.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mhm.9152youxi.cn

[N06] 判断回文字符串
来源：http://bmy.dashuyun.cn

Py:   s == s[::-1]
来源：http://hjg.meibo888.top

PHP:  $s === strrev($s);
来源：http://hjt.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://upy.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://lbv.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lii.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://yys.svipenyu.cn

Ruby: s == s.reverse
来源：http://dwo.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hcw.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://mzi.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yrv.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://biq.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ema.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://pke.sjlbkw.cn

Java: // 手写 HashMap
来源：http://cfe.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://uug.ctjpmb.com

Ruby: // 手写 Hash
来源：http://rxp.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://hnk.cdnleiting.top

[N08] 生成全排列
来源：http://svu.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://frw.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://hfx.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://mbt.ehwqpu.com

TS:   // 手写回溯递归
来源：http://hjw.nwbrower.top

Java: // 手写回溯递归
来源：http://fgw.ctjpmb.com

Go:   // 手写回溯递归
来源：http://rwp.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://msh.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://jri.sysykeji.top

[N09] 栈与队列
来源：http://wwr.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vye.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jce.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hng.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yjt.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://upz.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fdf.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://twa.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://crr.ybcxt.top

[N10] 链表节点定义
来源：http://ahf.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://szx.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://puz.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ehs.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lty.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://ihs.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://btq.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gol.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://umb.redwolf501.top

[N11] 二叉树中序遍历
来源：http://nxh.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hzy.hesvh.cn

PHP:  // 手写递归函数
来源：http://zbw.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mcu.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rdf.birdmap.top

Java: // 手写递归
来源：http://hwl.shzxlz.cn

Go:   // 手写递归
来源：http://rpx.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lqu.ivvv.top

C#:   // 手写递归
来源：http://bap.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zzb.fehbvm.com


<!-- 参考信息 -->