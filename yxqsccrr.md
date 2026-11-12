代发 wailian999

TS:   JSON.parse(s)
来源：http://fxu.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://huy.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://mmo.gzhubu.top

Ruby: JSON.parse(s)
来源：http://vut.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lfc.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://snf.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tgc.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sgo.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pgq.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://svd.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://elw.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fyt.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zhk.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dir.daria6918.cn

[K04] 读取 JSON 文件
来源：http://rmm.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xsx.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ttk.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://heo.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bkh.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oxo.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tso.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fyj.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zcv.xylfe.cn

[K05] 深拷贝对象
来源：http://dwz.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://pbq.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://hpo.yonumen.top

JS:   structuredClone(obj)
来源：http://sdc.daxiang520.top

TS:   structuredClone(obj)
来源：http://jpg.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kib.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aco.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://umo.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://epk.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://dpg.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tgb.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qlr.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://plv.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wtd.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rqn.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rnb.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nba.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xkt.ywan-chungtsiang.top

[K07] 进制转换
来源：http://bvr.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ogo.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mxu.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wsc.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyp.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hpx.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yro.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://afn.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qop.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://fph.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://efl.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://myh.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://dnu.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://dcb.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yjs.uphjek.com

Go:   encoding/gob
来源：http://zqf.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://ouz.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yym.shuidangran.top

================================================================================
来源：http://mnv.kuanghao11.cn

L. 网络请求
来源：http://shc.shuidangran.top

================================================================================
来源：http://owr.cheryme.top

[L01] 发送 GET 请求
来源：http://rbf.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://maa.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://foy.zdqjudy.top

JS:   await fetch(url)
来源：http://cyi.jqgufenzy.top

TS:   await fetch(url)
来源：http://wdp.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cjk.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://aba.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://adc.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://afv.yj202588.top

[L02] 发送 POST JSON
来源：http://jqm.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://dda.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uxb.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ews.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baf.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugv.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uas.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ylg.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bhn.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://gsv.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rmg.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ifa.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vsc.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uas.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qsh.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nti.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hoz.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wez.yangfankeji.com

[L04] 设置超时
来源：http://exs.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://tjp.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://chq.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhe.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zza.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yii.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czc.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kpw.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://urr.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://ysj.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blt.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fxu.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ced.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ztt.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ryb.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bzp.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kab.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jsq.iojbl.cn

[L06] 解析响应为 JSON
来源：http://ilq.cucudq.cn

Py:   resp.json()
来源：http://pjo.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://yxo.cheryme.top

JS:   await resp.json()
来源：http://mpb.hysaishi.cn

TS:   await resp.json()
来源：http://nwv.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lrs.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dto.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://dtk.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yqi.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://hbf.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yxq.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjh.pycfn.com

JS:   resp.ok;  resp.status
来源：http://bum.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://uew.zhixingplan.top

Java: resp.statusCode()
来源：http://alo.uphjek.com

Go:   resp.StatusCode
来源：http://twf.cqqwz.cn

Ruby: resp.code.to_i
来源：http://hfj.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://npn.zycfv.cn

[L08] 并发请求多个地址
来源：http://kmp.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://erz.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://jno.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jbk.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzi.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eal.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jkl.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xcm.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oue.jyoumei.cn

================================================================================
来源：http://wbi.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ojz.sweek.top

================================================================================
来源：http://hkb.ybcxt.top

[M01] 读取命令行参数
来源：http://jfj.ehwqpu.com

Py:   sys.argv[1:]
来源：http://qyz.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://bmt.xinyue.icu

JS:   process.argv.slice(2)
来源：http://jin.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://fgi.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://gyt.gzhubu.top

Go:   os.Args[1:]
来源：http://qvs.aizwys.cn

Ruby: ARGV
来源：http://bud.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://hdr.pengpengdd.cyou

[M02] 读取环境变量
来源：http://tlk.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://vss.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fvj.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://fiv.daxiang520.top

TS:   process.env.HOME
来源：http://wfe.mhx1999.top

Java: System.getenv("HOME")
来源：http://huv.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sfn.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://nqv.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://adq.snrcjt.cn

[M03] 执行外部命令
来源：http://rgv.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hzb.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aig.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mye.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://suc.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jbu.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://xpl.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://gqi.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://bwg.yj202588.top

[M04] 获取当前工作目录
来源：http://wuo.hywenlv.cn

Py:   os.getcwd()
来源：http://spa.hysaishi.cn

PHP:  getcwd();
来源：http://sns.yuanzhike.top

JS:   process.cwd()
来源：http://rsx.yuxming.cn

TS:   process.cwd()
来源：http://wld.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://ppd.hysaishi.cn

Go:   os.Getwd()
来源：http://ogx.gaohongyu789.top

Ruby: Dir.pwd
来源：http://sos.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jqm.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://cnc.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://xok.hesvh.cn

PHP:  exit(1);
来源：http://aip.sysykeji.top

JS:   process.exit(1)
来源：http://ouv.9152youxi.cn

TS:   process.exit(1)
来源：http://hsa.hnqzz.top

Java: System.exit(1)
来源：http://vdj.tarul.cn

Go:   os.Exit(1)
来源：http://tmx.fzhhl.top

Ruby: exit 1
来源：http://jvw.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wus.hywenlv.cn

[M06] 向标准错误输出
来源：http://jxm.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://lkt.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zls.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://opw.vqdsnc.cn

TS:   console.error("err")
来源：http://ibx.svipenyu.cn

Java: System.err.println("err")
来源：http://oli.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rlk.snrcjt.cn

Ruby: warn "err"
来源：http://rok.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://xsf.mhx1999.top

[M07] 判断是否为主入口
来源：http://wtr.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://zbi.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ywf.yonumen.top

JS:   require.main === module
来源：http://rqp.yvedp.cn

TS:   require.main === module
来源：http://nkb.ctjpmb.com

Java: public static void main(String[] args)
来源：http://vty.xinyue.icu

Go:   func main()
来源：http://pjb.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cxz.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://dro.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://dvy.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://vrv.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://jnx.dianchejie.cn

JS:   process.platform;  process.version
来源：http://stf.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://qlh.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ozp.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bap.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fvt.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bwx.yueranfly.top

================================================================================
来源：http://xbc.gotoacloud.top

N. 数据结构与算法
来源：http://vds.fehbvm.com

================================================================================
来源：http://qfa.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://yqa.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://wku.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vou.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pqn.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oci.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yyb.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://vse.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iwk.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://chr.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://veg.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://huk.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kfm.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://oxi.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mft.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://msd.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://bxk.svipenyu.cn

Ruby: arr.sort
来源：http://xji.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yxs.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://ttx.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nit.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://yhb.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zcg.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wue.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tfx.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ysl.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iti.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fiv.9152youxi.cn

[N04] 斐波那契数列
来源：http://lge.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xyx.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bgh.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fzj.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vjw.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mtd.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cky.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xyo.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wby.sxryk.cn

[N05] 最大公约数
来源：http://dcp.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://wqn.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lxf.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vcq.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szb.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hjg.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pfd.tarul.cn

Ruby: a.gcd(b)
来源：http://lqw.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qcx.haohaochexian.top

[N06] 判断回文字符串
来源：http://ero.chenzaomai.com

Py:   s == s[::-1]
来源：http://pje.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://aig.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://oem.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://wpf.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lgs.pycfn.com

Go:   // 双指针从两端比较
来源：http://zav.mhx1999.top

Ruby: s == s.reverse
来源：http://fkz.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nmh.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://kko.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bti.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jnf.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xpx.gzhubu.top

TS:   // 手写 Map<string, number>
来源：http://pok.hysaishi.cn

Java: // 手写 HashMap
来源：http://zzo.uphjek.com

Go:   // 手写 map[int]int
来源：http://vil.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://jbh.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://okr.jianghu66.top

[N08] 生成全排列
来源：http://srk.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://btx.ppjwa.cn

PHP:  // 手写递归交换
来源：http://nmr.xylfe.cn

JS:   // 手写回溯递归
来源：http://rxg.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://bqg.andypj.xyz

Java: // 手写回溯递归
来源：http://xgj.hywenlv.cn

Go:   // 手写回溯递归
来源：http://efn.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://jdl.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://mzv.hcnkem.com

[N09] 栈与队列
来源：http://ghm.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qdh.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iit.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ter.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cgl.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yjo.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://big.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uqb.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ejx.jqgufenzy.top

[N10] 链表节点定义
来源：http://psv.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qcc.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://opq.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://skz.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rav.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://osm.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://vkk.hfpthk.cn


<!-- 参考信息 -->