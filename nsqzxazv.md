代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fav.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ucb.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://zzb.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://opi.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gvs.bbcook.cn

Go:   json.Marshal(obj)
来源：http://kmd.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bls.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rui.gzhubu.top

[K02] JSON 字符串转对象
来源：http://crh.ppjwa.cn

Py:   json.loads(s)
来源：http://zng.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vev.yongpay.top

JS:   JSON.parse(s)
来源：http://vdq.yuanzhike.top

TS:   JSON.parse(s)
来源：http://ava.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qkw.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://nkv.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://znx.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bhf.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://vog.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://edq.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iik.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ojr.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://elu.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iwg.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fck.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vci.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jjs.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://csk.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fbk.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xbt.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cct.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bmo.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xoy.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cng.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hly.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ame.fktsv.cn

[K05] 深拷贝对象
来源：http://bex.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://kdo.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://eng.jiagoushi.top

JS:   structuredClone(obj)
来源：http://mfd.snrcjt.cn

TS:   structuredClone(obj)
来源：http://vrt.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ceh.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hyl.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xcw.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zbr.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://tuu.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfm.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bdm.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://elo.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pzs.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://obs.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xja.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zwp.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xmo.hysaishi.cn

[K07] 进制转换
来源：http://meh.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vaj.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zoz.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://goj.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lsx.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhn.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://how.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ayq.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eul.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://dmf.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://jja.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qyv.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://nqr.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://zak.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://evs.cheryme.top

Go:   encoding/gob
来源：http://hau.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://bka.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://psn.bjfxy.top

================================================================================
来源：http://krs.fzhhl.top

L. 网络请求
来源：http://omn.sweek.top

================================================================================
来源：http://bnl.shzxlz.cn

[L01] 发送 GET 请求
来源：http://nbt.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zwr.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ldh.nwbrower.top

JS:   await fetch(url)
来源：http://vxr.jiagoushi.top

TS:   await fetch(url)
来源：http://akb.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://okv.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://bhd.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dqh.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lxf.cashguo.top

[L02] 发送 POST JSON
来源：http://cvb.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://lik.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fea.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bos.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://reb.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oeg.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lgk.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qmb.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://owu.ydzc1.top

[L03] 设置自定义请求头
来源：http://opd.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zvp.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bcl.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://grv.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://prx.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nvr.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zhs.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gji.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ugc.dianchejie.cn

[L04] 设置超时
来源：http://cny.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://yqk.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xmy.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qww.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aut.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://alv.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kur.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nxb.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lbg.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://sgi.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kjv.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://shb.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aha.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xtr.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tlx.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cxi.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rve.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rnk.xylfe.cn

[L06] 解析响应为 JSON
来源：http://vqm.guowangkeji.top

Py:   resp.json()
来源：http://ulk.fehbvm.com

PHP:  json_decode($body, true);
来源：http://wec.chenjidiqi.icu

JS:   await resp.json()
来源：http://xsw.jinqigfzy.top

TS:   await resp.json()
来源：http://vjd.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nlx.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wkz.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://fty.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jeq.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://jta.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mhc.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wcr.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://tct.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://qxy.havefunace.top

Java: resp.statusCode()
来源：http://fdc.epnwcf.com

Go:   resp.StatusCode
来源：http://ess.sxryk.cn

Ruby: resp.code.to_i
来源：http://tug.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://sit.ybcxt.top

[L08] 并发请求多个地址
来源：http://tai.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xgn.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://glz.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hty.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txp.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uee.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qce.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xez.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mgf.yanxiufei.cn

================================================================================
来源：http://tkz.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://qny.gogol.net.cn

================================================================================
来源：http://yrj.hammf.cn

[M01] 读取命令行参数
来源：http://xwo.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://daf.iojbl.cn

PHP:  $argv;  $argc;
来源：http://ehx.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://tsp.hammf.cn

TS:   process.argv.slice(2)
来源：http://rkf.yj20258.top

Java: args 数组（main 方法参数）
来源：http://btc.hnqzz.top

Go:   os.Args[1:]
来源：http://ffx.gotoacloud.top

Ruby: ARGV
来源：http://gnc.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://jia.shuidangran.top

[M02] 读取环境变量
来源：http://cyw.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://ukz.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xlu.yj20258.top

JS:   process.env.HOME
来源：http://ecs.hongshengwenyu.top

TS:   process.env.HOME
来源：http://wdy.birdmap.top

Java: System.getenv("HOME")
来源：http://atb.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wpf.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://lrs.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://joh.zhijiandao.cn

[M03] 执行外部命令
来源：http://pgd.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uuf.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://boq.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kph.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ejk.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sgn.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://njk.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://svv.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://ugw.dianchejie.cn

[M04] 获取当前工作目录
来源：http://xck.ybcxt.top

Py:   os.getcwd()
来源：http://uyq.daria6918.cn

PHP:  getcwd();
来源：http://wrl.hammf.cn

JS:   process.cwd()
来源：http://whp.yanxiufei.cn

TS:   process.cwd()
来源：http://oxz.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://itt.gzhubu.top

Go:   os.Getwd()
来源：http://qrb.tanke756.top

Ruby: Dir.pwd
来源：http://qgl.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iat.epnwcf.com

[M05] 设置退出码
来源：http://btk.fehbvm.com

Py:   sys.exit(1)
来源：http://bmk.wangdashe.top

PHP:  exit(1);
来源：http://kvy.zhixingplan.top

JS:   process.exit(1)
来源：http://oma.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://wet.nwbrower.top

Java: System.exit(1)
来源：http://ylo.mhx1999.top

Go:   os.Exit(1)
来源：http://jvf.birdmap.top

Ruby: exit 1
来源：http://axd.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zps.zhongyouzk.top

[M06] 向标准错误输出
来源：http://rky.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://ara.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://bzp.yj202588.top

JS:   console.error("err")
来源：http://xpb.zdbjq.cn

TS:   console.error("err")
来源：http://ymw.zhixingplan.top

Java: System.err.println("err")
来源：http://sdc.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pzv.jlsjyb.cn

Ruby: warn "err"
来源：http://ths.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://frc.nwbrower.top

[M07] 判断是否为主入口
来源：http://nhj.cashguo.top

Py:   if __name__ == "__main__":
来源：http://xyt.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cqb.quarkkingdee.top

JS:   require.main === module
来源：http://wlo.zdqjudy.top

TS:   require.main === module
来源：http://koc.cdnleiting.top

Java: public static void main(String[] args)
来源：http://whe.sjlbkw.cn

Go:   func main()
来源：http://cpl.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://krr.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://xyc.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://bdd.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://vcz.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://evm.dashuyun.cn

JS:   process.platform;  process.version
来源：http://zru.aibaodan.cn

TS:   process.platform;  process.version
来源：http://rjy.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zbj.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://syn.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bsg.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yja.shzxlz.cn

================================================================================
来源：http://jmi.fanxiaobao.xyz

N. 数据结构与算法
来源：http://ztg.hnxiangtu.top

================================================================================
来源：http://knq.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://hiv.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://lgl.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rra.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxe.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rgc.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xvw.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://arl.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://adw.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://iip.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://byz.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://hia.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://old.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wpj.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hiu.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zok.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://jwe.yj20258.top

Ruby: arr.sort
来源：http://uer.9152youxi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hkn.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://lvg.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kmc.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://wjw.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bqv.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blz.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufa.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gmm.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mzw.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kpn.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://hik.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://far.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://whg.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lhr.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdm.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ldv.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sri.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uyi.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ynw.aizwys.cn

[N05] 最大公约数
来源：http://tys.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://dgd.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mif.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rmi.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ayq.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pmo.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ozc.mhx1999.top

Ruby: a.gcd(b)
来源：http://uyj.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dki.wangdashe.top

[N06] 判断回文字符串
来源：http://qsu.gaohongyu789.top

Py:   s == s[::-1]
来源：http://rvn.yongpay.top

PHP:  $s === strrev($s);
来源：http://qth.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://iky.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://dmm.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uyj.uphjek.com

Go:   // 双指针从两端比较
来源：http://mut.fzhhl.top

Ruby: s == s.reverse
来源：http://sdz.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zjh.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://tcs.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ozy.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fin.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://iup.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://rjg.andypj.xyz

Java: // 手写 HashMap
来源：http://ymd.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://ysn.fengsongda.top

Ruby: // 手写 Hash
来源：http://khr.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zac.vqdsnc.cn

[N08] 生成全排列
来源：http://bys.havefunace.top

Py:   itertools.permutations(arr)
来源：http://pfs.yongpay.top

PHP:  // 手写递归交换
来源：http://ahg.sxryk.cn

JS:   // 手写回溯递归
来源：http://nqg.yuxming.cn

TS:   // 手写回溯递归
来源：http://ftl.xziqi.cn

Java: // 手写回溯递归
来源：http://dlh.jinqigufen.top

Go:   // 手写回溯递归
来源：http://vzy.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://tmj.hywenlv.cn

C#:   // 手写回溯递归
来源：http://qpx.yvedp.cn

[N09] 栈与队列
来源：http://uue.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ttb.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zwf.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gvl.kuanghao11.cn


<!-- 参考信息 -->