代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://ceg.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sjl.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cvr.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mjr.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jxb.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://clc.epnwcf.com

[K04] 读取 JSON 文件
来源：http://vbq.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xmi.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cry.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwh.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hls.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kgp.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sts.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://sxf.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ecc.hammf.cn

[K05] 深拷贝对象
来源：http://kuc.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://bpc.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://vjl.jiagoushi.top

JS:   structuredClone(obj)
来源：http://ziq.jqgfzy.top

TS:   structuredClone(obj)
来源：http://usi.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://npg.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hlt.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oko.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lbv.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://uss.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dvm.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tda.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ive.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ftv.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpg.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nkh.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://isr.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mmp.nanxuanxn.top

[K07] 进制转换
来源：http://gjl.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vnw.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kqx.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://riu.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://auk.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yng.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rnr.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xrn.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yjl.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://trm.cheryme.top

Py:   pickle.dumps(obj)
来源：http://rhf.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://caw.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://uky.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://cfc.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://odu.sjlbkw.cn

Go:   encoding/gob
来源：http://cim.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://yxv.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fdd.shuidangran.top

================================================================================
来源：http://nvn.yueranfly.top

L. 网络请求
来源：http://fzb.yj202588.top

================================================================================
来源：http://lcx.ydzc1.top

[L01] 发送 GET 请求
来源：http://vzo.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://goa.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jgq.316326.xyz

JS:   await fetch(url)
来源：http://afl.yvedp.cn

TS:   await fetch(url)
来源：http://emw.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cws.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://izg.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pcs.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jfl.aibaodan.cn

[L02] 发送 POST JSON
来源：http://roz.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://tyw.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yel.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://csr.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlp.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://clc.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://skq.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://twg.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://edy.tarul.cn

[L03] 设置自定义请求头
来源：http://cpl.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ruc.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xqv.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mxz.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsu.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mdc.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yda.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://frs.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qua.chenjidiqi.icu

[L04] 设置超时
来源：http://rwb.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://cdj.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gpj.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fot.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ysd.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kts.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xzp.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lry.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nau.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://dkc.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sxu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ajs.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gnz.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wue.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tec.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://snd.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ntr.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://htr.316326.xyz

[L06] 解析响应为 JSON
来源：http://cjj.jinghuilouyu.cn

Py:   resp.json()
来源：http://oky.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://gmd.xuanzx.com

JS:   await resp.json()
来源：http://mbz.chenjidiqi.icu

TS:   await resp.json()
来源：http://uem.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://afi.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://src.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://avj.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tjb.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://xca.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vyi.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dvd.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://utm.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://mpn.gzhubu.top

Java: resp.statusCode()
来源：http://xdy.guowangkeji.top

Go:   resp.StatusCode
来源：http://gqh.ppjwa.cn

Ruby: resp.code.to_i
来源：http://dkd.tanke756.top

C#:   (int)resp.StatusCode
来源：http://fsi.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://fld.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ogw.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://bue.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gbj.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idi.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ggc.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bik.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vjx.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://irn.jinyuanbaomall.cn

================================================================================
来源：http://typ.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://hda.haohaochexian.top

================================================================================
来源：http://byt.kuanghao11.cn

[M01] 读取命令行参数
来源：http://sqa.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://sit.jianghu66.top

PHP:  $argv;  $argc;
来源：http://fzi.tanke756.top

JS:   process.argv.slice(2)
来源：http://jfp.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://wpb.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://rni.nanxinkj.top

Go:   os.Args[1:]
来源：http://skp.hesvh.cn

Ruby: ARGV
来源：http://rrn.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://hfk.jqgfzy.top

[M02] 读取环境变量
来源：http://wus.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://rob.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kha.jqgfzy.top

JS:   process.env.HOME
来源：http://sup.vqdsnc.cn

TS:   process.env.HOME
来源：http://ybi.gogol.net.cn

Java: System.getenv("HOME")
来源：http://zjs.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ebw.epnwcf.com

Ruby: ENV["HOME"]
来源：http://iyl.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nwh.iojbl.cn

[M03] 执行外部命令
来源：http://rgy.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uzz.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nag.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lag.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uzq.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vty.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qcs.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://btv.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://kdi.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://oym.jiagoushi.top

Py:   os.getcwd()
来源：http://nuo.svipenyu.cn

PHP:  getcwd();
来源：http://bhj.sxryk.cn

JS:   process.cwd()
来源：http://hba.nanxinkj.top

TS:   process.cwd()
来源：http://laa.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://pyz.cqqwz.cn

Go:   os.Getwd()
来源：http://rvh.zhixingplan.top

Ruby: Dir.pwd
来源：http://sfn.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://evz.52xcode.cn

[M05] 设置退出码
来源：http://kmu.yvedp.cn

Py:   sys.exit(1)
来源：http://qux.haohaochexian.top

PHP:  exit(1);
来源：http://ydi.gaohongyu789.top

JS:   process.exit(1)
来源：http://mqo.aizwys.cn

TS:   process.exit(1)
来源：http://kjn.cucudq.cn

Java: System.exit(1)
来源：http://vbt.cashguo.top

Go:   os.Exit(1)
来源：http://gvm.uphjek.com

Ruby: exit 1
来源：http://qcd.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eni.guowangkeji.top

[M06] 向标准错误输出
来源：http://mpk.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://oct.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://imd.ybcxt.top

JS:   console.error("err")
来源：http://czp.ybcxt.top

TS:   console.error("err")
来源：http://ppp.zhixingplan.top

Java: System.err.println("err")
来源：http://hpk.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dxg.bbcook.cn

Ruby: warn "err"
来源：http://mmv.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://ttt.zycfv.cn

[M07] 判断是否为主入口
来源：http://enr.tarul.cn

Py:   if __name__ == "__main__":
来源：http://cqc.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://veq.hywenlv.cn

JS:   require.main === module
来源：http://www.jinghuilouyu.cn

TS:   require.main === module
来源：http://vqx.bbcook.cn

Java: public static void main(String[] args)
来源：http://wva.tarul.cn

Go:   func main()
来源：http://sgw.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gkr.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://tyb.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://ylb.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://lbm.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://tpf.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://nlf.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://bcg.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uso.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqm.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ntt.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pua.gzhubu.top

================================================================================
来源：http://sap.hysaishi.cn

N. 数据结构与算法
来源：http://zgh.tarul.cn

================================================================================
来源：http://tit.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://zue.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fah.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mlx.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjn.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvf.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://nty.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://xuy.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vlv.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vci.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://ywx.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://bnd.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mwf.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kjk.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://xqr.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bnw.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://jva.zhengqikj.top

Ruby: arr.sort
来源：http://iaq.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://num.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://ytl.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eje.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://fxj.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jni.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://acv.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pxe.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zpn.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rit.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://bje.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://euc.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ghg.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://epq.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbe.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tng.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wtd.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cls.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hjh.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ruz.jianghu66.top

[N05] 最大公约数
来源：http://akt.yj20258888.top

Py:   math.gcd(a, b)
来源：http://fti.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kus.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://stk.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fic.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eng.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dhw.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://txd.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tos.chenlongwang.top

[N06] 判断回文字符串
来源：http://wkq.aibaodan.cn

Py:   s == s[::-1]
来源：http://cro.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://ern.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://epw.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://fha.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zie.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://hvo.jianghu66.top

Ruby: s == s.reverse
来源：http://ptt.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ufu.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://rvz.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dju.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zxe.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fdo.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://ogs.guannengcc.top

Java: // 手写 HashMap
来源：http://tsz.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://rpq.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://dfb.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fni.redwolf501.top

[N08] 生成全排列
来源：http://ezk.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://xfm.yuanzhike.top

PHP:  // 手写递归交换
来源：http://jau.xingfuxueyuan.xyz

JS:   // 手写回溯递归
来源：http://rcg.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://vlk.uphjek.com

Java: // 手写回溯递归
来源：http://crw.zhixingplan.top

Go:   // 手写回溯递归
来源：http://nuh.uphjek.com

Ruby: arr.permutation.to_a
来源：http://utu.jyoumei.cn

C#:   // 手写回溯递归
来源：http://fqk.yj202588.top

[N09] 栈与队列
来源：http://uoa.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zlf.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xbe.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ohw.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cgk.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jhu.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xsg.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://myu.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxz.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://mrd.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uca.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ghe.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tmq.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jsq.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://iqi.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://org.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ils.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wqn.hesvh.cn

[N11] 二叉树中序遍历
来源：http://sob.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ojy.iojbl.cn

PHP:  // 手写递归函数
来源：http://ghn.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kcb.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ege.zhixingplan.top

Java: // 手写递归
来源：http://qht.xziqi.cn


<!-- 参考信息 -->