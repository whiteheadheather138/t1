代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pka.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://wxv.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://geh.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fms.zycfv.cn

[K02] JSON 字符串转对象
来源：http://rtp.guannengcc.top

Py:   json.loads(s)
来源：http://tbz.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://egt.yfazqb.com

JS:   JSON.parse(s)
来源：http://ira.wangdashe.top

TS:   JSON.parse(s)
来源：http://ftm.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jbn.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://hpz.yvedp.cn

Ruby: JSON.parse(s)
来源：http://xik.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mle.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://irm.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ksj.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://edb.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://uvc.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sgq.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hvc.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kvu.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://mgx.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gvm.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://oxf.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mue.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tcf.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uvk.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sjk.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ybw.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blh.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tne.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ber.bjfxy.top

[K05] 深拷贝对象
来源：http://aqw.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://pbx.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://flc.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://xbo.cqqwz.cn

TS:   structuredClone(obj)
来源：http://soi.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://utx.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://feg.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xhv.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lyb.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://jlk.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ocy.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hvw.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eii.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://shd.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mgu.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mbu.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rlj.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://enr.xuetiantiany.cn

[K07] 进制转换
来源：http://ukh.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ytk.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hzl.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://deu.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://udw.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kzj.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aaz.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bwe.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qww.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://duo.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://jwv.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lcj.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://nbe.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://ocs.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uli.yangfankeji.com

Go:   encoding/gob
来源：http://wgo.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://ccu.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vml.jinghuilouyu.cn

================================================================================
来源：http://jyf.xuetiantiany.cn

L. 网络请求
来源：http://plp.havefunace.top

================================================================================
来源：http://nkb.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://ycb.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rsv.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ano.sysykeji.top

JS:   await fetch(url)
来源：http://tmr.xziqi.cn

TS:   await fetch(url)
来源：http://fna.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gvd.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://puy.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mid.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zhq.daxiang520.top

[L02] 发送 POST JSON
来源：http://vae.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://nya.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ewz.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hyk.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ooy.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://div.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://njq.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://duo.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dry.smart0.xyz

[L03] 设置自定义请求头
来源：http://xfm.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wet.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wje.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pmy.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pmv.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fkh.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jms.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bpn.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pvm.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://uty.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://clk.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dtu.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bwz.uphjek.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bty.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mzk.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxa.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pso.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://esj.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://hhr.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kqx.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qdh.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mdc.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ynz.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mpn.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tki.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gem.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fpe.316326.xyz

[L06] 解析响应为 JSON
来源：http://nex.jlsjyb.cn

Py:   resp.json()
来源：http://gxj.havefunace.top

PHP:  json_decode($body, true);
来源：http://pdu.yueranfly.top

JS:   await resp.json()
来源：http://zcl.zhixingplan.top

TS:   await resp.json()
来源：http://nje.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lug.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pfi.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://qms.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qku.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://fqb.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tpq.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uvc.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://ecm.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://lgm.316326.xyz

Java: resp.statusCode()
来源：http://jok.tanke756.top

Go:   resp.StatusCode
来源：http://ikr.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://nnr.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://lqg.aibaodan.cn

[L08] 并发请求多个地址
来源：http://gji.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cik.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://oom.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dnx.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://awa.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pry.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vfx.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zym.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://diw.fehbvm.com

================================================================================
来源：http://lle.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://yll.chenlongwang.top

================================================================================
来源：http://xon.yj202588.top

[M01] 读取命令行参数
来源：http://uah.fehbvm.com

Py:   sys.argv[1:]
来源：http://efm.bjfxy.top

PHP:  $argv;  $argc;
来源：http://dtu.cashguo.top

JS:   process.argv.slice(2)
来源：http://lmj.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://jar.yongpay.top

Java: args 数组（main 方法参数）
来源：http://jbi.zhengqikj.top

Go:   os.Args[1:]
来源：http://wfb.xuanzx.com

Ruby: ARGV
来源：http://nbn.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://efh.mhx1999.top

[M02] 读取环境变量
来源：http://rof.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://lam.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yef.ppjwa.cn

JS:   process.env.HOME
来源：http://qcd.ctjpmb.com

TS:   process.env.HOME
来源：http://vbc.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://pra.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cwf.fktsv.cn

Ruby: ENV["HOME"]
来源：http://icb.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://swe.zhijiandao.cn

[M03] 执行外部命令
来源：http://aca.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nhl.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kyn.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nkq.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ljx.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lwm.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bwl.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nym.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://znd.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://yeo.redwolf501.top

Py:   os.getcwd()
来源：http://auw.fehbvm.com

PHP:  getcwd();
来源：http://zho.sjlbkw.cn

JS:   process.cwd()
来源：http://ela.9152youxi.cn

TS:   process.cwd()
来源：http://avz.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://gwr.fktsv.cn

Go:   os.Getwd()
来源：http://cvh.jqgufenzy.top

Ruby: Dir.pwd
来源：http://rud.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cvo.ppjwa.cn

[M05] 设置退出码
来源：http://ipv.xuanzx.com

Py:   sys.exit(1)
来源：http://ikw.smart0.xyz

PHP:  exit(1);
来源：http://bnz.gzhubu.top

JS:   process.exit(1)
来源：http://eav.tian-w.cn

TS:   process.exit(1)
来源：http://uha.sxryk.cn

Java: System.exit(1)
来源：http://ssv.hfpthk.cn

Go:   os.Exit(1)
来源：http://ptq.smart0.xyz

Ruby: exit 1
来源：http://hmu.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gax.nanxuanxn.top

[M06] 向标准错误输出
来源：http://bmk.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://ikh.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://rci.xinyue.icu

JS:   console.error("err")
来源：http://ppt.ivvv.top

TS:   console.error("err")
来源：http://cif.sysykeji.top

Java: System.err.println("err")
来源：http://wpx.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ghu.gzhubu.top

Ruby: warn "err"
来源：http://uut.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://won.birdmap.top

[M07] 判断是否为主入口
来源：http://hnn.gaohongyu789.top

Py:   if __name__ == "__main__":
来源：http://eeg.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dep.guowangkeji.top

JS:   require.main === module
来源：http://zsu.chenlongwang.top

TS:   require.main === module
来源：http://ned.wangdashe.top

Java: public static void main(String[] args)
来源：http://gdv.gogol.net.cn

Go:   func main()
来源：http://iqj.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rbf.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://wwr.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://ykh.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://wkz.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://yhe.ctjpmb.com

JS:   process.platform;  process.version
来源：http://gxf.yj20258888.top

TS:   process.platform;  process.version
来源：http://hmc.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://izp.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qyl.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://swl.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://ksz.yfazqb.com

================================================================================
来源：http://nmm.epnwcf.com

N. 数据结构与算法
来源：http://jcv.fanxiaobao.xyz

================================================================================
来源：http://jsh.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://uld.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ulx.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uzk.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsp.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cca.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qhf.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://epy.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ttq.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nnk.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://jdh.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://gto.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://atq.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hms.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://rhn.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zvs.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://hdw.yvedp.cn

Ruby: arr.sort
来源：http://gnf.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yie.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://plr.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bph.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://axf.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sfd.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oow.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zxt.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dya.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vzs.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://bbd.sysykeji.top

[N04] 斐波那契数列
来源：http://vvw.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kkk.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://joc.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://top.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bms.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://djr.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gpm.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nzm.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hle.xuetiantiany.cn

[N05] 最大公约数
来源：http://eue.aizwys.cn

Py:   math.gcd(a, b)
来源：http://isy.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oom.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yjz.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qjd.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ylz.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wbv.tanke756.top

Ruby: a.gcd(b)
来源：http://qfv.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uzg.cqqwz.cn

[N06] 判断回文字符串
来源：http://cki.yangfankeji.com

Py:   s == s[::-1]
来源：http://wnl.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://omp.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://nbi.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://nli.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uxw.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://nad.zhixingplan.top

Ruby: s == s.reverse
来源：http://rey.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fay.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://mwh.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ljj.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dhx.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hud.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://tng.cqqwz.cn

Java: // 手写 HashMap
来源：http://afa.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://ilw.shzxlz.cn

Ruby: // 手写 Hash
来源：http://nox.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://sbi.iojbl.cn

[N08] 生成全排列
来源：http://wkd.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://nxz.xziqi.cn

PHP:  // 手写递归交换
来源：http://oqf.gogol.net.cn

JS:   // 手写回溯递归
来源：http://gdk.xinyue.icu

TS:   // 手写回溯递归
来源：http://jcy.gzhubu.top

Java: // 手写回溯递归
来源：http://chm.cheryme.top

Go:   // 手写回溯递归
来源：http://zbv.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://vrj.zdqjudy.top

C#:   // 手写回溯递归
来源：http://ppe.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://dvv.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lsr.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wql.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dcq.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uxn.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xre.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qfq.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://edp.xziqi.cn


<!-- 参考信息 -->