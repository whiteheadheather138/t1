代发 wailian999

================================================================================
来源：http://lkw.zhengqikj.top

K. JSON 与序列化
来源：http://lro.aibaodan.cn

================================================================================
来源：http://ewa.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://nzz.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lty.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jgh.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://usj.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://ddl.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bih.hcnkem.com

Go:   json.Marshal(obj)
来源：http://sse.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kyp.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dqb.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://gha.nanxinkj.top

Py:   json.loads(s)
来源：http://ass.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dox.vehdjk.com

JS:   JSON.parse(s)
来源：http://hgo.svipenyu.cn

TS:   JSON.parse(s)
来源：http://wts.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dfj.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://ihm.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://pbp.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wwy.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://xhd.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rzd.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ckl.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gkb.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eli.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eas.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nrf.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://frv.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kbx.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://lvq.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kci.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bgf.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ube.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kum.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wkr.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xwa.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xaq.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jsz.52xcode.cn

[K05] 深拷贝对象
来源：http://srp.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://jbf.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://syi.snrcjt.cn

JS:   structuredClone(obj)
来源：http://zjc.hywenlv.cn

TS:   structuredClone(obj)
来源：http://cgd.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hfv.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyb.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sav.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mfj.smart0.xyz

[K06] 解析 URL 查询串
来源：http://hin.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mwr.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sev.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xuh.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pbv.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ueu.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ksn.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://war.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pkv.svipenyu.cn

[K07] 进制转换
来源：http://baw.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kqn.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vvp.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xft.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bie.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qtd.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gad.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ddr.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://isq.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://fmd.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://yyg.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rcj.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://fyl.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://kme.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://buq.hfpthk.cn

Go:   encoding/gob
来源：http://aqe.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://tqm.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nwd.sxryk.cn

================================================================================
来源：http://rgg.uphjek.com

L. 网络请求
来源：http://zaw.52xcode.cn

================================================================================
来源：http://tlx.cdnleiting.top

[L01] 发送 GET 请求
来源：http://zgb.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xwb.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xzk.sweek.top

JS:   await fetch(url)
来源：http://kbp.jinqigufen.top

TS:   await fetch(url)
来源：http://tws.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bsp.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://nxr.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jlz.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bon.fzhhl.top

[L02] 发送 POST JSON
来源：http://dtq.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zcn.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mng.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usn.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://scg.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mhc.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://asa.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qec.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xxg.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://zzg.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kkc.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mnt.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fdt.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zog.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://krg.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xbt.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qid.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ujf.zhengqikj.top

[L04] 设置超时
来源：http://vtu.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://rmz.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wjn.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tsu.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ngh.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ccx.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qpj.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jsn.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://inm.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://nmr.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lyw.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wve.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://afl.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ccw.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yqs.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bjh.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bur.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jwz.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://yjg.c1oappe.top

Py:   resp.json()
来源：http://lps.xziqi.cn

PHP:  json_decode($body, true);
来源：http://uiw.redwolf501.top

JS:   await resp.json()
来源：http://kxt.yuxming.cn

TS:   await resp.json()
来源：http://shp.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rmr.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hof.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://dfc.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mps.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://izk.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cuk.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vwx.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://zvc.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://mcc.cucudq.cn

Java: resp.statusCode()
来源：http://flk.xylfe.cn

Go:   resp.StatusCode
来源：http://rtt.yvedp.cn

Ruby: resp.code.to_i
来源：http://rlc.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://tag.bjfxy.top

[L08] 并发请求多个地址
来源：http://ezl.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xsk.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://ucz.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgv.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lnu.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ohk.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wlw.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://joq.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qzj.yfazqb.com

================================================================================
来源：http://idr.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://xzt.gzhubu.top

================================================================================
来源：http://uns.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://srs.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://vdi.c1oappe.top

PHP:  $argv;  $argc;
来源：http://puv.cucudq.cn

JS:   process.argv.slice(2)
来源：http://hrd.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://pfp.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://wqv.yanxiufei.cn

Go:   os.Args[1:]
来源：http://pyy.yonumen.top

Ruby: ARGV
来源：http://lpr.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://wbo.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://bjb.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://zts.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jrt.gogol.net.cn

JS:   process.env.HOME
来源：http://agi.ppjwa.cn

TS:   process.env.HOME
来源：http://cto.yonumen.top

Java: System.getenv("HOME")
来源：http://jko.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bbf.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://dhs.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rjx.pycfn.com

[M03] 执行外部命令
来源：http://xyf.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qke.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fcz.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://czt.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bir.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kpr.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://evz.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://onr.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://koc.uphjek.com

[M04] 获取当前工作目录
来源：http://gji.nanxinkj.top

Py:   os.getcwd()
来源：http://eyl.yvedp.cn

PHP:  getcwd();
来源：http://mlm.shanyushiyangtech.top

JS:   process.cwd()
来源：http://huo.dashuyun.cn

TS:   process.cwd()
来源：http://cor.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://tlg.cqqwz.cn

Go:   os.Getwd()
来源：http://gsx.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://amz.jianghu66.top

C#:   Directory.GetCurrentDirectory()
来源：http://hyi.vqdsnc.cn

[M05] 设置退出码
来源：http://uke.snrcjt.cn

Py:   sys.exit(1)
来源：http://ntk.zhoulong.xyz

PHP:  exit(1);
来源：http://epz.cucudq.cn

JS:   process.exit(1)
来源：http://wen.zhiwuduotai.top

TS:   process.exit(1)
来源：http://lqa.yangfankeji.com

Java: System.exit(1)
来源：http://isp.wangdashe.top

Go:   os.Exit(1)
来源：http://fzg.zhixingplan.top

Ruby: exit 1
来源：http://tnf.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://olz.cucudq.cn

[M06] 向标准错误输出
来源：http://owg.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://yid.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jta.zhixingplan.top

JS:   console.error("err")
来源：http://osm.cashguo.top

TS:   console.error("err")
来源：http://oqn.52xcode.cn

Java: System.err.println("err")
来源：http://blq.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xtb.jqgfzy.top

Ruby: warn "err"
来源：http://wkv.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://qmj.svipenyu.cn

[M07] 判断是否为主入口
来源：http://yla.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://uqm.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lzo.gogol.net.cn

JS:   require.main === module
来源：http://yio.jqgufenzy.top

TS:   require.main === module
来源：http://gpx.yvedp.cn

Java: public static void main(String[] args)
来源：http://jpk.jinyuanbaomall.cn

Go:   func main()
来源：http://dos.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yhs.ivvv.top

C#:   static void Main(string[] args)
来源：http://tve.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://ddh.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://amq.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://vys.c1oappe.top

JS:   process.platform;  process.version
来源：http://sqb.jianghu66.top

TS:   process.platform;  process.version
来源：http://sct.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qrp.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://lqu.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pxh.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sih.chenjidiqi.icu

================================================================================
来源：http://fvq.nwbrower.top

N. 数据结构与算法
来源：http://jop.hesvh.cn

================================================================================
来源：http://vls.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://zgd.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://hoo.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cdj.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wpp.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blj.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://ohq.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://upu.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://akf.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://pqs.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://kha.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://ogi.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://quf.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yiu.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gik.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bdo.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://nwx.havefunace.top

Ruby: arr.sort
来源：http://sxq.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://yql.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://gmc.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qqz.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://nnr.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lxv.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ytg.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yhz.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wdu.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vnt.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ket.pycfn.com

[N04] 斐波那契数列
来源：http://gyt.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jff.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jbl.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upt.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://leg.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iji.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xnp.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wfz.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sus.cashguo.top

[N05] 最大公约数
来源：http://zes.xuanzx.com

Py:   math.gcd(a, b)
来源：http://mwb.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vpt.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://riv.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbb.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eri.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tis.fzhhl.top

Ruby: a.gcd(b)
来源：http://yco.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fll.fehbvm.com

[N06] 判断回文字符串
来源：http://qeq.zhongyouzk.top

Py:   s == s[::-1]
来源：http://qwx.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://yrn.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://mqm.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://jvm.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ged.birdmap.top

Go:   // 双指针从两端比较
来源：http://osg.svipenyu.cn

Ruby: s == s.reverse
来源：http://hmh.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wqt.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://ccf.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nto.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://opn.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://fmp.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://hwc.gzhubu.top

Java: // 手写 HashMap
来源：http://gij.sxryk.cn

Go:   // 手写 map[int]int
来源：http://epr.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://ysq.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://deg.svipenyu.cn

[N08] 生成全排列
来源：http://cmb.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://jsf.cdnleiting.top

PHP:  // 手写递归交换
来源：http://pcp.cqqwz.cn

JS:   // 手写回溯递归
来源：http://lnn.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://nao.tanke756.top

Java: // 手写回溯递归
来源：http://trr.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://dud.yongpay.top

Ruby: arr.permutation.to_a
来源：http://vhn.gzhubu.top

C#:   // 手写回溯递归
来源：http://leo.yuanzhike.top


<!-- 参考信息 -->