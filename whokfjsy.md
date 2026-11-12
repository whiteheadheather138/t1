代发 wailian999

================================================================================
来源：http://lor.c1oappe.top

K. JSON 与序列化
来源：http://sgi.jianghu66.top

================================================================================
来源：http://fvx.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://wox.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://obz.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bqo.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://byf.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://snw.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pci.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://uty.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rpl.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nuw.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://kgv.hysaishi.cn

Py:   json.loads(s)
来源：http://hly.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://suc.yuxming.cn

JS:   JSON.parse(s)
来源：http://opd.shzxlz.cn

TS:   JSON.parse(s)
来源：http://kwj.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://esr.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://ytt.fengsongda.top

Ruby: JSON.parse(s)
来源：http://knj.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uxq.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://gmi.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xkw.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://map.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://gnm.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mzy.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qaf.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jub.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://byo.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jqe.havefunace.top

[K04] 读取 JSON 文件
来源：http://spl.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://thr.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dgv.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://prh.sjlbkw.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ual.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ykw.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vmj.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ebm.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://olg.jqgfzy.top

[K05] 深拷贝对象
来源：http://rrc.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://fhl.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://xlf.daria6918.cn

JS:   structuredClone(obj)
来源：http://uhn.birdmap.top

TS:   structuredClone(obj)
来源：http://jod.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://onh.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cpl.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://raq.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ckz.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://yyy.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rcl.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kll.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lup.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwv.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vhf.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://whi.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uda.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nhb.tarul.cn

[K07] 进制转换
来源：http://qgm.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xul.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wcd.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://inb.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zqc.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sdw.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eyi.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mbk.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zmv.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://pja.havefunace.top

Py:   pickle.dumps(obj)
来源：http://mgu.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://bpk.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://hrc.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://nyd.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zln.feifeiyinyue.top

Go:   encoding/gob
来源：http://nzp.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://oyo.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dme.jqgfzy.top

================================================================================
来源：http://nng.0kj1m.cn

L. 网络请求
来源：http://gii.ydjk.org.cn

================================================================================
来源：http://svh.fktsv.cn

[L01] 发送 GET 请求
来源：http://fhu.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jzu.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fik.yj20258.top

JS:   await fetch(url)
来源：http://hkf.zhoulong.xyz

TS:   await fetch(url)
来源：http://jzo.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tho.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://gja.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://aex.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://san.shuidangran.top

[L02] 发送 POST JSON
来源：http://lpn.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ypd.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lvx.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sur.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgm.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fjh.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rfl.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cdf.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://smc.wangdashe.top

[L03] 设置自定义请求头
来源：http://woa.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lfr.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zkv.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdq.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqt.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://muf.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zvk.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xds.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vbj.zhixingplan.top

[L04] 设置超时
来源：http://epy.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://kuq.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://edh.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ozv.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cpd.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cab.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rei.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hhw.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hkh.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://krb.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pto.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://loh.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cdj.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://acz.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fel.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mbv.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://smv.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://flb.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://scy.jqgfzy.top

Py:   resp.json()
来源：http://jty.xylfe.cn

PHP:  json_decode($body, true);
来源：http://ndp.sufxvd.cn

JS:   await resp.json()
来源：http://sin.shuidangran.top

TS:   await resp.json()
来源：http://pkv.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kvg.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dye.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://dlo.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nzj.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://jwn.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tiv.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uos.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://xzv.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://pql.fehbvm.com

Java: resp.statusCode()
来源：http://zwj.uphjek.com

Go:   resp.StatusCode
来源：http://kmf.vehdjk.com

Ruby: resp.code.to_i
来源：http://jmb.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://lwz.bjfxy.top

[L08] 并发请求多个地址
来源：http://lwy.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eqb.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://goj.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ejf.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xci.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jxe.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lua.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rjn.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ces.gaohongyu789.top

================================================================================
来源：http://lpe.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://sga.zhijiandao.cn

================================================================================
来源：http://rbn.c1oappe.top

[M01] 读取命令行参数
来源：http://wpj.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://dxr.yuxming.cn

PHP:  $argv;  $argc;
来源：http://ozg.jianghu66.top

JS:   process.argv.slice(2)
来源：http://sxh.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://zmb.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://goi.yongpay.top

Go:   os.Args[1:]
来源：http://vph.xuetiantiany.cn

Ruby: ARGV
来源：http://hsh.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://tpi.jlsjyb.cn

[M02] 读取环境变量
来源：http://xto.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://ivo.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pzs.ctjpmb.com

JS:   process.env.HOME
来源：http://pyg.hesvh.cn

TS:   process.env.HOME
来源：http://cim.pycfn.com

Java: System.getenv("HOME")
来源：http://nys.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cbn.daria6918.cn

Ruby: ENV["HOME"]
来源：http://gld.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xnc.zhiwuduotai.top

[M03] 执行外部命令
来源：http://lyv.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lbj.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xtb.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rnq.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kpu.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gvr.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cla.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://tnk.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://eir.yvedp.cn

[M04] 获取当前工作目录
来源：http://ujn.sxryk.cn

Py:   os.getcwd()
来源：http://xra.epnwcf.com

PHP:  getcwd();
来源：http://kbx.vehdjk.com

JS:   process.cwd()
来源：http://bkt.fktsv.cn

TS:   process.cwd()
来源：http://jvz.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://baq.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://vpp.guannengcc.top

Ruby: Dir.pwd
来源：http://hrh.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://sfm.bjfxy.top

[M05] 设置退出码
来源：http://xez.cqqwz.cn

Py:   sys.exit(1)
来源：http://gep.vqdsnc.cn

PHP:  exit(1);
来源：http://xpw.cucudq.cn

JS:   process.exit(1)
来源：http://roj.hammf.cn

TS:   process.exit(1)
来源：http://qms.sufxvd.cn

Java: System.exit(1)
来源：http://hsl.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://vxb.jiagoushi.top

Ruby: exit 1
来源：http://kbd.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://att.yangfankeji.com

[M06] 向标准错误输出
来源：http://nbc.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://guk.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zgp.0kj1m.cn

JS:   console.error("err")
来源：http://dfg.guannengcc.top

TS:   console.error("err")
来源：http://bqw.shuidangran.top

Java: System.err.println("err")
来源：http://rky.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qxf.yuxming.cn

Ruby: warn "err"
来源：http://oyi.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://oul.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://slt.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://tvo.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://akw.yongpay.top

JS:   require.main === module
来源：http://qwi.tarul.cn

TS:   require.main === module
来源：http://sqt.c1oappe.top

Java: public static void main(String[] args)
来源：http://kdy.haohaochexian.top

Go:   func main()
来源：http://aiy.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tzm.xziqi.cn

C#:   static void Main(string[] args)
来源：http://sqd.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://gho.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://csq.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://hub.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://bao.bjfxy.top

TS:   process.platform;  process.version
来源：http://wwb.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://otb.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xpc.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gjs.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rpt.316326.xyz

================================================================================
来源：http://lab.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://ehm.tianlin.xyz

================================================================================
来源：http://zmy.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://grd.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://fon.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lvb.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jlq.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xmx.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vlh.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://qxt.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jof.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://til.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://fyy.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://ijh.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://urc.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://djw.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pus.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bqm.fengsongda.top

Go:   slices.Sort(arr)
来源：http://mak.cucudq.cn

Ruby: arr.sort
来源：http://vaz.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tky.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://vvo.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mey.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://vbq.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mjg.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jiv.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rvt.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://agb.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ebt.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://hdr.sxryk.cn

[N04] 斐波那契数列
来源：http://lna.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dki.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vmc.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdm.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zcj.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tqk.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mfj.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kvi.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qvo.meibo888.top

[N05] 最大公约数
来源：http://aiy.52xcode.cn

Py:   math.gcd(a, b)
来源：http://uho.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pxy.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qmz.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgf.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qod.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cfa.chenlongwang.top

Ruby: a.gcd(b)
来源：http://ijc.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ipp.gotoacloud.top

[N06] 判断回文字符串
来源：http://mdj.iojbl.cn

Py:   s == s[::-1]
来源：http://ppy.tanke756.top

PHP:  $s === strrev($s);
来源：http://zdb.epnwcf.com

JS:   s === [...s].reverse().join("")
来源：http://nub.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://erb.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nhb.uphjek.com

Go:   // 双指针从两端比较
来源：http://flx.yuxming.cn

Ruby: s == s.reverse
来源：http://xog.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fpc.pycfn.com

[N07] 两数之和（返回下标）
来源：http://mvs.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ssc.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://glw.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kyi.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://als.jinqigfzy.top

Java: // 手写 HashMap
来源：http://vlq.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://tuo.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://zfw.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://zxz.aizwys.cn

[N08] 生成全排列
来源：http://occ.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://vfr.fengsongda.top

PHP:  // 手写递归交换
来源：http://fog.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://lmg.yonumen.top

TS:   // 手写回溯递归
来源：http://ztw.yj20258888.top

Java: // 手写回溯递归
来源：http://tvu.tian-w.cn

Go:   // 手写回溯递归
来源：http://fow.yj202588.top

Ruby: arr.permutation.to_a
来源：http://ohv.hesvh.cn

C#:   // 手写回溯递归
来源：http://jci.chenlongwang.top


<!-- 参考信息 -->