代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://uoj.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://peu.nwbrower.top

[K04] 读取 JSON 文件
来源：http://vcz.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rjb.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ygz.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jge.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ufe.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cmr.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mdf.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yzz.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nfm.guowangkeji.top

[K05] 深拷贝对象
来源：http://yfw.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://niw.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://xww.52xcode.cn

JS:   structuredClone(obj)
来源：http://bdi.andypj.xyz

TS:   structuredClone(obj)
来源：http://yvd.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fwn.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cgu.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://its.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xdp.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://jrx.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://npl.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bwj.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ezw.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://clu.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rtv.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lod.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rdb.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pil.yanxiufei.cn

[K07] 进制转换
来源：http://doy.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sjq.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tsk.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://scd.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qrg.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nlq.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://frj.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zlp.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rka.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://kyf.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://uog.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pgm.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://low.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://myi.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mgc.epnwcf.com

Go:   encoding/gob
来源：http://erm.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://lgi.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hdg.zdbjq.cn

================================================================================
来源：http://jvj.meibo888.top

L. 网络请求
来源：http://chp.snrcjt.cn

================================================================================
来源：http://eaa.daria6918.cn

[L01] 发送 GET 请求
来源：http://ogt.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ymy.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cli.uphjek.com

JS:   await fetch(url)
来源：http://qwr.sysykeji.top

TS:   await fetch(url)
来源：http://pzf.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://box.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://tea.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ocy.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://znn.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://hap.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://vwk.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cxw.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://apo.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sez.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ajl.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lxy.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zza.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pbu.0kj1m.cn

[L03] 设置自定义请求头
来源：http://nkg.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aki.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://azd.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vmv.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eym.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rtb.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yom.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uav.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://idz.nanxuanxn.top

[L04] 设置超时
来源：http://dqg.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://pcj.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pbl.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tid.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sql.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ejl.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://agu.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xir.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://itr.xylfe.cn

[L05] 上传文件（multipart）
来源：http://gyj.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://atg.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://brx.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zwv.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jsy.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rgb.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iqn.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jny.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mrr.birdmap.top

[L06] 解析响应为 JSON
来源：http://ojr.andypj.xyz

Py:   resp.json()
来源：http://qbb.tanke756.top

PHP:  json_decode($body, true);
来源：http://cyi.svipenyu.cn

JS:   await resp.json()
来源：http://ata.hnqzz.top

TS:   await resp.json()
来源：http://kbz.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xaq.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://msa.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://nan.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cvm.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://saq.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ktm.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://odr.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://xms.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://byf.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://fzc.xziqi.cn

Go:   resp.StatusCode
来源：http://imn.0kj1m.cn

Ruby: resp.code.to_i
来源：http://gmh.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://vif.bjfxy.top

[L08] 并发请求多个地址
来源：http://xkt.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zhz.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://jbo.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewu.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idm.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tig.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kvf.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iho.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fat.fengsongda.top

================================================================================
来源：http://itz.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://rky.snrcjt.cn

================================================================================
来源：http://tgi.hesvh.cn

[M01] 读取命令行参数
来源：http://lnm.redwolf501.top

Py:   sys.argv[1:]
来源：http://lip.pycfn.com

PHP:  $argv;  $argc;
来源：http://xbw.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://gbx.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://nte.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://ymg.ehwqpu.com

Go:   os.Args[1:]
来源：http://cov.uphjek.com

Ruby: ARGV
来源：http://rfx.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://ofk.yanxiufei.cn

[M02] 读取环境变量
来源：http://gia.hammf.cn

Py:   os.environ.get("HOME")
来源：http://otb.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aie.zhoulong.xyz

JS:   process.env.HOME
来源：http://spy.dianchejie.cn

TS:   process.env.HOME
来源：http://lmk.hysaishi.cn

Java: System.getenv("HOME")
来源：http://ltq.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wum.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://awg.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jnb.gogol.net.cn

[M03] 执行外部命令
来源：http://znr.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zei.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xrd.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://xyp.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tps.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dcc.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://par.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://nkf.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://fwc.hcnkem.com

[M04] 获取当前工作目录
来源：http://gue.shzxlz.cn

Py:   os.getcwd()
来源：http://cgw.hcnkem.com

PHP:  getcwd();
来源：http://ciy.fzhhl.top

JS:   process.cwd()
来源：http://xue.cashguo.top

TS:   process.cwd()
来源：http://ejk.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://pik.ydjk.org.cn

Go:   os.Getwd()
来源：http://slv.yj202588.top

Ruby: Dir.pwd
来源：http://biz.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nbs.vqdsnc.cn

[M05] 设置退出码
来源：http://hap.jqgufenzy.top

Py:   sys.exit(1)
来源：http://tgy.xylfe.cn

PHP:  exit(1);
来源：http://xwe.ehwqpu.com

JS:   process.exit(1)
来源：http://kut.shuidangran.top

TS:   process.exit(1)
来源：http://hhy.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://eyf.quarkkingdee.top

Go:   os.Exit(1)
来源：http://dmu.hywenlv.cn

Ruby: exit 1
来源：http://orc.zhiwuduotai.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oyr.epnwcf.com

[M06] 向标准错误输出
来源：http://woo.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://jzb.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://urn.dianchejie.cn

JS:   console.error("err")
来源：http://khq.shanyushiyangtech.top

TS:   console.error("err")
来源：http://zgb.jinqigufen.top

Java: System.err.println("err")
来源：http://asj.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fae.sjlbkw.cn

Ruby: warn "err"
来源：http://knk.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://llk.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://jwd.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://qsn.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mim.jinqigufen.top

JS:   require.main === module
来源：http://iyp.cashguo.top

TS:   require.main === module
来源：http://quf.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://gvo.vqdsnc.cn

Go:   func main()
来源：http://zza.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hwh.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://tcp.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://dgb.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://jkg.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://kae.shuidangran.top

JS:   process.platform;  process.version
来源：http://fhg.gzhubu.top

TS:   process.platform;  process.version
来源：http://dhj.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nnx.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://erk.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dss.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yzn.0kj1m.cn

================================================================================
来源：http://ths.redwolf501.top

N. 数据结构与算法
来源：http://snc.yvedp.cn

================================================================================
来源：http://qqc.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://lah.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://uqy.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cvf.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://myn.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://akx.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://opk.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://pfd.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://esm.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ili.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://laz.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://otj.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oqn.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qlo.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zkf.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ebg.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://yid.cucudq.cn

Ruby: arr.sort
来源：http://kde.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wwy.tarul.cn

[N03] 快速排序（分治示例）
来源：http://hch.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jsr.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://fmr.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lys.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngw.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jwn.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ryo.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jvt.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zji.gotoacloud.top

[N04] 斐波那契数列
来源：http://sge.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ida.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tsa.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfg.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yqy.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rsf.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hgo.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://twb.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ypq.jqgufenzy.top

[N05] 最大公约数
来源：http://tsz.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://aac.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbm.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sty.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fiz.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vsa.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pya.cdnleiting.top

Ruby: a.gcd(b)
来源：http://siv.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ayl.birdmap.top

[N06] 判断回文字符串
来源：http://ltm.yongpay.top

Py:   s == s[::-1]
来源：http://egc.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://pes.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://veq.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://ldf.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qnh.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://jlo.havefunace.top

Ruby: s == s.reverse
来源：http://ktd.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ubo.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://gtd.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://frj.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gcl.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://esb.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://chl.sysykeji.top

Java: // 手写 HashMap
来源：http://dpo.yongpay.top

Go:   // 手写 map[int]int
来源：http://npj.fengsongda.top

Ruby: // 手写 Hash
来源：http://oqn.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://oir.chenlongwang.top

[N08] 生成全排列
来源：http://pgz.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://iei.shzxlz.cn

PHP:  // 手写递归交换
来源：http://pqb.9152youxi.cn

JS:   // 手写回溯递归
来源：http://vkq.daxiang520.top

TS:   // 手写回溯递归
来源：http://yxh.hywenlv.cn

Java: // 手写回溯递归
来源：http://eqg.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://nea.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://xvj.iojbl.cn

C#:   // 手写回溯递归
来源：http://ygx.52xcode.cn

[N09] 栈与队列
来源：http://gnj.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://igw.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pnb.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vqp.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zha.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hvj.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mtx.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vbr.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cgu.guannengcc.top

[N10] 链表节点定义
来源：http://kpi.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eex.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gku.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uhp.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://veq.sweek.top

Java: class Node { int v; Node next; }
来源：http://hrm.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ezf.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hdu.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jqm.fengsongda.top

[N11] 二叉树中序遍历
来源：http://cfz.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bcf.gzhubu.top

PHP:  // 手写递归函数
来源：http://tlt.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wig.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zgc.iojbl.cn

Java: // 手写递归
来源：http://krq.tian-w.cn

Go:   // 手写递归
来源：http://chj.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pmu.yueranfly.top

C#:   // 手写递归
来源：http://ans.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bno.fzhhl.top


<!-- 参考信息 -->