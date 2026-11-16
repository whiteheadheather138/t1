代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cqe.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://wzn.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hxj.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://msa.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mmy.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://sem.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://got.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://adj.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://lku.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eea.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://ndv.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wvs.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fal.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://knn.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hng.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uaf.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sbw.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lll.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wfn.birdmap.top

[K05] 深拷贝对象
来源：http://ekt.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://sey.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://rad.sysykeji.top

JS:   structuredClone(obj)
来源：http://uoh.zhengqikj.top

TS:   structuredClone(obj)
来源：http://ziw.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://pny.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sxl.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eac.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tgt.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://dle.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ptu.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vxu.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpg.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ihc.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jad.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mvd.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uho.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gor.yvedp.cn

[K07] 进制转换
来源：http://fbo.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jlf.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qyf.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ttq.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ozx.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oex.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dmy.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tow.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ray.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://uil.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://fbk.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zlj.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://zpf.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ltd.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://luk.chenjidiqi.icu

Go:   encoding/gob
来源：http://jhr.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://ecc.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xeh.tanke756.top

================================================================================
来源：http://xaq.hcnkem.com

L. 网络请求
来源：http://ppe.vehdjk.com

================================================================================
来源：http://dnk.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://yzq.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mvc.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vvr.redwolf501.top

JS:   await fetch(url)
来源：http://myj.aizwys.cn

TS:   await fetch(url)
来源：http://xio.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mrh.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://wmo.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gox.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sqk.sysykeji.top

[L02] 发送 POST JSON
来源：http://bdo.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eim.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mgr.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jdw.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgl.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ttx.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vyn.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nfg.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qjo.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://ajs.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gbp.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rvf.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://unj.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://erf.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hvt.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ibm.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pcp.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jdq.shanyushiyangkeji.top

[L04] 设置超时
来源：http://jcy.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://ljp.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jso.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mep.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwj.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mum.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mru.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pco.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://juc.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://jui.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oan.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vai.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://suo.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsu.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kbt.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://htp.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://att.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tnn.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://rgl.epnwcf.com

Py:   resp.json()
来源：http://wzu.yj202588.top

PHP:  json_decode($body, true);
来源：http://xnw.shzxlz.cn

JS:   await resp.json()
来源：http://xpy.yuxming.cn

TS:   await resp.json()
来源：http://cnu.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://maq.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://khe.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://gtn.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ksv.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://iqq.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fcx.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://frl.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://aoo.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://llu.tarul.cn

Java: resp.statusCode()
来源：http://vvd.vqdsnc.cn

Go:   resp.StatusCode
来源：http://aky.hfpthk.cn

Ruby: resp.code.to_i
来源：http://paw.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://fzn.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://chm.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yns.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://vvh.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://len.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dho.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://abe.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pmi.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dkh.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xdd.jqgufenzy.top

================================================================================
来源：http://vmj.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://kgz.meibo888.top

================================================================================
来源：http://uwe.hysaishi.cn

[M01] 读取命令行参数
来源：http://swe.jiagoushi.top

Py:   sys.argv[1:]
来源：http://opa.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://nql.iojbl.cn

JS:   process.argv.slice(2)
来源：http://ndv.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://obx.hammf.cn

Java: args 数组（main 方法参数）
来源：http://izd.yj20258.top

Go:   os.Args[1:]
来源：http://xik.yj202588.top

Ruby: ARGV
来源：http://kgs.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://bse.gogol.net.cn

[M02] 读取环境变量
来源：http://fvm.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://ioo.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gpw.kuanghao11.cn

JS:   process.env.HOME
来源：http://erx.jinqigufen.top

TS:   process.env.HOME
来源：http://gez.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://kle.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://siv.cucudq.cn

Ruby: ENV["HOME"]
来源：http://ane.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qvb.fzhhl.top

[M03] 执行外部命令
来源：http://rwm.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hal.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://urx.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sjt.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qho.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kbr.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oaz.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://xxe.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://luz.wangdashe.top

[M04] 获取当前工作目录
来源：http://tff.ivvv.top

Py:   os.getcwd()
来源：http://att.daxiang520.top

PHP:  getcwd();
来源：http://laj.mhx1999.top

JS:   process.cwd()
来源：http://wse.wangshuangyany.cn

TS:   process.cwd()
来源：http://nab.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://dxo.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://pph.zdbjq.cn

Ruby: Dir.pwd
来源：http://jpp.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bbv.yongpay.top

[M05] 设置退出码
来源：http://psk.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://tbu.dianchejie.cn

PHP:  exit(1);
来源：http://zea.0kj1m.cn

JS:   process.exit(1)
来源：http://dtu.ppjwa.cn

TS:   process.exit(1)
来源：http://dkp.nanxinkj.top

Java: System.exit(1)
来源：http://pup.yangfankeji.com

Go:   os.Exit(1)
来源：http://auu.fengsongda.top

Ruby: exit 1
来源：http://bgg.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aaf.iojbl.cn

[M06] 向标准错误输出
来源：http://muo.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://pig.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wmk.iojbl.cn

JS:   console.error("err")
来源：http://xev.daxiang520.top

TS:   console.error("err")
来源：http://lcv.yueranfly.top

Java: System.err.println("err")
来源：http://msc.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aja.kuanghao11.cn

Ruby: warn "err"
来源：http://jsm.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://lcx.cashguo.top

[M07] 判断是否为主入口
来源：http://hcj.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://rkd.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cil.zhixingplan.top

JS:   require.main === module
来源：http://xxh.shangyingyoupin.top

TS:   require.main === module
来源：http://hls.pycfn.com

Java: public static void main(String[] args)
来源：http://huh.jyoumei.cn

Go:   func main()
来源：http://ngo.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iqt.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://ohh.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://ohx.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://ovt.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://awg.ctjpmb.com

JS:   process.platform;  process.version
来源：http://nyw.ppjwa.cn

TS:   process.platform;  process.version
来源：http://aan.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wsz.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gob.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kzo.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vbb.shanyushiyangkeji.top

================================================================================
来源：http://qtm.jinqigufen.top

N. 数据结构与算法
来源：http://wvg.zhiwuduotai.top

================================================================================
来源：http://dgw.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://bbv.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://jfc.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nhp.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://svl.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zuh.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ixs.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://hoz.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://foh.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://pae.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://orx.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://idd.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dmc.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://osa.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ajd.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://suc.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://wzt.jinghuilouyu.cn

Ruby: arr.sort
来源：http://yah.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qyt.tanke756.top

[N03] 快速排序（分治示例）
来源：http://rsb.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://twn.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://dwk.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lju.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pbs.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://isk.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ybk.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nii.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://pay.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://qim.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kcc.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mnj.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hcv.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cmv.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://foo.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rnw.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://smq.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://krr.pengpengdd.cyou

[N05] 最大公约数
来源：http://dvd.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://oqk.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dvl.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pnl.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rpj.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://das.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hqf.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://uli.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xuc.tianlin.xyz

[N06] 判断回文字符串
来源：http://obw.jqgufenzy.top

Py:   s == s[::-1]
来源：http://tpd.bjfxy.top

PHP:  $s === strrev($s);
来源：http://bwq.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://dkc.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://gdt.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nzg.havefunace.top

Go:   // 双指针从两端比较
来源：http://ygc.hnqzz.top

Ruby: s == s.reverse
来源：http://wcz.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xge.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://iel.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ett.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wmx.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://tna.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://rnh.chenzaomai.com

Java: // 手写 HashMap
来源：http://eqp.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://mqc.pycfn.com

Ruby: // 手写 Hash
来源：http://gjv.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gxz.316326.xyz

[N08] 生成全排列
来源：http://zvp.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://pmi.chenzaomai.com

PHP:  // 手写递归交换
来源：http://mmh.yuxming.cn

JS:   // 手写回溯递归
来源：http://ubm.sxryk.cn

TS:   // 手写回溯递归
来源：http://axz.havefunace.top

Java: // 手写回溯递归
来源：http://kzx.sufxvd.cn

Go:   // 手写回溯递归
来源：http://wcv.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://mfw.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://hly.hnxiangtu.top

[N09] 栈与队列
来源：http://rbo.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pab.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://psn.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://niu.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qle.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ydo.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ojy.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uwc.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wit.quarkkingdee.top

[N10] 链表节点定义
来源：http://gok.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wkj.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ecd.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://auw.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xhy.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://hwz.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://nzd.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mmf.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bal.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://wit.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fjc.birdmap.top


<!-- 参考信息 -->