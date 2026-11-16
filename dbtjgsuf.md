代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sdx.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://fwi.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://klr.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vni.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://wgu.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://kun.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nwb.sxryk.cn

JS:   JSON.parse(s)
来源：http://gxu.hnqzz.top

TS:   JSON.parse(s)
来源：http://mvn.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bjg.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://rrc.ybcxt.top

Ruby: JSON.parse(s)
来源：http://six.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hfc.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://kav.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hqi.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwm.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pze.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ynm.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mey.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yqt.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://kxf.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ibi.ybcxt.top

[K04] 读取 JSON 文件
来源：http://har.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ykp.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dam.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gsa.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://anq.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bli.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wyz.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://frs.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ivc.nwbrower.top

[K05] 深拷贝对象
来源：http://jul.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://rwa.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://ocz.jiagoushi.top

JS:   structuredClone(obj)
来源：http://sqn.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://wwy.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gyi.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qyh.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mcb.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yzm.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://qhi.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xol.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nnr.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qeo.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://obj.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zgo.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rss.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://miq.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ami.ydjk.org.cn

[K07] 进制转换
来源：http://wmt.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kha.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iyw.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://grv.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ywf.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xik.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jsr.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dfi.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lio.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://twn.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://gsw.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rev.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://gwj.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://ewj.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sgc.xuetiantiany.cn

Go:   encoding/gob
来源：http://pus.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://rsh.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fqt.ivvv.top

================================================================================
来源：http://mix.nanxuanxn.top

L. 网络请求
来源：http://iyv.jianghu66.top

================================================================================
来源：http://xnu.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://xxv.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ktd.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gxd.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://mgd.jqgufenzy.top

TS:   await fetch(url)
来源：http://ilp.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://avh.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://urn.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://swr.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cxq.meibo888.top

[L02] 发送 POST JSON
来源：http://tks.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://pwe.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kjb.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kls.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsv.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xnt.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fxs.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://naz.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pgc.zhixingplan.top

[L03] 设置自定义请求头
来源：http://xcz.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://khs.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fdi.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayj.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yka.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zyi.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yax.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xrn.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dil.ydjk.org.cn

[L04] 设置超时
来源：http://ocp.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://btv.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ilx.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ylp.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zsb.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aqu.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://png.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kld.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xnw.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://vik.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kxc.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jto.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://arf.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hnl.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rcm.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xwc.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtj.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gmt.cashguo.top

[L06] 解析响应为 JSON
来源：http://uda.zhaomingkeji.xyz

Py:   resp.json()
来源：http://dlv.fengsongda.top

PHP:  json_decode($body, true);
来源：http://nrq.xuanzx.com

JS:   await resp.json()
来源：http://yjx.jyoumei.cn

TS:   await resp.json()
来源：http://qei.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ihy.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wuz.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://nhn.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rdq.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://tbr.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://afr.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hdf.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://xtr.tarul.cn

TS:   resp.ok;  resp.status
来源：http://iuy.gzhubu.top

Java: resp.statusCode()
来源：http://jks.snrcjt.cn

Go:   resp.StatusCode
来源：http://dmh.fzhhl.top

Ruby: resp.code.to_i
来源：http://bke.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://raj.ehwqpu.com

[L08] 并发请求多个地址
来源：http://qob.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dai.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://uuh.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dcl.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pbo.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bxq.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uet.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vgc.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://puq.shzxlz.cn

================================================================================
来源：http://yzm.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://wta.tianlin.xyz

================================================================================
来源：http://cxu.zhongyouzk.top

[M01] 读取命令行参数
来源：http://gel.ybcxt.top

Py:   sys.argv[1:]
来源：http://dvd.ydzc1.top

PHP:  $argv;  $argc;
来源：http://qxw.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://jdq.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://fhy.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://vos.guannengcc.top

Go:   os.Args[1:]
来源：http://gmm.shangyingyoupin.top

Ruby: ARGV
来源：http://zdu.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://tam.jianghu66.top

[M02] 读取环境变量
来源：http://red.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://qvz.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cxh.yueranfly.top

JS:   process.env.HOME
来源：http://gxw.yueranfly.top

TS:   process.env.HOME
来源：http://pgl.ybcxt.top

Java: System.getenv("HOME")
来源：http://dza.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vtm.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://uuj.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bja.daria6918.cn

[M03] 执行外部命令
来源：http://pib.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kdp.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bjl.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://moa.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qyz.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hgy.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xmp.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://zqr.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://jsa.c1oappe.top

[M04] 获取当前工作目录
来源：http://iyf.aizwys.cn

Py:   os.getcwd()
来源：http://zik.bbcook.cn

PHP:  getcwd();
来源：http://nwl.jiagoushi.top

JS:   process.cwd()
来源：http://pbl.vqdsnc.cn

TS:   process.cwd()
来源：http://war.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://vua.vqdsnc.cn

Go:   os.Getwd()
来源：http://hhu.fehbvm.com

Ruby: Dir.pwd
来源：http://fmq.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://kmf.chenzaomai.com

[M05] 设置退出码
来源：http://ddz.jqgufenzy.top

Py:   sys.exit(1)
来源：http://sub.zdqjudy.top

PHP:  exit(1);
来源：http://uvt.jlsjyb.cn

JS:   process.exit(1)
来源：http://ycm.sufxvd.cn

TS:   process.exit(1)
来源：http://mej.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://nso.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://urc.chenjidiqi.icu

Ruby: exit 1
来源：http://bbg.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mvt.yangfankeji.com

[M06] 向标准错误输出
来源：http://zps.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://gpb.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mdy.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://ddk.yangfankeji.com

TS:   console.error("err")
来源：http://azj.wangshuangyany.cn

Java: System.err.println("err")
来源：http://awh.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qhy.aizwys.cn

Ruby: warn "err"
来源：http://xov.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://cfb.aizwys.cn

[M07] 判断是否为主入口
来源：http://nzk.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://ssm.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qjw.sufxvd.cn

JS:   require.main === module
来源：http://ppi.ehwqpu.com

TS:   require.main === module
来源：http://tng.hesvh.cn

Java: public static void main(String[] args)
来源：http://mjj.gzhubu.top

Go:   func main()
来源：http://afa.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://agd.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://twn.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://gwt.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://aqv.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://lyz.redwolf501.top

JS:   process.platform;  process.version
来源：http://fyv.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://aew.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qiw.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://enx.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qjq.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mnp.sufxvd.cn

================================================================================
来源：http://clf.gogol.net.cn

N. 数据结构与算法
来源：http://vxi.tarul.cn

================================================================================
来源：http://ues.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://dlo.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://jdf.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wpy.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ztm.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvb.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://kbg.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://hhv.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bnj.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://nmt.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://vgh.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://aip.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xlc.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zlo.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://pyn.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ysl.tanke756.top

Go:   slices.Sort(arr)
来源：http://ziq.zdqjudy.top

Ruby: arr.sort
来源：http://zkb.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://irp.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://dvh.ybcxt.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ozq.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://npt.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppu.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wri.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://elk.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yen.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rgj.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nef.yj20258.top

[N04] 斐波那契数列
来源：http://bwn.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lml.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wtl.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xkr.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lsw.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hds.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ceh.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rwk.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ksh.nwbrower.top

[N05] 最大公约数
来源：http://pbm.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://kle.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ihs.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jlx.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxt.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://imp.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rip.cashguo.top

Ruby: a.gcd(b)
来源：http://pkj.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://heo.dianchejie.cn

[N06] 判断回文字符串
来源：http://ghy.sxryk.cn

Py:   s == s[::-1]
来源：http://jha.hammf.cn

PHP:  $s === strrev($s);
来源：http://hsh.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://cka.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://lyx.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://exs.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://iqx.havefunace.top

Ruby: s == s.reverse
来源：http://tld.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tmo.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://xdr.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://del.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lvb.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zou.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://lef.zycfv.cn

Java: // 手写 HashMap
来源：http://hzl.yueranfly.top

Go:   // 手写 map[int]int
来源：http://rlt.guannengcc.top

Ruby: // 手写 Hash
来源：http://kkq.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://apg.jqgufenzy.top

[N08] 生成全排列
来源：http://ckd.316326.xyz

Py:   itertools.permutations(arr)
来源：http://pbo.cashguo.top

PHP:  // 手写递归交换
来源：http://vxt.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://oir.yfazqb.com

TS:   // 手写回溯递归
来源：http://wnw.tarul.cn

Java: // 手写回溯递归
来源：http://ypn.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://yxl.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://mzn.cucudq.cn

C#:   // 手写回溯递归
来源：http://che.redwolf501.top

[N09] 栈与队列
来源：http://qwr.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tvb.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qgw.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pnu.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vds.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mvb.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://njn.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ksh.sxryk.cn


<!-- 参考信息 -->