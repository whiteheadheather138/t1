代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ead.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://oyw.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dvo.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bjs.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nhe.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hjl.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jee.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kgf.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://zfk.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vjp.smart0.xyz

[K04] 读取 JSON 文件
来源：http://dnc.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fnw.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xej.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpr.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://apc.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://myt.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fdv.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://tjn.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kve.vehdjk.com

[K05] 深拷贝对象
来源：http://duu.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://boh.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://cce.gogol.net.cn

JS:   structuredClone(obj)
来源：http://nzj.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://rrd.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uks.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vxz.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ood.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dzk.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://mql.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fmc.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sfk.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yic.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://byq.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bvq.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rno.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bux.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iig.jlsjyb.cn

[K07] 进制转换
来源：http://wcc.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ezb.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kjp.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://snb.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sti.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ini.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qek.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://era.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lii.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://owx.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://poi.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://flb.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://eee.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://rfu.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://toh.hcnkem.com

Go:   encoding/gob
来源：http://pml.sweek.top

Ruby: Marshal.dump(obj)
来源：http://hva.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vkx.wangshuangyany.cn

================================================================================
来源：http://ved.jinqigfzy.top

L. 网络请求
来源：http://ptm.feifeiyinyue.top

================================================================================
来源：http://vus.birdmap.top

[L01] 发送 GET 请求
来源：http://zwg.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://coq.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pez.yvedp.cn

JS:   await fetch(url)
来源：http://nho.52xcode.cn

TS:   await fetch(url)
来源：http://fuz.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ysq.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://rnj.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sls.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dwf.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://dqf.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lol.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyw.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tle.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kaf.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rwz.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jkr.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iuu.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cep.yuxming.cn

[L03] 设置自定义请求头
来源：http://tff.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wew.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vdz.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zpx.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://prg.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://epu.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wsm.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://scl.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fjk.yangfankeji.com

[L04] 设置超时
来源：http://yoi.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://goi.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://auu.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pfk.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uky.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rgh.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aul.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tyb.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yox.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://ejt.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mze.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rhs.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zqy.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dey.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yfu.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cpk.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wkp.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fwc.shuidangran.top

[L06] 解析响应为 JSON
来源：http://twy.gaohongyu789.top

Py:   resp.json()
来源：http://kok.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://omo.jinghuilouyu.cn

JS:   await resp.json()
来源：http://svk.fengsongda.top

TS:   await resp.json()
来源：http://fma.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jug.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wcg.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://nqp.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wqv.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://yub.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vxw.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nil.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://uwp.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://pyc.tian-w.cn

Java: resp.statusCode()
来源：http://apl.havefunace.top

Go:   resp.StatusCode
来源：http://wmv.haohaochexian.top

Ruby: resp.code.to_i
来源：http://pyu.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://hcv.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://dog.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cgp.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://ywe.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cxw.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://igg.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jti.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qok.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://grk.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gfl.pengpengdd.cyou

================================================================================
来源：http://evq.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://wim.iojbl.cn

================================================================================
来源：http://azt.zhijiandao.cn

[M01] 读取命令行参数
来源：http://phd.daxiang520.top

Py:   sys.argv[1:]
来源：http://twd.yuxming.cn

PHP:  $argv;  $argc;
来源：http://fmc.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://qbv.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://oud.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://awq.pycfn.com

Go:   os.Args[1:]
来源：http://ycr.zhoulong.xyz

Ruby: ARGV
来源：http://fxe.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://iey.jinqigufen.top

[M02] 读取环境变量
来源：http://adm.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://fha.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iaq.fktsv.cn

JS:   process.env.HOME
来源：http://nep.yj202588.top

TS:   process.env.HOME
来源：http://brd.gotoacloud.top

Java: System.getenv("HOME")
来源：http://oft.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wzm.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://aan.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vmr.ivvv.top

[M03] 执行外部命令
来源：http://enj.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tid.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://amb.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xbx.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cml.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aaq.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ynv.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://juu.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://buc.gzhubu.top

[M04] 获取当前工作目录
来源：http://zyl.haohaochexian.top

Py:   os.getcwd()
来源：http://mik.cashguo.top

PHP:  getcwd();
来源：http://sge.tianlin.xyz

JS:   process.cwd()
来源：http://ctu.xuanzx.com

TS:   process.cwd()
来源：http://wew.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://gak.yonumen.top

Go:   os.Getwd()
来源：http://age.tanke756.top

Ruby: Dir.pwd
来源：http://chu.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://urs.yj20258.top

[M05] 设置退出码
来源：http://rfu.shuidangran.top

Py:   sys.exit(1)
来源：http://xdc.zdbjq.cn

PHP:  exit(1);
来源：http://wux.dashuyun.cn

JS:   process.exit(1)
来源：http://hjo.svipenyu.cn

TS:   process.exit(1)
来源：http://qdt.cucudq.cn

Java: System.exit(1)
来源：http://yao.52xcode.cn

Go:   os.Exit(1)
来源：http://arp.shuidangran.top

Ruby: exit 1
来源：http://mtz.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uek.gaohongyu789.top

[M06] 向标准错误输出
来源：http://guu.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://xap.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zzn.zhiwuduotai.top

JS:   console.error("err")
来源：http://kus.0kj1m.cn

TS:   console.error("err")
来源：http://qkk.havefunace.top

Java: System.err.println("err")
来源：http://cqz.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mog.yangfankeji.com

Ruby: warn "err"
来源：http://bic.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://ckf.birdmap.top

[M07] 判断是否为主入口
来源：http://gzz.316326.xyz

Py:   if __name__ == "__main__":
来源：http://zyx.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qig.snrcjt.cn

JS:   require.main === module
来源：http://iip.nanxinkj.top

TS:   require.main === module
来源：http://zpl.daria6918.cn

Java: public static void main(String[] args)
来源：http://njt.haohaochexian.top

Go:   func main()
来源：http://nxl.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://omu.uphjek.com

C#:   static void Main(string[] args)
来源：http://spb.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://duv.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://szl.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://hhl.vehdjk.com

JS:   process.platform;  process.version
来源：http://oou.zdqjudy.top

TS:   process.platform;  process.version
来源：http://pqq.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tex.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://sfs.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wya.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xyj.hesvh.cn

================================================================================
来源：http://mcw.birdmap.top

N. 数据结构与算法
来源：http://lys.zhaomingkeji.xyz

================================================================================
来源：http://swt.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://bws.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cfo.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pmg.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eya.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zrp.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://vjf.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ygw.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xbi.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://tby.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://inm.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://gww.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pvg.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qdd.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://crh.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://otf.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://yjs.zhiwuduotai.top

Ruby: arr.sort
来源：http://dry.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zxh.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://gco.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cio.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://ukn.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mtq.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vna.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kbd.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://edx.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zjh.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ivf.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://fvy.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mbx.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hij.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fux.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gly.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pwd.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jmz.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gin.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oqq.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://czs.jianghu66.top

Py:   math.gcd(a, b)
来源：http://jje.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://udw.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vlt.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rai.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ftx.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xjt.0kj1m.cn

Ruby: a.gcd(b)
来源：http://tdw.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nng.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://yyn.yangfankeji.com

Py:   s == s[::-1]
来源：http://dhz.hesvh.cn

PHP:  $s === strrev($s);
来源：http://gey.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://ioo.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://ifp.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://str.smart0.xyz

Go:   // 双指针从两端比较
来源：http://kvf.yj202588.top

Ruby: s == s.reverse
来源：http://yyf.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rfm.uphjek.com

[N07] 两数之和（返回下标）
来源：http://fgh.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ugc.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vgd.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cbz.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://hhy.xziqi.cn

Java: // 手写 HashMap
来源：http://trd.tian-w.cn

Go:   // 手写 map[int]int
来源：http://uit.snrcjt.cn

Ruby: // 手写 Hash
来源：http://gzy.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://cua.kuanghao11.cn

[N08] 生成全排列
来源：http://gcf.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://qmv.cqqwz.cn

PHP:  // 手写递归交换
来源：http://sxp.316326.xyz

JS:   // 手写回溯递归
来源：http://yqh.xuanzx.com

TS:   // 手写回溯递归
来源：http://bzd.hcnkem.com

Java: // 手写回溯递归
来源：http://kse.ehwqpu.com

Go:   // 手写回溯递归
来源：http://zix.shzxlz.cn

Ruby: arr.permutation.to_a
来源：http://vgf.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://nlv.hywenlv.cn

[N09] 栈与队列
来源：http://lpv.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mbg.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bdl.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://noy.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wqh.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pqz.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hgl.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://unq.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nvu.0kj1m.cn

[N10] 链表节点定义
来源：http://hly.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oew.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dxt.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://run.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wat.yj202588.top

Java: class Node { int v; Node next; }
来源：http://beh.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ywi.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://khp.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ccy.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://fgb.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://avg.hcnkem.com


<!-- 参考信息 -->