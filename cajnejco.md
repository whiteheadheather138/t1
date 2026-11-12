代发 wailian999

TS:   JSON.parse(s)
来源：http://wio.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kyq.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://ztf.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://zrg.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cef.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://znw.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://azq.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dho.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qda.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pnp.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mve.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vyx.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nod.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ifb.redwolf501.top

[K04] 读取 JSON 文件
来源：http://djf.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vka.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://itq.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sma.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hlm.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fnr.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ecb.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lim.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qef.nanxuanxn.top

[K05] 深拷贝对象
来源：http://uds.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://xaf.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://wga.nwbrower.top

JS:   structuredClone(obj)
来源：http://eaq.guannengcc.top

TS:   structuredClone(obj)
来源：http://wgu.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://afc.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://emi.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mzx.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zyd.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://ydl.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ult.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kxc.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dhi.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kgb.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kax.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cyy.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://njn.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://smo.sysykeji.top

[K07] 进制转换
来源：http://npe.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://odr.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rde.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xkl.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://obz.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iia.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dls.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gqj.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jji.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://dpu.sweek.top

Py:   pickle.dumps(obj)
来源：http://cqb.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nkt.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://ziu.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://lmz.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://njl.kuanghao11.cn

Go:   encoding/gob
来源：http://urb.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://pjt.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gee.chenjidiqi.icu

================================================================================
来源：http://ruo.jinqigfzy.top

L. 网络请求
来源：http://vih.yangfankeji.com

================================================================================
来源：http://lmk.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://ueh.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lpi.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://orv.nanxinkj.top

JS:   await fetch(url)
来源：http://qkp.cdnleiting.top

TS:   await fetch(url)
来源：http://uro.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://juh.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://mhe.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ddh.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qjx.jyoumei.cn

[L02] 发送 POST JSON
来源：http://vpd.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://quw.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://csz.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cfr.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bju.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bnc.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lju.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ddl.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oai.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://mov.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lsv.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://inp.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vuc.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qdv.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cnm.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gfn.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lxy.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jol.tian-w.cn

[L04] 设置超时
来源：http://kop.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://vmy.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jbd.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hji.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jsb.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fgd.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ijx.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yoa.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lzv.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://tqx.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://prm.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://asc.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xan.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://laf.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sju.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nrr.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lvd.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mwv.iojbl.cn

[L06] 解析响应为 JSON
来源：http://klq.shanyushiyangtech.top

Py:   resp.json()
来源：http://zoj.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://ojz.52xcode.cn

JS:   await resp.json()
来源：http://olo.gogol.net.cn

TS:   await resp.json()
来源：http://fex.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pgt.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mwq.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://mpl.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://egn.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://tbq.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yrx.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qmr.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://onk.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://yqd.dianchejie.cn

Java: resp.statusCode()
来源：http://nph.yongpay.top

Go:   resp.StatusCode
来源：http://fit.sysykeji.top

Ruby: resp.code.to_i
来源：http://pmp.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://kgd.gzhubu.top

[L08] 并发请求多个地址
来源：http://app.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pxw.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://zcj.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ywa.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cjx.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://axt.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nhg.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xek.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zhy.xingfuxueyuan.xyz

================================================================================
来源：http://bvu.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://mcd.zhoulong.xyz

================================================================================
来源：http://eqy.hfpthk.cn

[M01] 读取命令行参数
来源：http://kmv.fktsv.cn

Py:   sys.argv[1:]
来源：http://vxk.jianghu66.top

PHP:  $argv;  $argc;
来源：http://enb.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://hvv.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://jdo.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://lrv.zhengqikj.top

Go:   os.Args[1:]
来源：http://odg.nanxinkj.top

Ruby: ARGV
来源：http://ajg.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://rgb.fehbvm.com

[M02] 读取环境变量
来源：http://cgd.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://gmm.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://owz.ctjpmb.com

JS:   process.env.HOME
来源：http://erc.uphjek.com

TS:   process.env.HOME
来源：http://zmo.c1oappe.top

Java: System.getenv("HOME")
来源：http://fpo.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zad.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://pjb.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wdg.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://wcd.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eqw.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tep.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ljg.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://uxh.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://avw.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rxd.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://uyr.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://dcl.havefunace.top

[M04] 获取当前工作目录
来源：http://qhu.sxryk.cn

Py:   os.getcwd()
来源：http://nav.tianlin.xyz

PHP:  getcwd();
来源：http://pww.jqgufenzy.top

JS:   process.cwd()
来源：http://jqp.pycfn.com

TS:   process.cwd()
来源：http://nki.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://xbz.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://rbd.yanxiufei.cn

Ruby: Dir.pwd
来源：http://nex.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://app.wangdashe.top

[M05] 设置退出码
来源：http://qrx.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://hgu.fktsv.cn

PHP:  exit(1);
来源：http://owt.xziqi.cn

JS:   process.exit(1)
来源：http://qoj.xinyue.icu

TS:   process.exit(1)
来源：http://ooc.jqgufenzy.top

Java: System.exit(1)
来源：http://apc.hywenlv.cn

Go:   os.Exit(1)
来源：http://dhh.chenzaomai.com

Ruby: exit 1
来源：http://usn.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yhg.hcnkem.com

[M06] 向标准错误输出
来源：http://eid.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://tcn.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lpr.zhoulong.xyz

JS:   console.error("err")
来源：http://yep.yuanzhike.top

TS:   console.error("err")
来源：http://yyg.zhiwuduotai.top

Java: System.err.println("err")
来源：http://vie.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dsy.guannengcc.top

Ruby: warn "err"
来源：http://pzk.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://ziq.pycfn.com

[M07] 判断是否为主入口
来源：http://uyf.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://lsi.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://odk.fzhhl.top

JS:   require.main === module
来源：http://tpe.jinghuilouyu.cn

TS:   require.main === module
来源：http://vnq.chenzaomai.com

Java: public static void main(String[] args)
来源：http://qgn.haohaochexian.top

Go:   func main()
来源：http://jtg.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kkd.jianghu66.top

C#:   static void Main(string[] args)
来源：http://nfe.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://wjl.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://erb.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://kpl.zhixingplan.top

JS:   process.platform;  process.version
来源：http://poh.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://gwc.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zoq.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ovt.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kmn.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bwc.yj20258.top

================================================================================
来源：http://flj.gotoacloud.top

N. 数据结构与算法
来源：http://asc.ywan-chungtsiang.top

================================================================================
来源：http://cjf.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://dzk.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://zwj.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mwp.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ycp.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cud.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://zej.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bdx.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jex.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://sxp.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://ivs.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://xzl.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xdj.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kat.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cdw.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qun.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://lrg.yvedp.cn

Ruby: arr.sort
来源：http://drx.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fdm.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://aac.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sgi.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://daj.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpx.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://odq.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vsa.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://irz.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vat.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://wax.daxiang520.top

[N04] 斐波那契数列
来源：http://xpf.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ywt.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qox.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhw.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tju.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://htd.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://snc.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hij.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vqq.cashguo.top

[N05] 最大公约数
来源：http://ikj.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://jbx.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bsn.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wjc.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tez.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://whx.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kjg.dianchejie.cn

Ruby: a.gcd(b)
来源：http://kzv.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tmb.c1oappe.top

[N06] 判断回文字符串
来源：http://ipq.jianghu66.top

Py:   s == s[::-1]
来源：http://yjj.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://abm.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://wpw.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://vbt.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kqh.bjfxy.top

Go:   // 双指针从两端比较
来源：http://pmn.ybcxt.top

Ruby: s == s.reverse
来源：http://jhf.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ntp.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://qtg.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qop.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tbu.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bob.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://ikb.sufxvd.cn

Java: // 手写 HashMap
来源：http://eml.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://diy.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://biw.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://idq.pengpengdd.cyou

[N08] 生成全排列
来源：http://lhe.uphjek.com

Py:   itertools.permutations(arr)
来源：http://csn.shuidangran.top

PHP:  // 手写递归交换
来源：http://liq.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://rcc.xinyue.icu

TS:   // 手写回溯递归
来源：http://eqs.jinqigfzy.top

Java: // 手写回溯递归
来源：http://dbd.ehwqpu.com

Go:   // 手写回溯递归
来源：http://iln.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://ugc.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://chx.jiagoushi.top

[N09] 栈与队列
来源：http://kqq.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qfn.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rsg.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mdt.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ade.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fat.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ryp.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lkw.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://itq.cashguo.top

[N10] 链表节点定义
来源：http://udt.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mbt.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aez.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bkv.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nir.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://qqj.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uly.zhaomingkeji.xyz


<!-- 参考信息 -->