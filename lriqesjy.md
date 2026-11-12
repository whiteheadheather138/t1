代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vfs.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://suk.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://btj.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://umh.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kxe.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rdv.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mcf.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://luu.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://muj.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://owq.yuxming.cn

[K04] 读取 JSON 文件
来源：http://gox.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://urd.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jpu.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxu.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ehp.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dkk.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://teo.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pns.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nby.havefunace.top

[K05] 深拷贝对象
来源：http://hrp.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://tms.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://dhv.fengsongda.top

JS:   structuredClone(obj)
来源：http://uos.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://dnl.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fvl.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kyd.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://thj.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jmy.tarul.cn

[K06] 解析 URL 查询串
来源：http://gnt.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ayz.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xzh.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tdt.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tlk.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oyc.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://dur.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nea.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gml.daxiang520.top

[K07] 进制转换
来源：http://wdh.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rhq.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://paa.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tjv.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://osx.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qwg.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rts.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pku.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iez.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://vpg.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://miv.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xtj.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://xte.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://tgp.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ahc.jiagoushi.top

Go:   encoding/gob
来源：http://amq.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://dod.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vgf.gaohongyu789.top

================================================================================
来源：http://inl.svipenyu.cn

L. 网络请求
来源：http://apu.shangyingyoupin.top

================================================================================
来源：http://jxs.haohaochexian.top

[L01] 发送 GET 请求
来源：http://qse.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sde.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://djn.dianchejie.cn

JS:   await fetch(url)
来源：http://kia.yongpay.top

TS:   await fetch(url)
来源：http://vnj.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kfi.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://ijr.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://beo.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://klq.ctjpmb.com

[L02] 发送 POST JSON
来源：http://mzz.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://rum.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zql.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qcq.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://esu.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fiy.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cxl.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wtd.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtv.c1oappe.top

[L03] 设置自定义请求头
来源：http://dmz.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rer.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rng.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kma.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://att.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qec.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bqx.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uxk.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qev.bjfxy.top

[L04] 设置超时
来源：http://mma.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://hkp.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nau.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://scu.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yrj.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rkj.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ddz.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ops.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zey.birdmap.top

[L05] 上传文件（multipart）
来源：http://hrq.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mun.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://anz.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mzt.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bvb.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cde.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jzv.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vxp.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gsz.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://qgp.feifeiyinyue.top

Py:   resp.json()
来源：http://wze.birdmap.top

PHP:  json_decode($body, true);
来源：http://trd.chenzaomai.com

JS:   await resp.json()
来源：http://ggl.ivvv.top

TS:   await resp.json()
来源：http://poj.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uzn.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fpq.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://ixn.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://slx.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://ayo.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kgc.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cpr.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://ldg.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://ccx.gotoacloud.top

Java: resp.statusCode()
来源：http://tck.zhixingplan.top

Go:   resp.StatusCode
来源：http://nnb.tanke756.top

Ruby: resp.code.to_i
来源：http://kai.yongpay.top

C#:   (int)resp.StatusCode
来源：http://mpo.sysykeji.top

[L08] 并发请求多个地址
来源：http://cmz.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jrf.sweek.top

PHP:  curl_multi_init() 系列
来源：http://rva.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asy.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qzu.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rhv.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cyr.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zva.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wqc.pycfn.com

================================================================================
来源：http://snz.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://ojp.vehdjk.com

================================================================================
来源：http://fbm.mhx1999.top

[M01] 读取命令行参数
来源：http://wea.gzhubu.top

Py:   sys.argv[1:]
来源：http://asr.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://wqi.fengsongda.top

JS:   process.argv.slice(2)
来源：http://jvx.316326.xyz

TS:   process.argv.slice(2)
来源：http://tam.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://ikb.sjlbkw.cn

Go:   os.Args[1:]
来源：http://bzv.c1oappe.top

Ruby: ARGV
来源：http://hxz.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://pkq.vqdsnc.cn

[M02] 读取环境变量
来源：http://wbb.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://lpr.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gmr.guowangkeji.top

JS:   process.env.HOME
来源：http://wqb.tian-w.cn

TS:   process.env.HOME
来源：http://ghw.nanxinkj.top

Java: System.getenv("HOME")
来源：http://uhd.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ajw.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://tlv.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bta.gotoacloud.top

[M03] 执行外部命令
来源：http://wwb.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://psa.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vzx.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wfe.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xsq.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mke.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fpn.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://fpe.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://evz.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://ayt.ydjk.org.cn

Py:   os.getcwd()
来源：http://bkm.redwolf501.top

PHP:  getcwd();
来源：http://rib.jianghu66.top

JS:   process.cwd()
来源：http://nhb.gotoacloud.top

TS:   process.cwd()
来源：http://gqr.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://bhu.zhiwuduotai.top

Go:   os.Getwd()
来源：http://wah.sysykeji.top

Ruby: Dir.pwd
来源：http://djh.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://urr.birdmap.top

[M05] 设置退出码
来源：http://ozp.havefunace.top

Py:   sys.exit(1)
来源：http://ubo.nanxuanxn.top

PHP:  exit(1);
来源：http://ahm.yj20258.top

JS:   process.exit(1)
来源：http://zon.shzxlz.cn

TS:   process.exit(1)
来源：http://ctp.tarul.cn

Java: System.exit(1)
来源：http://gxq.xziqi.cn

Go:   os.Exit(1)
来源：http://ypw.pengpengdd.cyou

Ruby: exit 1
来源：http://qpt.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gpi.zhengqikj.top

[M06] 向标准错误输出
来源：http://sdf.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://ono.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://gbu.sysykeji.top

JS:   console.error("err")
来源：http://svh.cheryme.top

TS:   console.error("err")
来源：http://wxo.birdmap.top

Java: System.err.println("err")
来源：http://jzj.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wqn.hnqzz.top

Ruby: warn "err"
来源：http://pur.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://wel.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://ffe.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://pef.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mjy.316326.xyz

JS:   require.main === module
来源：http://zzt.jqgfzy.top

TS:   require.main === module
来源：http://uhv.sxryk.cn

Java: public static void main(String[] args)
来源：http://axq.zycfv.cn

Go:   func main()
来源：http://eby.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xoj.fengsongda.top

C#:   static void Main(string[] args)
来源：http://jrh.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://zgf.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://rdo.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://trx.yueranfly.top

JS:   process.platform;  process.version
来源：http://kse.yj202588.top

TS:   process.platform;  process.version
来源：http://jtm.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xxu.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wsv.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ajh.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hbh.ctjpmb.com

================================================================================
来源：http://wqn.bbcook.cn

N. 数据结构与算法
来源：http://uug.aibaodan.cn

================================================================================
来源：http://zbx.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://vuk.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://wmn.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gtd.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uhw.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hyu.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://xin.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://byt.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vkh.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nbf.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://man.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://ibr.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nnz.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kzb.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qza.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fov.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://tii.yangfankeji.com

Ruby: arr.sort
来源：http://jen.ydzc1.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mui.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://eco.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dtx.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://fek.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fez.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://evg.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qsn.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://taa.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://otg.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://yzt.fzhhl.top

[N04] 斐波那契数列
来源：http://hjl.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wki.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nvt.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lrs.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vbr.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ozk.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zcf.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qey.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gzz.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://xgs.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://fak.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://znl.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pkz.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpr.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bav.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixf.guowangkeji.top

Ruby: a.gcd(b)
来源：http://whf.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eoe.dianchejie.cn

[N06] 判断回文字符串
来源：http://xkq.c1oappe.top

Py:   s == s[::-1]
来源：http://aak.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://xna.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://odx.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://sev.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hzr.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://owf.yuxming.cn

Ruby: s == s.reverse
来源：http://ckb.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ozd.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://jwr.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ieh.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zyo.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ckj.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://dui.52xcode.cn

Java: // 手写 HashMap
来源：http://crj.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://izt.nwbrower.top

Ruby: // 手写 Hash
来源：http://qcb.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gmk.tianlin.xyz

[N08] 生成全排列
来源：http://pzn.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://enx.xziqi.cn

PHP:  // 手写递归交换
来源：http://jzf.zycfv.cn

JS:   // 手写回溯递归
来源：http://ckt.yangfankeji.com

TS:   // 手写回溯递归
来源：http://csv.smart0.xyz

Java: // 手写回溯递归
来源：http://ffl.haohaochexian.top

Go:   // 手写回溯递归
来源：http://jju.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://jxn.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://nwv.dianchejie.cn

[N09] 栈与队列
来源：http://tgf.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gol.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mjd.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fdn.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dsw.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tes.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://whn.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mxj.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dbr.yonumen.top

[N10] 链表节点定义
来源：http://ilb.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ros.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://krl.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jwk.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ftv.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://yhv.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://nuu.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cqb.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lsa.fengsongda.top

[N11] 二叉树中序遍历
来源：http://mjg.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hff.yj202588.top


<!-- 参考信息 -->