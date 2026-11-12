代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://lrk.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://env.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wql.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lms.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://vxg.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://igf.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://bnt.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vtj.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eae.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ouk.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohc.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bwz.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fwh.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nvj.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ofl.jiagoushi.top

[K05] 深拷贝对象
来源：http://axc.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://lrx.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://dnz.wangdashe.top

JS:   structuredClone(obj)
来源：http://tly.vehdjk.com

TS:   structuredClone(obj)
来源：http://pqs.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hyf.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ggx.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jby.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rwu.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://nmn.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oib.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zij.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://leq.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afv.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xit.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://taa.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dgr.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zuc.jyoumei.cn

[K07] 进制转换
来源：http://sui.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dmz.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://san.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kjo.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ryr.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wby.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uwn.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nhq.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zwe.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://abv.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://lvl.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oqg.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://rov.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://yko.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jip.c1oappe.top

Go:   encoding/gob
来源：http://fro.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://lqc.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rit.xziqi.cn

================================================================================
来源：http://sox.ywan-chungtsiang.top

L. 网络请求
来源：http://hty.aizwys.cn

================================================================================
来源：http://ltq.jinqigufen.top

[L01] 发送 GET 请求
来源：http://pfa.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ind.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ihy.hfpthk.cn

JS:   await fetch(url)
来源：http://haa.hongshengwenyu.top

TS:   await fetch(url)
来源：http://bag.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uug.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://qyj.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jbz.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jrw.andypj.xyz

[L02] 发送 POST JSON
来源：http://uiw.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://qxn.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gmm.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ock.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axe.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bwm.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jfk.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nqk.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://djj.ydzc1.top

[L03] 设置自定义请求头
来源：http://xsk.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fjr.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yxd.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://onn.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://siw.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://euw.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wwa.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gtd.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://coq.kuanghao11.cn

[L04] 设置超时
来源：http://ust.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://dsd.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ohz.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jha.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oop.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uvo.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nuu.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zuw.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jcg.pycfn.com

[L05] 上传文件（multipart）
来源：http://eeb.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eou.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tri.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jjs.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tfu.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kcv.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ztc.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://req.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sen.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://buu.fzhhl.top

Py:   resp.json()
来源：http://yvq.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://ygm.zhengqikj.top

JS:   await resp.json()
来源：http://jrx.yj202588.top

TS:   await resp.json()
来源：http://nor.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zjb.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vqr.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://qvw.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rty.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://ftm.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zxm.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kev.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://vyf.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://wud.zycfv.cn

Java: resp.statusCode()
来源：http://svn.andypj.xyz

Go:   resp.StatusCode
来源：http://onm.bjfxy.top

Ruby: resp.code.to_i
来源：http://sql.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://cwx.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://lkn.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lyi.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://xjt.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bvk.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lml.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://idn.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ghe.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tip.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eyz.zdbjq.cn

================================================================================
来源：http://vbm.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://ois.yuanzhike.top

================================================================================
来源：http://crm.hcnkem.com

[M01] 读取命令行参数
来源：http://sgs.shuidangran.top

Py:   sys.argv[1:]
来源：http://xlx.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://qoi.yj20258.top

JS:   process.argv.slice(2)
来源：http://bsr.bbcook.cn

TS:   process.argv.slice(2)
来源：http://ydu.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://phw.sxryk.cn

Go:   os.Args[1:]
来源：http://lqv.hesvh.cn

Ruby: ARGV
来源：http://mdy.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://kwp.cheryme.top

[M02] 读取环境变量
来源：http://obb.yongpay.top

Py:   os.environ.get("HOME")
来源：http://obi.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mrv.xuanzx.com

JS:   process.env.HOME
来源：http://ype.birdmap.top

TS:   process.env.HOME
来源：http://jzz.yj20258.top

Java: System.getenv("HOME")
来源：http://ozu.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aav.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://xyc.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://swh.tarul.cn

[M03] 执行外部命令
来源：http://lvq.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ugq.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vwk.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://sib.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dpp.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sof.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fcy.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://ucq.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://zns.guowangkeji.top

[M04] 获取当前工作目录
来源：http://bku.tanke756.top

Py:   os.getcwd()
来源：http://exr.uphjek.com

PHP:  getcwd();
来源：http://qjy.jqgufenzy.top

JS:   process.cwd()
来源：http://skh.hywenlv.cn

TS:   process.cwd()
来源：http://zde.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://hqq.hongshengwenyu.top

Go:   os.Getwd()
来源：http://wyl.daria6918.cn

Ruby: Dir.pwd
来源：http://abj.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://nqt.daxiang520.top

[M05] 设置退出码
来源：http://okj.hywenlv.cn

Py:   sys.exit(1)
来源：http://zly.xziqi.cn

PHP:  exit(1);
来源：http://tut.fengsongda.top

JS:   process.exit(1)
来源：http://qbk.chenjidiqi.icu

TS:   process.exit(1)
来源：http://jde.sysykeji.top

Java: System.exit(1)
来源：http://ffa.cucudq.cn

Go:   os.Exit(1)
来源：http://ood.daria6918.cn

Ruby: exit 1
来源：http://sst.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aon.zhoulong.xyz

[M06] 向标准错误输出
来源：http://rdg.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://ycg.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://knf.smart0.xyz

JS:   console.error("err")
来源：http://vya.fktsv.cn

TS:   console.error("err")
来源：http://dzc.chenzaomai.com

Java: System.err.println("err")
来源：http://mhz.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hxo.zhongyouzk.top

Ruby: warn "err"
来源：http://zmi.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://gnv.dashuyun.cn

[M07] 判断是否为主入口
来源：http://pul.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://kjx.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mug.ctjpmb.com

JS:   require.main === module
来源：http://brv.zdbjq.cn

TS:   require.main === module
来源：http://vjy.hysaishi.cn

Java: public static void main(String[] args)
来源：http://foo.shuidangran.top

Go:   func main()
来源：http://wyi.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jip.yuxming.cn

C#:   static void Main(string[] args)
来源：http://luk.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://kgs.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://yhm.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://rpb.yongpay.top

JS:   process.platform;  process.version
来源：http://xcg.9152youxi.cn

TS:   process.platform;  process.version
来源：http://cnb.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uew.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jua.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nmk.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cjc.guowangkeji.top

================================================================================
来源：http://azr.9152youxi.cn

N. 数据结构与算法
来源：http://ggi.yj20258888.top

================================================================================
来源：http://hxy.cashguo.top

[N01] 二分查找（有序数组）
来源：http://asx.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://icv.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bmt.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aji.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://adf.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ske.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://ibo.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://dgn.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://pzs.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://elf.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://dhi.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cpc.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ibo.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nws.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qcq.daria6918.cn

Go:   slices.Sort(arr)
来源：http://rjk.bjfxy.top

Ruby: arr.sort
来源：http://eiq.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xaw.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://mza.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mvo.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://qia.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wul.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnz.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://czr.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uqp.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://njc.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://uoe.ydzc1.top

[N04] 斐波那契数列
来源：http://yqk.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://scf.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://afy.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hvd.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wej.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yes.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gkc.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://odx.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://azb.hongshengwenyu.top

[N05] 最大公约数
来源：http://osu.guannengcc.top

Py:   math.gcd(a, b)
来源：http://ory.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://smy.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mad.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qxa.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zyp.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wix.yongpay.top

Ruby: a.gcd(b)
来源：http://szc.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://flx.52xcode.cn

[N06] 判断回文字符串
来源：http://fpw.sysykeji.top

Py:   s == s[::-1]
来源：http://tjt.birdmap.top

PHP:  $s === strrev($s);
来源：http://afh.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://ink.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://zht.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vgs.xinyue.icu

Go:   // 双指针从两端比较
来源：http://kay.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://ipt.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://qpp.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://uzq.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nqd.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qmg.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://dat.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://hcd.quarkkingdee.top

Java: // 手写 HashMap
来源：http://fkp.nwbrower.top

Go:   // 手写 map[int]int
来源：http://pon.aibaodan.cn

Ruby: // 手写 Hash
来源：http://lvn.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lks.52xcode.cn

[N08] 生成全排列
来源：http://pvd.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://ihg.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://mhx.bbcook.cn

JS:   // 手写回溯递归
来源：http://crk.ctjpmb.com

TS:   // 手写回溯递归
来源：http://bcv.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://jim.zycfv.cn

Go:   // 手写回溯递归
来源：http://gnt.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://ifa.ydzc1.top

C#:   // 手写回溯递归
来源：http://ant.jianghu66.top

[N09] 栈与队列
来源：http://xri.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hdg.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pnp.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ddb.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fyk.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yuh.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cts.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pes.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ilw.cdnleiting.top

[N10] 链表节点定义
来源：http://ueg.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qho.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vkv.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wzu.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vyn.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://tak.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ypr.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xnq.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qks.mhx1999.top

[N11] 二叉树中序遍历
来源：http://bnf.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vyo.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://tgy.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://len.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tnj.birdmap.top

Java: // 手写递归
来源：http://gjg.tian-w.cn


<!-- 参考信息 -->